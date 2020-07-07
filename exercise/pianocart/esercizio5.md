# PIANO CARTESIANO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 5:

> Individua il punto $$P$$ che ha ordinata uguale all'ascissa ed è equidistante da $$A(-2;2)$$ e $$B(5;4)$$. 

## Soluzione: 

Come prima cosa ricordo che con ordinate si intende le $$y$$ e con ascisse le $$x$$. Dire che un punto ha ordinata uguale all'ascissa significa che il punto deve avere coordinata $$x$$ uguale alla coordinata $$y$$. In altre parole, se chiamo $$t$$ la coordinata $$x$$ del punto (che deve essere uguale alla coordinata $$y$$), il punto sarà del tipo $$P(t;t)$$.

Devo poi richiedere che la distanza fra questo punto $$P(t;t)$$ e i punti $$A$$ e $$B$$ sia uguale. Ricordo che la distanza fra due punti $$A(x_A;y_A)$$ e $$B(x_B;y_B)$$ è data da 

$$\overline{AB} = \sqrt{(x_B-x_A)^2+(y_B-y_A)^2}$$

Nel nostro caso quindi 

$$\begin{align*}
\overline{PA} & = \sqrt{(-2-t)^2+(2-t)^2} \\
\overline{PB} & = \sqrt{(5-t)^2+(4-t)^2}
\end{align*}$$

Imponendo $$\overline{PA} = \overline{PB}$$, otteniamo 

$$\begin{align*}
\sqrt{(-2-t)^2+(2-t)^2} & = \sqrt{(5-t)^2+(4-t)^2} \\
& \downarrow \\
\text{elevo al} & \; \text{quadrato:} \\
(-2-t)^2+(2-t)^2 & = (5-t)^2+(4-t)^2 \\
4+t^2+4t+4+t^2-4t & = 25+t^2-10t+16+t^2-8t \\
8+2t^2 & = 41 +2t^2-18t \\
18t & = 41-8 \\
18t & = 33 \\
\frac{18t}{18} & = \frac{33}{18} \\
t & = \frac{33}{18}
\end{align*}$$

**Memo**: $$(A\pm B)^2 = A^2 \pm 2AB + B^2$$. 

Il punto $$P$$ che stavamo cercando ha quindi coordinate $$P\left(\frac{33}{18}; \frac{33}{18}\right)$$.

$$\begin{tikzpicture}
\draw[->] (-3,0) -- (6,0);
\draw [->] (0,-1) -- (0,5);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (4,-0.2) -- (4,0.2);
\draw (5,-0.2) -- (5,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,4) -- (0.2,4);
\node at (6.5,0) {$x$};
\node at (0,5.5) {$y$};
\draw[fill=red] (-2,2) circle (0.07cm);
\draw[fill=red] (5,4) circle (0.07cm);
\draw[fill=red] (33/18,33/18) circle (0.07cm);
\node[red] at (-2,2.5) {$A$};
\node[red] at (5,4.5) {$B$};
\node[red] at (33/18,33/18-0.5) {$P$};
\draw (-2,2) -- (5,4);
\draw (-2,2) -- (33/18,33/18);
\draw (5,4) -- (33/18,33/18);
\node[blue, ultra thick] at (0.5,1.9) {$\Huge \mathbb{\times}$};
\node[blue, ultra thick] at (3,2.63) {$\Huge \mathbb{\times}$};
\end{tikzpicture}$$
