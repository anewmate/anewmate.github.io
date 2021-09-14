# ELLISSE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Data l'equazione dell'ellisse determina la misura dei semiassi, le coordinate dei vertici e dei fuochi, l'eccentricità e reppresenta la curva graficamente. 

$$x^2+9y^2 = 36$$

Soluzione: 

Come prima cosa riscrivo l'equazione in forma canonica, ossia del tipo $$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$$: per fare ciò, devo dividere destra e sinistra per $$36$$.

$$\begin{align*}
x^2+9y^2 & = 36 \\
\frac{1}{36} \cdot (x^2+9y^2) & = 36 \cdot \frac{1}{36} \\
\frac{x^2}{36} + \frac{y^2}{4} & = 1
\end{align*}
$$

Avendola scritta in forma canonica ho subito che 

$$\begin{align*}
a^2 = 36  & \rightarrow  a = 6 \; \; \text{(semiasse maggiore)} \\
b^2 = 4 & \rightarrow b = 2 \; \; \text{(semiasse minore)} 
\end{align*}
$$

Dato che $$a > b$$, l'ellisse ha i fuochi sull'asse $$x$$. 

Le coordinate dei vertici diventano quindi 

$$\begin{align*}
A(-a,0)  & \rightarrow  A(-6,0)  \\
B(a,0)  & \rightarrow B(6,0) \\
C(0,-b) & \rightarrow C(0,-2) \\
D(0,b) & \rightarrow D(0,2) 
\end{align*}
$$

Per calcolare i fuochi e l'eccentricità ho bisogno di sapere $$c$$, che posso trovare tramite la formula $$c^2 = a^2-b^2$$:

$$ c = \sqrt{36-4} = \sqrt{32} = \sqrt{2^4\cdot 2} = \sqrt {2^4} \cdot \sqrt{2} = 2^2 \cdot \sqrt{2} = 4\sqrt{2}$$

Le coordinate dei fuochi sono quindi 

$$\begin{align*}
F_1(-c,0)  & \rightarrow  F_1(-4\sqrt{2},0)  \\
F_2(c,0)  & \rightarrow F_2(4\sqrt{2},0) \\
\end{align*}
$$

e l'eccentricità 

$$e = \frac{c}{a} = \frac{4\sqrt{2}}{6} = \frac{2\sqrt{2}}{3}$$

Conoscendo la misura dei semiassi, possiamo rappresentarla graficamente:

$$\begin{tikzpicture}[scale=1.02]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-7, xmax=7,
	ymin=-3, ymax=3,
	restrict y to domain=-3:3,
	%ytick={3},
	%xtick={-1,1},
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\addplot[red,domain=-6:6,semithick]{(((1/9)*(36-(x^2)))^(1/2))};
\addplot[red,domain=-6:6,semithick]{-(((1/9)*(36-(x^2)))^(1/2))};
%\addplot[green,domain=-5:4,semithick]{(x+4)/2};
%\shade [shading=ellipse] (0,0) ellipse [x radius=2cm,y radius=1cm];
%\addplot[black]{x+1};
%\addplot[] coordinates {(1,1.5)} node{$y=x+1$};
%\draw (axis cs:0,3) circle [black, radius=1];
\addplot[black,mark=*] coordinates {(-6,0)};
\addplot[black,mark=*] coordinates {(6,0)};
\addplot[black,mark=*] coordinates {(0,2)};
\addplot[black,mark=*] coordinates {(0,-2)};
\addplot[red] coordinates {(-6.3,0.5)} node{$A$};
\addplot[red] coordinates {(6.3,0.5)} node{$B$};
\addplot[red] coordinates {(0.4,-2.5)} node{$C$};
\addplot[red] coordinates {(0.4,2.5)} node{$D$};
%\addplot[green] coordinates {(2,2.4)} node{$y=\frac{x+4}{2}$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$ 








