# PIANO CARTESIANO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Rappresenta nel piano cartesiano gli insiemi di punti $$P(x;y)$$ le cui coordinate soddisfano le seguenti condizioni.

$$\begin{cases}
-2 \leq x \leq 3 \\
-3 \leq y < 0
\end{cases}$$


## Soluzione: 

Come prima cosa disegno un sistema di riferimento cartesiano.

$$\begin{tikzpicture}
\draw[->] (-4,0) -- (4,0);
\draw [->] (0,-4) -- (0,4);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\node at (4.5,0) {$x$};
\node at (0,4.5) {$y$};
\end{tikzpicture}$$

Ricordo che l'asse delle $$x$$ si chiama asse delle ascisse mentre l'asse $$y$$ è l'asse delle ordinate. 

Disegno la prima condizione $$-2 \leq x \leq 3$$. Una volta che individuo gli estremi $$x = -2$$ e $$x = 3$$ non devo fare altro che prendere tutto lo "spazio" compreso fra questi due numeri (estremi inclusi). 

$$\begin{tikzpicture}
\shade[top color=red!40!white, bottom color = red!40!white, middle color = red] (-2,4) rectangle (3,-4);
\draw[->] (-4,0) -- (4,0);
\draw [->] (0,-4) -- (0,4);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\draw[red,thick] (-2,-4) -- (-2,4);
\draw[red,thick] (3,-4) -- (3,4);
\node at (4.5,0) {$x$};
\node at (0,4.5) {$y$};
\end{tikzpicture}$$

Disegno la seconda condizione $$-3 \leq y < 0$$. Una volta che individuo gli estremi $$y = -3$$ e $$y = 0$$ non devo fare altro che prendere tutto lo "spazio" compreso fra questi due numeri ($$-3$$ incluso mentre zero no). 

$$\begin{tikzpicture}
\shade[top color=green!40!white, bottom color = green!40!white, middle color = green] (-4,0) rectangle (4,-3);
\draw[->] (-4,0) -- (4,0);
\draw [->] (0,-4) -- (0,4);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\draw[green,thick, dashed] (-4,0) -- (4,0);
\draw[green,thick] (-4,-3) -- (4,-3);
\node at (4.5,0) {$x$};
\node at (0,4.5) {$y$};
\end{tikzpicture}$$

Devo infine prendere l'intersezione di queste due strisce di piano, ossia quella parte di piano cartesiano dove ci sono entrambe le strisce. I punti $$P(x;y)$$ le cui coordinate soddisfano le condizioni 

$$\begin{cases}
-2 \leq x \leq 3 \\
-3 \leq y < 0
\end{cases}$$

sono quelli colorati in giallo qui sotto. Per chiarezza, i bordi sono indicati in viola (per capire se gli estremi sono inclusi o no).

$$\begin{tikzpicture}
\shade[top color=yellow!40!white, bottom color = yellow!40!white, middle color = yellow] (-2,0) rectangle (3,-3);
\draw[->] (-4,0) -- (4,0);
\draw [->] (0,-4) -- (0,4);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\draw[violet,ultra thick, dashed] (-2,0) -- (3,0);
\draw[violet,ultra thick] (-2,-3) -- (3,-3);
\draw[violet,ultra thick] (-2,-3) -- (-2,0);
\draw[violet,ultra thick] (3,0) -- (3,-3);
\node at (4.5,0) {$x$};
\node at (0,4.5) {$y$};
\end{tikzpicture}$$