# DISEQUAZIONI IRRAZIONALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente disequazione irrazionale

$$\sqrt{x-1} > x-3$$

## Soluzione:

Come prima cosa notiamo che la disequazione è già scritta "bene", nel senso che il termine con la radice è a sinistra e tutto il resto a destra della disuguaglianza. Ci basta quindi solo applicare la formula. Siamo nel caso di indice di radice pari (uguale a $$2$$) con disequazione del tipo $$\sqrt{A(x)} > B(x)$$. Formula ci dice che la disuguaglianza è equivalente a risolvere 

$$\begin{cases}
A(x) \geq 0 \\
B(x) < 0 
\end{cases} \vee
\begin{cases}
B(x) \geq 0  \\
A(x) > (B(x))^2
\end{cases}$$

dove, nel nostro caso, $$A(x) = x-1$$ e $$B(x) = x-3$$.  I sistemi diventano quindi 

$$\begin{cases}
x-1 \geq 0 \\
x-3 < 0 
\end{cases} \vee
\begin{cases}
x-3 \geq 0  \\
x-1 > (x-3)^2
\end{cases}$$

Partiamo con la risoluzione del primo sistema.

$$\begin{align*}
& \begin{cases}
x-1 \geq 0 \\
x-3 < 0 
\end{cases} \\
& \begin{cases}
x \geq 1 \\
x < 3 
\end{cases}
\end{align*}$$

$$\begin{tikzpicture}
\draw[fill=yellow] (-1,2) rectangle (1,0);
\draw (-2,0)--(2,0);
\draw (-1,-0.2)--(-1,2);
\draw (1,-0.2)--(1,2);
\node at (-1,-0.5) {$1$};
\node at (1,-0.5) {$3$};
\node at (-3,0.5) {\scriptsize $x \geq 1$};
\node at (-3,1.5) {\scriptsize $x < 3$};
\draw[fill=black] (-1,0.5) circle (0.1cm);
\draw (1,1.5) circle (0.1cm);
\draw (1,1.5) -- (-2,1.5);
\draw (-1,0.5) -- (2,0.5);
\end{tikzpicture}$$

La soluzione del primo sistema è quindi 

$$1 \leq x < 3$$

Passiamo a risolvere il secondo sistema. 

$$\begin{align*}
& \begin{cases}
x-3 \geq 0 \\
x-1 > (x-3)^2 
\end{cases} \\
& \begin{cases}
x \geq 3 \\
x-1 > x^2 + 9 - 6x 
\end{cases} \\
& \begin{cases}
x \geq 3 \\
x-1 -x^2 -9 + 6x > 0 
\end{cases} \\
& \begin{cases}
x \geq 3 \\
-x^2 +7x -10> 0 
\end{cases} \\
& \begin{cases}
x \geq 3 \\
x^2 -7x +10 < 0 
\end{cases}
\end{align*}$$

Risolviamo a parte la disequazione di secondo grado. Ricordo che gli step per risolverla sono 

1. arrivare a una forma del tipo $$ax^2+bx+c \gtrless 0$$ con $$\underline{\mathbf{a > 0}}$$;
1. risolvere l'equazione associata $$ax^2+bx+c = 0$$ e trovare le soluzioni $$x_1,x_2$$ con $$x_2 \leq x_1$$;
1. se avevo $$ax^2+bx+c > 0$$ prendo gli intervalli esterni: $$x < x_2 \cup x > x_1$$
1. se avevo $$ax^2+bx+c < 0$$ prendo l'intervallo interno: $$x_2 < x < x_1$$
1. Nota: le disuguaglianze nelle soluzioni sono strette o no in base a quelle di partenza.

Risolvo quindi la nostra disuguaglianza:

$$\begin{align*}
x^2-7x+10 & < 0 \\
& \downarrow \\
\text{equazione} & \; \text{associata}\\
x^2 -7x + 10& = 0 \\
x_{1/2} & = \frac{7\pm \sqrt{49-4(1)(10)}}{2} \\
x_{1/2} & = \frac{7\pm \sqrt{49-40}}{2} \\
x_{1/2} & = \frac{7\pm \sqrt{9}}{2} \\
x_{1/2} & = \frac{7\pm 3}{2} \\
x_{1/2} & = \begin{cases}
5 \\
2
\end{cases} \\
& \downarrow \\
\text{avevo} < & \Rightarrow \text{intervallo interno} \\
2 < \; & x < 5
\end{align*}$$

Il secondo sistema diventa quindi

$$\begin{align*}
& \begin{cases}
x \geq 3 \\
x^2 -7x +10 < 0 
\end{cases} \\
& \begin{cases}
x \geq 3 \\
2 < x < 5 
\end{cases}
\end{align*}$$ 

$$\begin{tikzpicture}
\draw[fill=yellow] (0,2) rectangle (1,0);
\draw (-2,0)--(2,0);
\draw (-1,-0.2)--(-1,2);
\draw (0,-0.2)--(0,2);
\draw (1,-0.2)--(1,2);
\node at (-1,-0.5) {$2$};
\node at (0,-0.5) {$3$};
\node at (1,-0.5) {$5$};
\node at (-3,0.5) {\scriptsize $x \geq 3$};
\node at (-3,1.5) {\scriptsize $2<x<5$};
\draw[fill=black] (0,0.5) circle (0.1cm);
\draw (1,1.5) circle (0.1cm);
\draw (-1,1.5) circle (0.1cm);
\draw (1,1.5) -- (-1,1.5);
\draw (0,0.5) -- (2,0.5);
\end{tikzpicture}$$

La soluzione di questo sistema è quindi 

$$3 \leq x < 5$$

Poichè la soluzione finale è data dall'unione delle soluzioni dei due sistemi, si ha 

$$1 \leq x < 3 \cup 3 \leq x < 5$$

ossia

$$1 \leq x < 5$$


