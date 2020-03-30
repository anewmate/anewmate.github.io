# INTEGRALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Calcola il seguente integrale

$$\int \frac{x^2+5x-1}{x^3+x^2-2}dx$$

## Soluzione: 

Come prima cosa noto che l'integrale è indefinito. Come seconda cosa noto che ho una frazione di polinomi come argomento dell'integrale. L'integrazione di funzioni razionali fratte, segue delle regole precise.

***
Nell'integrazione di funzioni razionali fratte $$\int \frac{N(x)}{D(x)}dx$$ quando il **grado del numeratore è minore di quello del denominatore**:

*  se il numeratore è la derivata del denominatore:

$$\int \frac{f^{'}(x)}{f(x)} dx = \ln(|f(x)|)+c$$

* se il denominatore è di primo grado:

$$\int \frac{1}{ax+b}dx = \frac{1}{a}\ln(|ax+b|)+c$$

* se il denominatore è di secondo grado:

1. se $$\Delta > 0$$: essendo $$ax^2+bx+c = a(x-x_1)(x-x_2)$$, si cercano i valori $$A$$ e $$B$$ tali che

$$\frac{px+q}{ax^2+bx+c} = \frac{A}{a(x-x_1)}+\frac{B}{x-x_2}$$

2. se $$\Delta = 0$$: essendo $$ax^2+bx+c = a(x-x_1)^2$$, si cercano i valori $$A$$ e $$B$$ tali che

$$\frac{px+q}{ax^2+bx+c} = \frac{A}{a(x-x_1)}+\frac{B}{(x-x_1)^2}$$

3. se $$\Delta < 0$$: allora $$\int \frac{1}{ax^2+bx+c}dx$$ si trasforma in modo da utilizzare la formula

$$\int \frac{f^{'}(x)}{k^2+(f(x))^2}dx = \frac{1}{k}\arctan\left(\frac{f(x)}{k}\right) +c$$

mentre $$\int \frac{px+q}{ax^2+bx+c}dx$$ si trasforma nella somma 

$$r\int \frac{2ax+b}{ax^2+bx+c}dx + s\int \frac{1}{ax^2+bx+c}dx$$

dove gli integrali si risolvono con i metodi precedenti. 

* se il denominatore è di grado superiore al secondo, occorre scomporlo in fattori irriducibili e riscrivere la frazione come somma di frazioni con numeratori di primo e di secondo grado.

Quando, nell'integrale $$\int \frac{N(x)}{D(x)}dx$$, il **grado del numeratore è maggiore o uguale di quello del denominatore** si ritorna ai casi precedenti mediante la divisione polinomiale: $$\frac{N(x)}{D(x)} = Q(x) + \frac{R(x)}{D(x)}$$ dove il grado di $$R(x)$$ è minore di quello di $$D(x)$$.

***

Nel nostro caso abbiamo che il grado del numeratore (ossia 2) è minore del grado del denominatore (ossia 3).

Regola mi dice che devo scomporre il denominatore in fattori irriducibili e riscrivere la frazione come somma di frazioni con numeratori di primo e di secondo grado. Parto quindi scomponendo il denominatore.

Per scomporre il denominatore utilizzo la formula di Ruffini. Vedo subito che $$x=1$$ è una radice del polinomio $$x^3+x^2-2$$ in quanto

$$(1)^3+(1)^2-2 = 0$$

Quindi 

$$\begin{tikzpicture}
\draw (-0.25,0) -- (3,0);
\draw (0.25,1.5)--(0.25,-0.5);
\draw (2.2,1.5)--(2.2,-0.5);
%\node at (0.25,1) {$1$};
\node at (0.75,1) {$1$};
\node at (1.25,1) {$1$};
\node at (1.75,1) {$0$};
\node at (2.5,1) {$-2$};
\node at (0,0.5) {$1$};
%\node at (0.25,-0.25) {$1$};
%\node at (0.75,0.5) {$1$};
\node at (0.75,-0.25) {$1$};
\node at (1.25,0.5) {$1$};
\node at (1.25,-0.25) {$2$};
\node at (1.75,0.5) {$2$};
\node at (1.75,-0.25) {$2$};
\node at (2.5,0.5) {$2$};
\node at (2.5,-0.25) {$0$};
\end{tikzpicture}$$

e posso scomporre $$x^3+x^2-2$$ come

$$(x-1)(x^2+2x+2)$$

Calcolo il delta di $$x^2+2x+2$$ per vedere se si può scomporre ulteriormente. 

$$\Delta = b^2-4ac = 4-4(1)(2) = -4 < 0$$

Essendo il delta negativo, $$x^2+2x+2$$ è irriducibile. 

Devo ora scrivere la frazione iniziale come somma di due frazioni con denominatori rispettivamente $$x-1$$ e $$x^2+2x+2$$. Ossia devo trovare $$A$$, $$B$$ e $$C$$ numeri reali tali che

$$\frac{x^2+5x-1}{x^3+x^2-2} = \frac{A}{x-1} + \frac{Bx+C}{x^2+2x+2}$$

Per trovarli facciamo la somma di quelle due frazioni:

$$\begin{align*}
\frac{A}{x-1} + \frac{Bx+C}{x^2+2x+2} & = \frac{A(x^2+2x+2)+(Bx+C)(x-1)}{(x-1)(x^2+2x+2)} \\
& = \frac{Ax^2+2Ax+2A+Bx^2-Bx+Cx-C}{(x-1)(x^2+2x+2)} \\
& = \frac{x^2(A+B)+x(2A-B+C)+2A-C}{(x-1)(x^2+2x+2)}
\end{align*}$$

Poichè deve valere l'uguaglianza 

$$\frac{x^2(A+B)+x(2A-B+C)+2A-C}{(x-1)(x^2+2x+2)} = \frac{x^2+5x-1}{(x-1)(x^2+2x+2)}$$

devo avere 

$$\begin{cases}
A+B & = 1 \\
2A-B+C & = 5 \\
2A-C & = -1
\end{cases}$$

Risolviamo il sistema: isolo $$A$$ dalla prima equazione e lo sostituisco nelle altre due.

$$\begin{cases}
A & = 1 -B\\
2(1-B)-B+C & = 5 \\
2(1-B) -C& = -1
\end{cases}$$

Isolo $$C$$ dalla seconda equazione e lo sostituisco nella terza.

$$\begin{cases}
A & = 1 -B\\
C & = 3 +3B\\
2-2B -(3+3B)& = -1
\end{cases}$$

Risolvo la terza equazione solo in $$B$$.

$$\begin{cases}
A & = 1 -B\\
C & = 3 +3B\\
B & = 0
\end{cases}$$

Sostituendo il $$B$$ trovato nelle prime due equazioni ottengo

$$\begin{cases}
A & = 1 \\
C & = 3 \\
B & = 0
\end{cases}$$

Quindi 

$$\begin{align*}
\frac{x^2+5x-1}{(x-1)(x^2+2x+2)} & = \frac{A}{x-1} + \frac{Bx+C}{x^2+2x+2} \\
& = \frac{1}{x-1} + \frac{3}{x^2+2x+2}
\end{align*}$$

e di conseguenza 

$$\begin{align*}
\int \frac{x^2+5x-1}{(x-1)(x^2+2x+2)}dx
& = \int \left( \frac{1}{x-1} + \frac{3}{x^2+2x+2}\right) dx \\
& = \int \frac{1}{x-1}dx + \int \frac{3}{x^2+2x+2}dx
\end{align*}$$

Il primo integrale è immediato e si ha 

$$\int \frac{1}{x-1}dx = \ln(|x-1|)$$

mentre per il secondo 

$$\begin{align*}
\int \frac{3}{x^2+2x+2}dx & = 3 \int \frac{1}{x^2+2x+2}dx \\
& = 3 \int \frac{1}{(x^2+2x+1)+1} dx \\
& = 3 \int \frac{1}{(x+1)^2+1}dx \\
& = 3 \arctan(x+1)
\end{align*}$$

Alla fine quindi si ha

$$\int \frac{x^2+5x-1}{x^3+x^2-2}dx = \ln(|x-1|) + 3\arctan(x+1) +c$$






