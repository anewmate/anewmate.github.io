# INTEGRALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 5:

> Trova il volume del solido generato dalla rotazione completa attorno all'asse $$x$$ del trapezoide individuato dal grafico della funzione $$y =  \sqrt{\frac{x+4}{x}}$$ nell'intervallo $$[-5,-4]$$.

## Soluzione:

Come prima cosa facciamo un piccolo grafico della funzione nell'intervallo considerato: non è richiesto dal problema, ma preferisco sempre avere anche un'idea visiva di quello che sto facendo. 

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=1200,
	width=9.0cm,height=6.4cm,
	xmin=-8, xmax=2,
	ymin=-0.5, ymax=5,
	restrict y to domain=-0.5:5,
	ytick=none,
	xtick={-5,-4},
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\addplot[red,domain=-7:1.5,semithick]{sqrt((x+4)/x)};
\addplot[red] coordinates {(-2,2.5)} node{$\sqrt{\frac{x+4}{x}}$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

Facendo quindi ruotare il grafico della funzione in $$[-5,-4]$$ attorno all'asse $$x$$ di 360 gradi ottengo

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=1200,
	width=9.0cm,height=6.4cm,
	xmin=-6, xmax=-2,
	ymin=-0.5, ymax=5,
	restrict y to domain=-0.5:5,
	ytick=none,
	xtick={-4},
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\addplot[black,dashed] coordinates {
(-5,-0.4472135955)
(-5,0.4472135955)
};
\addplot[red,domain=-5:-4,semithick]{sqrt((x+4)/x)};
\addplot[red,domain=-5:-4,semithick]{-sqrt((x+4)/x)};
\draw[red] (100,50) ellipse (0.15cm and 0.40cm);
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

Voglio il volume di questo solido. La formula che devo utilizzare è

$$V = \pi \int_a^b f^2(x)dx$$

dove, nel nostro caso, $$a=-5,b=-4,f(x) = \sqrt{\frac{x+4}{x}}$$. 

Quindi 

$$\begin{align*}
V & = \pi \int_{-5}^{-4} \left(\sqrt{\frac{x+4}{x}}\right)^2 dx \\
& = \pi \int_{-5}^{-4} \frac{x+4}{x} dx \\
& = \pi \int_{-5}^{-4} \left( 1 + \frac{4}{x} \right)dx \\
& = \pi \left( \int_{-5}^{-4}dx + 4 \int_{-5}^{-4} \frac{1}{x}dx \right) \\
& = \pi \left( x \biggl|_{-5}^{-4} + 4 \cdot \ln(|x|) \biggl|_{-5}^{-4} \right) \\
& = \pi \left( (-4-(-5)) + 4 \cdot (\ln(|-4|)-(\ln(|-5|)))\right) \\
& = \pi \left( 1 + 4 \cdot (\ln(4)-\ln(5))\right) \\
& = \pi \left( 1 + 4 \cdot \ln\left(\frac{4}{5}\right) \right)
\end{align*}$$






