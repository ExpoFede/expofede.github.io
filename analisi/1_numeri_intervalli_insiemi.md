# Numeri

$N = \{0, 1, 2, ...\}$ Numeri naturali

$Z = N \cup (-N)$ Numeri interi $-1, 0, 1, 2$

$Q = \{p/q : p \in Z, q \in N-\{0\} \}$ Numeri razionali 0, 2/5, 3

Crisi pitagorica: i greci si sono resi conto che i numeri razionali non erano capaci di rappresentare la lunghezza dell'ipotenusa.

## Proprietà di densità di Q

Esistono infiniti elementi $n \in Q \mid a < n < b$

## Numeri reali

I numeri razionali sono un sottoinsieme dei numeri reali

$R - Q$ = numeri irrazionali

I numeri reali sono rappresentabili su una retta. Sono essenzialmente $]-\infty, +\infty [ $

R esteso = $R \cup \{-\infty, +\infty\} $

# Intervalli

Un intervallo è un sottoinsieme $I \subseteq R$ tale che per ogni coppia $a,b \in I$ se $a < r < b$ allora $r \in I$

$[a, b]$ è un intervallo chiuso (include $a$ e $b$)

$]a, b[$ è un intervallo aperto (non include $a$ e $b$)

## Modulo di un numero

Fissato $x \in R$, si dice modulo o valore assoluto di x la quantità definita da

$|x| = \begin{cases} x \text{ se } x >= 0 \\ -x \text{ se } x < 0\end{cases}$

$|x1 - x2|$ rappresenta la distanza tra $x1$ e $x2$

$|x| \leq M <=> -M \leq x \leq M$

### Teorema della disuguaglianza triangolare

$|x+y| \leq |x| + |y|$

# Insiemi limitati

$A \subseteq R$ si dice limitato se esiste un intervallo chiuso che lo contiene. Altrimenti è illimitato.

Un numero $\beta$ è maggiorante di $A$ se è $\geq$ di ogni elemento di $A$, ed è minorante se è $\leq$ di ogni elemento di $A$.

Superiormente limitato: esiste un maggiorante. Inferiormente limitato: esiste un minorante.

Un minorante di $A$ appartenente ad $A$ si dice minimo e si indica $min \text{ } A$. Idem per il massimo: è un maggiorante di $A$ appartenete ad $A$.

*Esempio*: $[2,4[$ ha minimo $2$, ma non ha massimo.

*Proposizione*: $A \subseteq R$. Se esistono, $min\text{ }A$ e $max\text{ }A$ sono unici.

## Estremo superiore e inferiore (min/max)

Sia $A \subseteq R$. Si dice estremo superiore di $A$ e si indica con $sup\text{ }A$ il minimo dell'insieme dei maggioranti di $A$.

Si dice estremo inferiore di $A$ e si indica con $inf\text{ }A$ il massimo dell'insieme dei minoranti di $A$.

*Teorema di completezza, seconda forma*: Ogni sottinsieme A di R superiormente limitato ha uno e uno solo estremo superiore. E viceversa per l'estremo inferiore.

Proposizione:

- Se $A$ è sup. limitato e $sup\text{ }A \in A$ allora $sup\text{ }A = max\text{ }A$

In $Q$ non possiamo enunciare un teorema di completezza come sopra. Infatti

$A = \{ x \in Q^{\geq 0} : x^2 \leq 2 \} $

Teorema della caratterizzazione di sup e inf:

Se $A \subseteq R, A \neq \varnothing$ sup limitato, allora

$$
S = sup\text{ }A <=> \begin{cases}
S \geq a \forall a \in A \text{     S è maggiorante} \\
\forall \epsilon > 0 \exists a \in A \mid a > S - \epsilon
\end{cases}
$$

Idem per gli inferiori.

*Teorema proprietà di archimede*: Se abbiamo due numeri reali positivi, allora esiste $n \in N \mid n*a > b$

*Teorema densità di Q in R*: per qualunque coppia di numeri reali esiste un razionale in mezzo


