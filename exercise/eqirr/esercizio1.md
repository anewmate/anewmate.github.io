# EQUAZIONI IRRAZIONALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente equazione irrazionale

$$3-4x-\sqrt{x^2-1} = 4-3x$$

## Soluzione:

Come prima cosa isoliamo la radice a sinistra dell'uguaglianza e portiamo a destra tutto il resto, ricordandoci di cambiare segno quando spostiamo gli elementi da una parte all'altra dell'uguale.

$$\begin{align*}
-\sqrt{x^2-1} & = 4-3x-3+4x \\
-\sqrt{x^2-1} & = x+1
\end{align*}$$

Moltiplico infine tutto per -1:

$$\begin{align*}
(-1)(-\sqrt{x^2-1}) & = (x+1)(-1) \\
\sqrt{x^2-1}& = -x-1
\end{align*}$$

Dato che l'indice della radice è pari, l'equazione è equivalente al sistema 

$$\begin{cases}
x^2-1 \geq 0 \\
-x-1 \geq 0 \\
x^2-1 = (-x-1)^2
\end{cases}$$

Sostanzialmente dobbiamo porre l'argomento della radice e il termine destro dell'uguaglianza maggiori di zero e poi possiamo elevare tutto al quadrato, mettendo le tre condizioni a sistema. 

La prima disuguaglianza diventa 

$$\begin{align*}
x^2-1 & \geq 0 \\
x^2 & \geq 1 \\
& \downarrow \\
\text{equazione} & \; \text{associata}\\
x^2 & = 1 \\
x & = \pm 1 \\
& \downarrow \\
\text{avevo} \geq & \Rightarrow \text{intervalli esterni} \\
x \leq -1 & \cup x \geq 1
\end{align*}$$

La seconda disuguaglianza diventa 

$$\begin{align*}
-x-1 & \geq 0 \\
-x & \geq 1 \\
(-1)(-x) & \leq 1(-1) \\
x & \leq -1
\end{align*}$$

dove nel penultimo passaggio ho cambiato il verso della disuguaglianza perchè ho moltiplicato per un numero negativo.

La terza equazione diventa 

$$\begin{align*}
x^2-1 & = (-x-1)^2 \\
x^2-1 & = (-(x+1))^2 \\
x^2-1 & = (-)^2 \cdot (x+1)^2 \\
x^2-1 & = x^2+1+2x \\
x^2-1-x^2-1-2x & = 0 \\
-2x-2 & = 0 \\
-2x & = 2 \\
\frac{-2x}{-2} & = \frac{2}{-2} \\
x & = -1
\end{align*}$$

dove nel quarto passaggio ho utilizzato la formula di sviluppo di binomio $$(A\pm B)^2 = A^2 + B^2 \pm 2AB$$ e con $$(-)^2$$ si intende meno per meno, ossia più. 

Il sistema diventa quindi 

$$\begin{cases}
 x \leq -1  \cup x \geq 1\\
x \leq -1 \\
x = -1
\end{cases}$$

$$\begin{tikzpicture}
\draw (-2,0)--(2,0);
\draw (-1,-0.2)--(-1,3);
\draw (1,-0.2)--(1,3);
\node at (-1,-0.5) {$-1$};
\node at (1,-0.5) {$1$};
\node at (-3,0.5) {\scriptsize $x=-1$};
\node at (-3,1.5) {\scriptsize $x\leq -1$};
\node at (-3.3,2.5) {\scriptsize $x\leq -1 \cup x \geq 1$};
\draw[fill=black] (-1,0.5) circle (0.1cm);
\draw[fill=black] (-1,1.5) circle (0.1cm);
\draw[fill=black] (-1,2.5) circle (0.1cm);
\draw[fill=black] (1,2.5) circle (0.1cm);
\draw (-1,2.5) -- (-2,2.5);
\draw (-1,1.5) -- (-2,1.5);
\draw (1,2.5) -- (2,2.5);
\end{tikzpicture}$$

Poichè abbiamo un sistema, dobbiamo scegliere le soluzioni comuni a tutte le equazioni, se ci sono. In questo caso l'unica soluzione presente in tutti e tre i casi è

$$x=-1$$

che è quindi soluzione finale dell'equazione iniziale. 

