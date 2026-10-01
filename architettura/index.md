# Architettura degli elaboratori

Calcolatore:
Insieme di componenti connesse tra loro

Visione gerarchica:
Insieme di sottosistemi correlati
Ogni sistema ad un livello si basa sulla descrizione astratta del livello successivo

Ad ogni livello:

- Struttura: come sono correlati i componenti
- Funzione: cosa fa ciascun componente

Descrizione top-down:

- Da componenti principali a sottocomponenti, fino a una descrizione completa dei dettagli

# Funzioni basilari di un calcolatore (livello più alto della gerarchia)

- Elaborazione dati (CPU)
- Memorizzazione dati (RAM)
- Trasmissione dati (BUS, I/O)

## 4 componenti principali

- CPU
- Memoria centrale
- I/O
- Interconnessioni (Bus)

# CPU

- Unità di controllo
- ALU (Arithmetic Logic Unit)
- Registri (memoria interna della CPU)
- Bus interno

## Unità di controllo

- Logica di sequenzializzazione
- Regostri di controllo e decodificatori
- Memoria di controllo

# Notazioni

Ogni cifra è moltiplicata per il peso associato a quella posizione.
ad esempio, in base 10:
$375 = 3*10^2 + 7*10^1 + 5*10^0
    $

$= 3*100 + 7*10 + 5$

Stessa cosa per la base 2

## In binario

111 è uguale a 1000 - 1 (dimostrabile con equazione)

# Ordini di grandezza

byte = 8 bit
kB = 1000 byte  ($10^3$)
MB = 1000 kB    ($10^6$)
GB = 1000 MB    ($10^9$)
TB = 1000 GB     ($10^{12}$)

## Notazione ottale

Un simbolo per ogni gruppo di 3 cifre binarie.
Esempio da bin a oct:  `000` = $0$   `001` = $1$   `010` = $2$   etc.

## Notazione esadecimale

Un simbolo per ogni gruppo di 4 cifre binarie (da 0 a 15)
`0 = 0` `9 = 9` `10 = A` `11 = B` `12 = C` `13 = D` `14 = E` `15 = F`

## Algebra di boole

Operazioni logiche: `AND`, `OR`, `NOT`, `XOR`

Puoi realizzare tutti i circuiti usando solo porte `NOR` o `NAND`: tutte le altre porte possono essere realizzate con una combinazione di porte `NOR`.

`AND` = moltiplicazione
`OR` = somma
`NOT` = negazione
`XOR` = differenza (vero se i due valori sono diversi)



## Operazioni di 4 tipi

- Processore-memoria

- Processore-I/O

- Elaborazione dati

- Controllo (salti)

## Esempio

- Ipotetica macchina con registri PC (Program Counter), IR (Instruction Register), AC (accumulatore, accumula gli input e i risultati delle operazioni)

- Parole di M di 16 bit

- Dati e istruzioni di 16 bit

- Alcuni codici operativi (4 bit: 16 diversi codici):
  
  - 0001 (1): carica in AC una cella di M
  - 0010 (2): scrive in M il contenuto di AC
  - 0101 (5): somma una cella di M ad aC

- $2^{12}$ celle indirizzabili in una istruzione

## Ciclo di esecuzione

- Instrution fetch

- Instruction operation decoding

- Operand address calculation

- Operand fetch

- Data operation (operazione vera e propria, ad es. nell'ALU)

- Operand address calculation (calcolo dove mettere il risultato, se applicabile)

- Operand store (salvo il risultato)

## Interruzioni

- Altri moduli (es. I/O) possono interrompere la normale sequenza di esecuzione

- Tipiche interruzioni:
  
  - Program (overflow, div by zero)
  - Timer (generata da un timer CPU)
  - I/O (fine di un'operazione I/O)

Le interruzioni permettono di accorciare l'attesa per gli eventi I/O, ma non è sempre possibile e non dipende tanto dal programmatore, quanto dalla concatenazione degli eventi e la velocità delle periferiche.

## Ciclo di interruzione

- aggiunto al ciclo di esecuzione

- La CPU controlla se ci sono interruzioni pendenti

- Se no, prende la prossima istruzione

- Se si:
  
  - Sospende l'esecuzione del programma corrente
  - Salva il contesto e i registri
  - Salta al programma di gestione dell'interruzione e lo esegue
  - Rimette il contesto al suo posto e continua il programma interrotto
