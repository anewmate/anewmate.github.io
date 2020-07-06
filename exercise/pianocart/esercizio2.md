# PIANO CARTESIANO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> In un riferimento cartesiano, disegna i punti 

$$A(-3;-4), B(-4;0), C(-2;-1),$$

$$D(0,5), E(2,3), F(1,-3)$$

## Soluzione: 

Come prima cosa disegno un sistema di riferimento cartesiano.

$$\begin{tikzpicture}
\draw[->] (-6,0) -- (6,0);
\draw [->] (0,-6) -- (0,6);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (4,-0.2) -- (4,0.2);
\draw (5,-0.2) -- (5,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-4,-0.2) -- (-4,0.2);
\draw (-5,-0.2) -- (-5,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,4) -- (0.2,4);
\draw (-0.2,5) -- (0.2,5);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\draw (-0.2,-4) -- (0.2,-4);
\draw (-0.2,-5) -- (0.2,-5);
\node at (6.5,0) {$x$};
\node at (0,6.5) {$y$};
\end{tikzpicture}$$

Ricordo che l'asse delle $$x$$ si chiama asse delle ascisse mentre l'asse $$y$$ è l'asse delle ordinate. 

Partiamo disegnando il punto $$A(-3;-4)$$: questo punto ha $$x = -3$$ e $$y = -4$$. Questo significa che mi devo spostare sull'asse delle $$x$$ di $$-3$$, ossia di tre unità a sinistra dello zero, e sull'asse delle $$y$$ di $$-4$$, ossia di quattro unità sotto lo zero.

$$\begin{tikzpicture}
\draw[->] (-6,0) -- (6,0);
\draw [->] (0,-6) -- (0,6);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (4,-0.2) -- (4,0.2);
\draw (5,-0.2) -- (5,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-4,-0.2) -- (-4,0.2);
\draw (-5,-0.2) -- (-5,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,4) -- (0.2,4);
\draw (-0.2,5) -- (0.2,5);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\draw (-0.2,-4) -- (0.2,-4);
\draw (-0.2,-5) -- (0.2,-5);
\node at (6.5,0) {$x$};
\node at (0,6.5) {$y$};
\draw[fill=green] (-3,0) circle (0.1cm);
\draw[fill=green] (0,-4) circle (0.1cm);
\end{tikzpicture}$$

Alla fine basta "collegare" i puntini verdi per trovare il punto richiesto. 

$$\begin{tikzpicture}
\draw[->] (-6,0) -- (6,0);
\draw [->] (0,-6) -- (0,6);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (4,-0.2) -- (4,0.2);
\draw (5,-0.2) -- (5,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-4,-0.2) -- (-4,0.2);
\draw (-5,-0.2) -- (-5,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,4) -- (0.2,4);
\draw (-0.2,5) -- (0.2,5);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\draw (-0.2,-4) -- (0.2,-4);
\draw (-0.2,-5) -- (0.2,-5);
\node at (6.5,0) {$x$};
\node at (0,6.5) {$y$};
\draw[fill=green] (-3,0) circle (0.1cm);
\draw[fill=green] (0,-4) circle (0.1cm);
\draw [dashed] (-3,0) -- (-3,-4);
\draw [dashed] (0,-4) -- (-3,-4);
\draw[fill = red] (-3,-4) circle (0.1cm);
\node[red] at (-3.5,-4.5) {$A(-3;-4)$};
\end{tikzpicture}$$

Analogamente per i punti $$C(-2;-1), E(2;3), F(1;-3)$$:

$$\begin{tikzpicture}
\draw[->] (-6,0) -- (6,0);
\draw [->] (0,-6) -- (0,6);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (4,-0.2) -- (4,0.2);
\draw (5,-0.2) -- (5,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-4,-0.2) -- (-4,0.2);
\draw (-5,-0.2) -- (-5,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,4) -- (0.2,4);
\draw (-0.2,5) -- (0.2,5);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\draw (-0.2,-4) -- (0.2,-4);
\draw (-0.2,-5) -- (0.2,-5);
\node at (6.5,0) {$x$};
\node at (0,6.5) {$y$};
\draw[fill=green] (-3,0) circle (0.1cm);
\draw[fill=green] (0,-4) circle (0.1cm);
\draw[fill=green] (-2,0) circle (0.1cm);
\draw[fill=green] (0,-1) circle (0.1cm);
\draw[fill=green] (2,0) circle (0.1cm);
\draw[fill=green] (0,3) circle (0.1cm);
\draw[fill=green] (1,0) circle (0.1cm);
\draw[fill=green] (0,-3) circle (0.1cm);
\draw [dashed] (-3,0) -- (-3,-4);
\draw [dashed] (0,-4) -- (-3,-4);
\draw [dashed] (-2,0) -- (-2,-1);
\draw [dashed] (0,-1) -- (-2,-1);
\draw [dashed] (1,0) -- (1,-3);
\draw [dashed] (0,-3) -- (1,-3);
\draw [dashed] (2,0) -- (2,3);
\draw [dashed] (0,3) -- (2,3);
\draw[fill = red] (-3,-4) circle (0.1cm);
\node[red] at (-3.5,-4.5) {$A(-3;-4)$};
\draw[fill = red] (-2,-1) circle (0.1cm);
\node[red] at (-2,-1.5) {$C(-2;-1)$};
\draw[fill = red] (1,-3) circle (0.1cm);
\node[red] at (1.5,-3.5) {$F(1;-3)$};
\draw[fill = red] (2,3) circle (0.1cm);
\node[red] at (2.5,3.5) {$E(2;3)$};
\end{tikzpicture}$$

Disegniamo ora invece il punto $$B(-4;0)$$. In questo caso dobbiamo spostarci di quattro unità a sinistra dello zero sull'asse delle $$x$$ in quanto il punto ha $$x = -4$$, e non dobbiamo spostarci in alto o in basso sull'asse delle $$y$$ in quanto il punto ha $$y = 0$$. Ragionamento analogo per il punto $$D(0,5)$$: non ci spostiamo nè a destra nè a sinistra dello zero sull'asse delle $$x$$ in quanto il punto ha $$x = 0$$, ma ci spostiamo verso l'alto di cinque unità sull'asse delle $$y$$ in quanto il punto ha $$y = 5$$. 

$$\begin{tikzpicture}
\draw[->] (-6,0) -- (6,0);
\draw [->] (0,-6) -- (0,6);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (4,-0.2) -- (4,0.2);
\draw (5,-0.2) -- (5,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-4,-0.2) -- (-4,0.2);
\draw (-5,-0.2) -- (-5,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,4) -- (0.2,4);
\draw (-0.2,5) -- (0.2,5);
\draw (-0.2,-1) -- (0.2,-1);
\draw (-0.2,-2) -- (0.2,-2);
\draw (-0.2,-3) -- (0.2,-3);
\draw (-0.2,-4) -- (0.2,-4);
\draw (-0.2,-5) -- (0.2,-5);
\node at (6.5,0) {$x$};
\node at (0,6.5) {$y$};
\draw[fill=green] (-3,0) circle (0.1cm);
\draw[fill=green] (0,-4) circle (0.1cm);
\draw[fill=green] (-2,0) circle (0.1cm);
\draw[fill=green] (0,-1) circle (0.1cm);
\draw[fill=green] (2,0) circle (0.1cm);
\draw[fill=green] (0,3) circle (0.1cm);
\draw[fill=green] (1,0) circle (0.1cm);
\draw[fill=green] (0,-3) circle (0.1cm);
\draw [dashed] (-3,0) -- (-3,-4);
\draw [dashed] (0,-4) -- (-3,-4);
\draw [dashed] (-2,0) -- (-2,-1);
\draw [dashed] (0,-1) -- (-2,-1);
\draw [dashed] (1,0) -- (1,-3);
\draw [dashed] (0,-3) -- (1,-3);
\draw [dashed] (2,0) -- (2,3);
\draw [dashed] (0,3) -- (2,3);
\draw[fill = red] (-3,-4) circle (0.1cm);
\node[red] at (-3.5,-4.5) {$A(-3;-4)$};
\draw[fill = red] (-2,-1) circle (0.1cm);
\node[red] at (-2,-1.5) {$C(-2;-1)$};
\draw[fill = red] (1,-3) circle (0.1cm);
\node[red] at (1.5,-3.5) {$F(1;-3)$};
\draw[fill = red] (2,3) circle (0.1cm);
\node[red] at (2.5,3.5) {$E(2;3)$};
\draw[fill = red] (0,5) circle (0.1cm);
\node[red] at (0.8,5) {$D(0;5)$};
\draw[fill = red] (-4,0) circle (0.1cm);
\node[red] at (-4,0.5) {$B(-4;0)$};
\end{tikzpicture}$$



