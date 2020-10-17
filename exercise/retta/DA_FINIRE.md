# RETTA

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> I punti $$A(-2;4)$$ e $$B(0;1)$$ sono due vertici del parallelgramma $$ABCD$$ e il punto $$M\left(2;\frac{9}{2}\right)$$ è il punto di intersezione delle diagonali. 

> a) Determina le coordinate dei vertici $$C$$ e $$D$$ del parallelogramma.

> b) Verifica che il parallelogramma è un rettangolo.

> c) Calcolane il perimetro e l'area. 
## Soluzione: 

Come prima cosa disegno i dati del problema. 

$$\begin{tikzpicture}
\draw[->] (-3,0) -- (7,0);
\draw [->] (0,-1) -- (0,9);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (4,-0.2) -- (4,0.2);
\draw (5,-0.2) -- (5,0.2);
\draw (6,-0.2) -- (6,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,4) -- (0.2,4);
\draw (-0.2,5) -- (0.2,5);
\draw (-0.2,6) -- (0.2,6);
\draw (-0.2,7) -- (0.2,7);
\draw (-0.2,8) -- (0.2,8);
\node at (7.5,0) {$x$};
\node at (0,9.5) {$y$};
\draw[fill=red] (-2,4) circle (0.07cm);
\draw[fill=red] (0,1) circle (0.07cm);
\draw[fill=red] (2,9/2) circle (0.07cm);
\node[red] at (-2,4.5) {$A$};
\node[red] at (0.3,0.7) {$B$};
\node[red] at (2.2,4) {$M$};
\draw (-2,4) -- (0,1);
\draw (0,1) -- (4.5,7*4.5/4+1);
\draw (-2,4) -- (6.5,6.5/8+17/4);
\end{tikzpicture}$$

**Memo:** in un parallelogramma, il punto di incontro delle diagonali divide ogni diagonale a metà.

Nel nostro caso quindi abbiamo che $$M$$ è il punto medio sia del segmento $$AC$$ che del segmento $$BD$$.

Il punto $$C$$ sarà quindi quel punto che appartiene alla retta $$AM$$ e tale che $$AM = MC$$.

Partiamo quindi calcolando l'equazione della retta $$AM$$. Ricordo che, dati due punti $$P_1$$ e $$P_2$$, l'equazione della retta che passa per quei punti è data da 

$$\frac{y-y_2}{y_1-y_2} = \frac{x-x_2}{x_1-x_2}$$ 

Quindi, 

$$\begin{align*}
\frac{y-\frac{9}{2}}{4-\frac{9}{2}} & = \frac{x-2}{-2-2} \\
\frac{y-\frac{9}{2}}{-\frac{1}{2}} & = \frac{x-2}{-4} \\
-2\left(y-\frac{9}{2}\right) & = \frac{x-2}{-4} \\
y - \frac{9}{2} & = \frac{x-2}{8} \\
y & = \frac{x}{8} - \frac{2}{8} + \frac{9}{2} \\
y & = \frac{x}{8} + \frac{17}{4}
\end{align*}$$

Poichè il punto $$C$$ deve appartenere a questa retta, esso avrà coordinate 

$$C\left(x; \frac{x}{8} + \frac{17}{4}\right)$$

Devo ora imporre la condizione $$AM = MC$$: per farlo, devo ricordarmi la formula per calcolare la distanza fra due punti, che scriviamo qui sotto. 

$$P_1P_2 = \sqrt{(x_1-x_2)^2+(y_1-y_2)^2}$$

Nel nostro caso,

$$AM = \sqrt{(2-(-2))^2+\left(\frac{9}{2}-4\right)^2} = \sqrt{16 + \frac{1}{4}} = \sqrt{\frac{65}{4}}$$

$$MC = \sqrt{(x-2)^2+\left(\frac{x}{8}+\frac{17}{4}-\frac{9}{2}\right)^2} = \sqrt{(x-2)^2+\left(\frac{x}{8}-\frac{1}{4}\right)^2}$$

Andando ad imporre $$AM = MC$$ mi sto sostanzialmente chiedendo quali sono i punti appartenenti alla retta $$y = \frac{x}{8}+\frac{17}{4}$$ equidistanti da $$M$$: mi posso quindi aspettare di ritrovare il punto $$A$$ e di trovare il punto $$C$$.

$$\begin{align*}
\sqrt{(x-2)^2+\left(\frac{x}{8}-\frac{1}{4}\right)^2} & = \sqrt{\frac{65}{4}}
\end{align*}$$