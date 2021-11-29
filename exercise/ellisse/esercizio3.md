# ELLISSE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Scrivi le equazioni delle tangenti all'ellisse di equazione $$x^2+2y^2 = 9$$ condotte dal punto $$P\left(3;\frac{3}{2}\right)$$. 

Soluzione: 

Come prima cosa scrivo tutte le rette che passano per il punto $$P$$. Ricordo che il fascio di tutte le rette che passano per un generico punto $$(x_0;y_0)$$ è dato da 

$$(y-y_0) = m (x-x_0)$$

Nel nostro caso $$x_0 = 3$$ e $$y_0 = \frac{3}{2}$$. Tutte le rette che passano per $$P$$ hanno quindi equazione 

$$y - \frac{3}{2} = m (x-3)$$

Per trovare le rette tangenti devo quindi trovare quell'$$m$$ che mi garantisce la condizione di tangenza. Come si fa? 

Intanto interseco tutte queste rette con l'ellisse: 

$$\begin{align*}
& \begin{cases}
y - \frac{3}{2} = m (x-3) \\
x^2+2y^2=9
\end{cases} \\
& \begin{cases}
y = mx - 3m + \frac{3}{2} \\
x^2+2y^2=9
\end{cases} \\
& \begin{cases}
y = mx-3m+\frac{3}{2} \\
x^2+2\left(mx-3m+\frac{3}{2}\right)^2=9
\end{cases}
\end{align*}
$$

Sistemo solo la seconda equazione:

$$\begin{align*}
x^2+2\left(mx-3m+\frac{3}{2}\right)^2& =9 \\
x^2 +2\left(m^2x^2-3m^2x+\frac{3}{2}mx-3m^2x+9m^2-\frac{9}{2}m+\frac{3}{2}mx-\frac{9}{2}m+\frac{9}{4}\right)& = 9 \\
x^2+2\left(m^2x^2-6m^2x+3mx-9m+9m^2+\frac{9}{4}\right) & = 9 \\
x^2 +2m^2x^2-12m^2x+6mx-18m+18m^2+\frac{9}{2}& = 9 
\end{align*}
$$

Mi fermo un attimo perchè di solito a questo punto non si sa più cosa si sta facendo. Qual è la variabile di quell'equazione? 

Quella scritta sopra è un'equazione di secondo grado in $${x}$$. Non ci dobbiamo far trarre in inganno per il fatto che c'è $$m$$: $$m$$ è soltanto un parametro, ossia un numero e come tale lo dobbiamo pensare. 

Vado quindi a raccogliere i termini in $$x$$:

$$\begin{align*}
x^2 +2m^2x^2-12m^2x+6mx-18m+18m^2+\frac{9}{2}& = 9 \\
x^2 \cdot \underbrace{(1+2m^2)}_{a} + x \cdot \underbrace{(-12m^2+6m)}_{b}  -\underbrace{18m+18m^2+\frac{9}{2} - 9}_{c} & = 0 
\end{align*}
$$

Avevamo detto che volevamo l'$$m$$ che ci garantisse la tangenza. Ciò si ottiene ponendo il $$\Delta$$ di questa equazione di secondo grado uguale a zero. 

$$\begin{align*}
\Delta & = b^2 - 4ac \\
& = (-12m^2+6m)^2 - 4 (1+2m^2)\left(-18m+18m^2-\frac{9}{2}\right) \\
& = 144m^4+36m^2-144m^3-4\left(-18m+18m^2-\frac{9}{2}-36m^3+36m^4-9m^2\right)\\
& = 144m^4+36m^2-144m^3+72m-72m^2+18+144m^3-144m^4+36m^2 \\
& = 72m+18 
\end{align*}
$$

Ponendo $$\Delta = 0$$ si ottiene un'equazione in $$m$$ (e qui $$m$$ è proprio la variabile che vogliamo trovare). 

$$\begin{align*}
\Delta & = 0 \\
72m+18 & = 0 \\
72m & = -18 \\
\frac{72m}{72} & = \frac{-18}{72} \\
m & = -\frac{1}{4}
\end{align*}
$$

Una retta di tangenza l'abbiamo quindi trovata: metto l'$$m$$ che ho appena trovato nel fascio e ho la retta. 

$$\begin{align*}
y - \frac{3}{2} & = m (x-3) \\
y - \frac{3}{2} & =-\frac{1}{4}(x-3) \\
y & = -\frac{1}{4}x + \frac{3}{4} + \frac{3}{2} \\
y & = -\frac{1}{4}x + \frac{3+6}{4} \\
y & = -\frac{1}{4}x + \frac{9}{4} 
\end{align*}
$$

Perchè ho trovato solo una retta di tangenza e non due? 

Calcolando tutte le rette che passano per $$P$$, gli unici $$m$$ che non riesco a trovare sono quelli delle rette verticali (ricordo che nelle rette verticali non si può definire $$m$$). 

Grafico quello che ho trovato fino ad adesso. 

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
\addplot[red,domain=-4:4,semithick]{(((1/2)*(9-(x^2)))^(1/2))};
\addplot[red,domain=-4:4,semithick]{-(((1/2)*(9-(x^2)))^(1/2))};
\addplot[green,domain=-4:4,semithick]{-1/4*x+9/4};
\addplot +[green,mark=none] coordinates {(3, -2.5) (3, 3)};
%\addplot[green,domain=-5:4,semithick]{(x+4)/2};
%\shade [shading=ellipse] (0,0) ellipse [x radius=2cm,y radius=1cm];
%\addplot[black]{x+1};
%\addplot[] coordinates {(1,1.5)} node{$y=x+1$};
%\draw (axis cs:0,3) circle [black, radius=1];
\addplot[black,mark=*] coordinates {(-3,0)};
\addplot[black,mark=*] coordinates {(3,0)};
\addplot[black,mark=*] coordinates {(0,2.12132034356)};
\addplot[black,mark=*] coordinates {(0,-2.12132034356)};
\addplot[black,mark=*] coordinates {(3,3/2)};
\addplot[red] coordinates {(3.4,3/2)} node{$P$};
%\addplot[green] coordinates {(2,2.4)} node{$y=\frac{x+4}{2}$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$ 

Visto che il punto $$P$$ è esterno all'ellisse, mi rendo subito conto che la seconda retta di tangenza ha equazione

$$x = 3$$

ossia $$x = x_P$$, dove $$x_P$$ è la coordinata $$x$$ del punto $$P$$. 

Le due rette tangenti hanno quindi equazione $$x = 3$$ e $$y & = -\frac{1}{4}x + \frac{9}{4}$$. 










