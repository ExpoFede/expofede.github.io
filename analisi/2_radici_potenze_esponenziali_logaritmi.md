# Radici, potenze, esponenziali, logaritmi

Teorema: siano $y \in R$, $y \geq 0$, $n \in N$ e $n >= 1$. Allora esiste ed è unico $\exists!$ x >= 0 tale che $x^n = y$. Tale numero $x$ viene indicato con uno dei simboli $\sqrt[n]{y}$ o $y^{1/n}$ e viene definito radice n-esima di y.

Radice $n$-esima di x è definito solo per $x \geq 0$ (in realtà per $n$ dispari potrebbe esistere, ma per semplicità non lo consideriamo). Se devo risolvere $x^3 = -27$, scrivo $x = -\sqrt[3]{27}$

Osservazione: $|x| = \sqrt{x^2}$

Osservazione: $\sqrt[n]{ab} = \sqrt[n]{a} \times \sqrt[n]{b}$

## Potenze

Siano $a > 0$, $r \in Q$, $r = p / q$, $q > 0$

$a^p = a*a*a... \text{(p volte) se }p\geq0$ e $p \in N$

Definiamo

$a^r = a^{p/q} = (a^p)^{1/q} = ^q\sqrt{a^p}$

Osservazione: $a^{-n}$ = $(\frac{1}{a})^{n}$

Come definisco la potenza $a^r$ nei numeri reali?

1. $r \in R^{>0}$
   Se a>1, r = $p, \alpha1, \alpha2, \alpha3...$ ($\alpha$ sono cifre dopo la virgola), sto considerando la successione $a^p\leq a^{p,\alpha1} \leq a^{p,\alpha1,\alpha2}$
   $a^r = sup \{a^{p,\alpha1,\alpha2,...\alpha n} | n \in N \}$
- caso 2: $1^r = 1$

- caso 3: $0<a<1$

$a^r = \frac{1}{(1/a)^r}$

### Numero di Nepero $e=2,71828...$

È un numero irrazionale.

Sarà importante: $e^x$ con $x \in R$

- Se $a>1$, $a^x$ è crescente

- Se $0 < a < 1$, $a^x$ è decrescente

## Logaritmi

Teorema: $a, y \in R$, $a,y>0$, $a\ne1$. Allora $\exists!$ $x \in R$ tale che $a^x = y$

Tale numero si dice logaritmo in base $a$ di $y$ e si indica con $log_a{y}$

$log_ay = sup\{r\in R | a^r \leq y\}$ se $a > 1$

$log_ay = sup\{r\in R | a^r \geq y\}$ se $0<a<1$

Oss: $a^{log_ay} = y = log_aa^y$

Oss: $a^x>0 \forall x\in R, \forall a>0$

Il logaritmo con base $a > 1$ è crescente, base $0<a<1$ è decrescente.

### Proprietà algebriche dei logaritmi

- $\log_a(x \cdot y) = \log_a(x) + \log_a(y)$

- $\log_a(x / y) = \log_a(x) - \log_a(y)$

- $\log_a(x^k) = k \cdot \log_a(x)$

- $\log_a(x) = \frac{\log_b(x)}{\log_b(a)}$

- $\log_a(b) = \frac{1}{\log_b(a)}$
