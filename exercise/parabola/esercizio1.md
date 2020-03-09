# PARABOLA

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Disegna la parabola con la seguente equazione

$$y = -3x^2+3$$

## Soluzione: 

Come prima cosa notiamo che la parabola ha asse parallelo all'asse $$y$$ poichè è scritta in forma 

$$y = ax^2+bx+c$$

dove, nel nostro caso, $$a=-3,b=0,c=+3$$.

Per disegnare la parabola abbiamo bisogno di trovare il vertice e l'intersezione con gli assi cartesiani. 

Per il vertice ricordiamo la formula: $$V=\left(-\frac{b}{2a};-\frac{\Delta}{4a}\right)$$

dove $$\Delta = b^2-4ac$$.

$$\begin{align*}
x_V = -\frac{b}{2a} & = -\frac{0}{2(-3)} = 0 \\
y_V = -\frac{\Delta}{4a} & = -\frac{b^2-4ac}{4a} = -\frac{0^2-4(-3)(+3)}{4(-3)} = +3
\end{align*}$$

Modo alternativo per trovare il vertice: visto che il vertice è un punto della parabola, le sue coordinate soddisfano l'equazione della parabola. Quindi, una volta che ho trovato la $$x_V$$ del vertice, posso sostituire questa nell'equazione della parabola per trovare la $$y_V$$. Per esempio, nel nostro caso, una volta che troviamo $$x_V=0$$, sostituisco questo valore di $$x$$ nell'equazione $$y = -3x^2+3$$ trovando

$$y_V = -3(0)^2 + 3 = +3$$

Passiamo ora all'intersezione con l'asse $$x$$. Quest'asse ha equazione $$y = 0$$, quindi, poichè intersecare significa mettere a sistema, devo risolvere 

$$\begin{align*}
\begin{cases}
y = 0 \\
y = -3x^2+3
\end{cases} \rightarrow -3x^2+3 = 0
\end{align*}$$

Portando $$x$$ a sinistra e tutto il resto a destra ottengo 

$$-3x^3 = -3$$

Divido destra e sinistra per $$-3$$ per isolare la $$x$$

$$x^2 = +1$$

e ottengo come soluzioni $$x = \pm 1$$.

Le intersezioni con l'asse $$x$$ sono quindi $$(1;0),(-1;0)$$.

***
Memo: Le equazioni del tipo $$x^2 = K$$ con $$K\geq 0$$, hanno direttamente soluzione 

$$x = \pm \sqrt{K}$$

Se $$K < 0$$, l'equazione è invece impossibile ($$\nexists x \in \mathbb{R}$$). Infatti, un quadrato è sempre positivo (ossia a sinistra dell'uguale ho qualcosa di maggiore di zero). Mi sto quindi chiedendo quando un numero positivo ($$x^2$$,a sinistra dell'uguale) è uguale a un numero negativo ($$K$$, a destra dell'uguale), e la risposta è chiaramente mai. 
***

Andiamo ora a vedere le intersezione con l'asse $$y$$. Quest'asse ha equazione $$x=0$$, quindi devo risolvere il sistema

$$\begin{align*}
\begin{cases}
x = 0 \\
y = -3x^2+3
\end{cases} \rightarrow y = +3
\end{align*}$$

L'intersezione con l'asse $$y$$ è quindi $$(0,3)$$.

Possiamo ora disegnare la parabola.

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-1.5, xmax=1.5,
	ymin=-1, ymax=4,
	restrict y to domain=-1:3.5,
	ytick={3},
	xtick={-1,1},
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\addplot[red,domain=-2:2,semithick]{-3*(x^2)+3};
%\addplot[black]{x+1};
%\addplot[] coordinates {(1,1.5)} node{$y=x+1$};
%\draw (axis cs:0,3) circle [black, radius=1];
\addplot[black,mark=*] coordinates {(0,3)};
\addplot[black,mark=*] coordinates {(-1,0)};
\addplot[black,mark=*] coordinates {(1,0)};
\addplot[black] coordinates {(0.2,3.2)} node{$V$};
\addplot[red] coordinates {(-2,0.6)} node{$y=-3x^2+3$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

Sostianzialmente devo disegnare i punti trovati e poi collegare i punti.



