# Parabola
<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Determina l'equazione della parabola $$p$$ con asse di simmetria l'asse $$y$$, con il vertice di ordinata $$4$$ e passante per il punto $$A(-2;0)$$. Scrivi poi le equazioni delle rette tangenti alla parabola $$p$$ passanti per il punto $$C(1;4)$$. Detti $$B$$ e $$D$$ i punti di tangenza, riconosci la natura del quadrilatero $$ABCD$$ e calcolane l'area. 

## Soluzione: 

Dal momento che la parabola ha asse di simmetria l'asse $$y$$, stiamo cercando una parabola del tipo 

$$y = ax^2+bx+c, \qquad a \neq 0$$

In più, visto che l'asse di simmetria deve essere l'asse $$y$$ e il vertice di una parabola appartiene a tale asse, sappiamo già che il vertice appartiene all'asse $$y$$ e quindi avrà $$x = 0$$. Ci viene poi detto che la coordinata $$y$$ (ordinata) del vertice è uguale a $$4$$ e che la parabola passa per il punto $$A(-2;0)$$. 
Ricordiamo la formula del vertice:

$$V = \left(-\frac{b}{2a}; - \frac{\Delta}{4a}\right)$$ 

dove $$\Delta = b^2-4ac$$.  Andiamo quindi ad imporre le tre condizioni al fine di trovare $$a,b,c$$ della parabola.

$$\begin{align*}
& \begin{cases}
-\frac{b}{2a} = 0 & \qquad \text{asse y come asse di simmetria}\\
 -\frac{b^2-4ac}{4a}  = 4 & \qquad \text{ordinata uguale a 4}\\
0  = a(-2)^2+b(-2)+c & \qquad \text{il punto A appartiene alla parabola}
\end{cases} \\
& \begin{cases}
-b = 0 \\
 -(b^2-4ac)= 4\cdot 4a & \\
0  = 4a-2b+c & 
\end{cases}\\
& \begin{cases}
b = 0 \\
 -(0^2-4ac)= 4\cdot 4a & \\
0  = 4a-2\cdot 0 +c & 
\end{cases}\\
& \begin{cases}
b = 0 \\
 4ac - 16a = 0 & \\
0  = 4a +c & 
\end{cases}\\
& \begin{cases}
b = 0 \\
 4a(-4a) - 16a = 0 & \\
c = - 4a & 
\end{cases}\\
& \begin{cases}
b = 0 \\
 -16a^2 - 16a = 0 & \\
c = - 4a & 
\end{cases}\\
& \begin{cases}
b = 0 \\
-16a(a+1) = 0 \rightarrow -16a = 0 \vee a +1 = 0\\
c = - 4a & 
\end{cases}
\end{align*}$$

Ho quindi trovato due soluzioni per $$a$$: o $$a = 0$$, che però escludo subito perchè in quel caso non avrei una parabola, o $$a = -1$$. 

$$\begin{align*}
\begin{cases}
b = 0 \\
a = -1 \\
c = - 4a = -4(-1) = 4
\end{cases}
\end{align*}$$

La parabola cercata ha quindi equazione 

$$y = ax^2+bx +c = (-1)x^2+(0)x+(4) = -x^2+4$$ 

Dobbiamo ora trovare le equazioni delle rette tangenti a $$p$$ passanti per il punto $$C(1;4)$$. 

$$\begin{tikzpicture}
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-3, xmax=3,
	ymin=-2, ymax=5,
	restrict y to domain=-2:5,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\addplot[red, mark=*, only marks] coordinates {(1,4) (0,4)};
\addplot[] coordinates {(1,-0.5)} node{\small $1$};
\addplot[] coordinates {(2,-0.5)} node{\small $2$};
\addplot[] coordinates {(-1,-0.5)} node{\small $-1$};
\addplot[] coordinates {(-2,-0.5)} node{\small $-2$};
\addplot[red] coordinates {(1.3,4.2)} node{\small $C$};
\addplot[red] coordinates {(-0.2,4.3)} node{\small $V$};
\addplot[red,domain=-2.7:2.7,semithick]{-x^2+4};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

Facendo il disegno notiamo subito che, dal momento che il punto $$C$$ e il vertice $$V$$ della parabola hanno la stessa ordinata, una retta tangente sarà la retta orizzontale $$y = 4$$. Procediamo comunque con il metodo "classico" per trovare la tangenti a una parabola passanti per un punto esterno. 

Scrivo tutte le rette passanti per il punto $$C(1;4)$$:

$$y - y_0 = m (x-x_0) $$

$$y - 4 = m (x-1)$$ 

Metto a sistema questo fascio di rette con la mia parabola: 

$$\begin{align*}
\begin{cases}
y-4 = m(x-1) \\
y = -x^2+4
\end{cases}\\
\begin{cases}
y = mx-m +4 \\
y = -x^2+4
\end{cases}
\end{align*}$$

Ottengo quindi 

$$\begin{align*}
mx-m+4 & = -x^2+4 \\
x^2+mx-m & = 0 
\end{align*}$$

Calcolo il delta e lo pongo uguale a zero per la condizione di tangenza:

$$\begin{align*}
\Delta & = (m)^2-4(1)(-m) \\
& = m^2+4m \\
\Delta & = 0  \rightarrow m^2+4m = 0 \\
& \qquad \; \; \; \; m(m+4)  = 0 
\end{align*}$$

Quindi o $$m = 0$$ oppure $$m = -4$$. 

Se $$m = 0$$: otteniamo la tangente che ci aspettavamo

$$\begin{align*}
y-4 & = m(x-1) \\
y-4 & = 0(x-1) \\
y-4 & = 0 \\
y & = 4 
\end{align*}$$

Se $$m = -4$$: 

$$\begin{align*}
y-4 & = m(x-1) \\
y-4 & = -4(x-1) \\
y-4 & = -4x+4 \\
y & = -4x+8 
\end{align*}$$

Per trovare i punti di tangenza, torniamo all'equazione di secondo grado in $$x$$ e sostituiamo gli $$m$$ che abbiamo trovato.

$$\begin{align*}
x^2+mx-m & = 0 \\
x^2-4x+4 & = 0  \\
(x-2)^2 & = 0 \\
x & = 2 \\
y & = -x^2+4 = -(2)^2+4 = 0
\end{align*}$$

$$\begin{align*}
x^2+mx-m & = 0 \\
x^2+(0)x+0 & = 0  \\
x^2 & = 0 \\
x & = 0 \\
y & = -x^2+4 = -(0)^2+4 = 4
\end{align*}$$

I due punti di tangenza sono quindi $$(2;0)$$ e $$(0,4)$$. Disegniamo ciò che abbiamo trovato finora. 

$$\begin{tikzpicture}
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-3, xmax=3,
	ymin=-2, ymax=5,
	restrict y to domain=-2:5,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\addplot[red, mark=*, only marks] coordinates {(1,4) (0,4) (2,0) (-2,0)};
\addplot[] coordinates {(1,-0.5)} node{\small $1$};
\addplot[] coordinates {(2,-0.5)} node{\small $2$};
\addplot[] coordinates {(-1,-0.5)} node{\small $-1$};
\addplot[] coordinates {(-2,-0.5)} node{\small $-2$};
\addplot[red] coordinates {(1.3,4.2)} node{\small $C$};
\addplot[red] coordinates {(-0.2,4.3)} node{\small $B$};
\addplot[red] coordinates {(2.2,0.5)} node{\small $D$};
\addplot[red] coordinates {(-2.2,0.5)} node{\small $A$};
\addplot[red,domain=-2.7:2.7,semithick]{-x^2+4};
\addplot[red,domain=-2.7:2.7,semithick, dashed]{4};
\addplot[red,domain=-2.7:2.7,semithick, dashed]{-4*x+8};
\draw[green, thick] (axis cs:-2,0) -- (axis cs:0,4);
\draw[green, thick] (axis cs:0,4) -- (axis cs:1,4);
\draw[green, thick] (axis cs:1,4) -- (axis cs:2,0);
\draw[green, thick] (axis cs:2,0) -- (axis cs:-2,0);
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

Graficamente capiamo subito che il quadrilatero $$ABCD$$ è un trapezio: per dimostrarlo analiticamente dobbiamo dimostrare che due lati non consecutivi sono paralleli. Consideriamo le rette $$AD$$ e $$BC$$: poichè sono rette orizzontali, la loro equazione è della forma $$y = k$$ con $$k$$ numero. 

Equazione della retta $$AD$$: $$y = 0$$.

Equazione della retta $$BC$$: $$y = 4$$.

Le due rette sono quindi parallele perchè entrambe hanno coefficiente angolare pari a zero. 

Ricordiamo come si calcolare l'area di un trapezio:

$$\begin{align*}
A & = \frac{(B+b)h}{2} \\
& = \frac{(AD+BC)BO}{2}
\end{align*}$$

dove $$O$$ è l'origine degli assi cartesiani. Andiamo a calcolare le lunghezze.

$$AD = |x_D-x_A| = |2-(-2)| = |4| = 4$$

$$BC = |x_C-x_B| = |1-0| = |1| = 1$$

$$BO = |y_B-y_O| = |4-0| = |4| = 4$$

L'area è quindi pari a 

$$\begin{align*}
A & = \frac{(AD+BC)BO}{2} \\
& = \frac{(4+1)\cdot4}{2} \\
& = 10
\end{align*}$$



