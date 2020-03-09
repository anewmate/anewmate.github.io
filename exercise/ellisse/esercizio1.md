# ELLISSE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Data l'ellisse di equazione $$x^2+4y^2 = 16$$, trova la lunghezza della corda individuata sulla retta di equazione $$x-2y+4=0$$.

## Soluzione: 

Come prima cosa riscriviamo l'equazione dell'ellisse dividendo tutto per $$16$$:

$$\frac{x^2}{16} + \frac{y^2}{4} = 1$$

Giusto per farci un'idea, facciamo un disegno: non è richiesto dall'esercizio, ma visualizzare fa sempre bene.

Ricordiamo l'equazione generale dell'ellisse:

$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$$

Per disegnarla mi servono soltanto $$a$$ e $$b$$. Nel nostro caso, $$a = \sqrt{16} = 4$$ e $$b = \sqrt{4} = 2$$. 

Per disegnare invece la retta, basta che trovo due suoi punti: con $$x=0$$ ottengo $$0-2y+4=0 \rightarrow y = 2$$ quindi il punto $$(0;2)$$, mentre con $$x=2$$ ottengo $$2-2y+4=0 \rightarrow y = 3$$ quindi il punto $$(2;3)$$. 

$$\begin{tikzpicture}[scale=1.02]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-4, xmax=4,
	ymin=-3, ymax=3,
	restrict y to domain=-3:3,
	%ytick={3},
	%xtick={-1,1},
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\addplot[red,domain=-4:4,semithick]{(1/2)*((16-(x^2))^(1/2))};
\addplot[red,domain=-4:4,semithick]{-(1/2)*((16-(x^2))^(1/2))};
\addplot[green,domain=-5:4,semithick]{(x+4)/2};
%\shade [shading=ellipse] (0,0) ellipse [x radius=2cm,y radius=1cm];
%\addplot[black]{x+1};
%\addplot[] coordinates {(1,1.5)} node{$y=x+1$};
%\draw (axis cs:0,3) circle [black, radius=1];
\addplot[black,mark=*] coordinates {(-4,0)};
\addplot[black,mark=*] coordinates {(4,0)};
\addplot[black,mark=*] coordinates {(0,2)};
\addplot[black,mark=*] coordinates {(0,-2)};
\addplot[red] coordinates {(2,-2.3)} node{$\frac{x^2}{16} + \frac{y^2}{4} = 1$};
\addplot[green] coordinates {(2,2.4)} node{$y=\frac{x+4}{2}$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$ 

Per trovare la lunghezza della corda individuata sulla retta, dobbiamo trovare i punti di intersezione fra la retta e l'ellisse e poi calcolare la distanza fra questi punti. Facendo il grafico i punti di intersezione sono chiari, ma andiamo a calcolarli come ci richiede l'esercizio. 

Dobbiamo mettere a sistema l'ellisse con la retta:

$$\begin{align*}
\begin{cases}
x^2+4y^2 = 16 \\
y = \frac{x+4}{2}
\end{cases}
\end{align*}$$

Sostituisco $$y$$ nell'equazione dell'ellisse e ottengo 

$$x^2 + 4 \left(\frac{x+4}{2}\right)^2 = 16$$

Svolgo i conti:

$$\begin{align*}
x^2+4 \cdot \frac{(x+4)^2}{4} & = 16 \\
x^2 + x^2+16+8x & = 16 \\
2x^2 + 8x +16 - 16 & = 0 \\
2x(x+4) & = 0 \\
\frac{2x(x+4)}{2} & = \frac{0}{2} \\
x(x+4) & = 0 
\end{align*}$$

Quindi, per la legge dell'annullamento del prodotto (un prodotto è zero se e solo se uno dei due termini è zero), ho che le soluzioni sono

$$x = 0 \qquad \vee \qquad x+4=0 \rightarrow x = -4$$

Con $$x=0$$ ottengo $$y = \frac{0+4}{2} = 2$$, ossia il punto $$(0;2)$$ che chiamo A.

Con $$x=-4$$ ottengo $$y = \frac{-4+4}{2} = 0$$, ossia il punto $$(-4;0)$$ che chiamo B.

Devo ora calcolare la distanza fra questi due punti. Ricordo che la distanza fra due punti $$A(x_A;y_A)$$ e $$B(x_B;y_B)$$ è calcolata come 

$$d = \sqrt{(x_B-x_A)^2 + (y_B-y_A)^2}$$

Nel nostro caso,

$$\begin{align*}
d & = \sqrt{(-4-0)^2+(0-2)^2} \\
& = \sqrt{16+4} \\
& = \sqrt{20} \\
& = \sqrt{4\cdot 5} \\
& = \sqrt{4} \cdot \sqrt{5} \\
& = 2\sqrt{5}
\end{align*}$$


