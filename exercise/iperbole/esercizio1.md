# IPERBOLE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Data l'equazione 

$$y=\frac{3ax+b}{x-c}$$

> determina $$a,c,b \in \mathbb{R}$$ tali che $$x=2$$ e $$y=6$$ rappresentino due asintoti per la funzione che passa per il punto $$A(3;14)$$. Disegna la curva così ottenuta. 

## Soluzione:

Come prima cosa notiamo che siamo di fronte a una funzione omografica, ossia un'iperbole equilatera traslata. In generale ha equazione 

$$y = \frac{Ax+B}{Cx+D}$$ 

con $$C \neq 0$$ e $$AD-BC \neq 0$$. Gli asintoti sono dati da 

$$x = -\frac{D}{C}, y = \frac{A}{C}$$

e il centro di simmetria ha coordinate $$C\left(-\frac{D}{C};\frac{A}{C}\right)$$.

Andiamo quindi a imporre le condizioni sugli asintoti nel nostro caso. Dato che vogliamo $$x=2$$ come asintoto devo avere 

$$-\frac{-c}{1} = 2$$

ossia $$c = 2$$.

Inoltre voglio $$y = 6$$ quindi 

$$\frac{3a}{1} = 6$$

ossia $$a = \frac{6}{3} = 2$$.

La nostra funzione per ora è data da 

$$y=\frac{6x+b}{x-2}$$ 

Per trovare $$b$$ dobbiamo imporre l'ultima condizione che ci dice il testo, ossia che la funzione deve passare per il punto $$A$$. Vado quindi a imporre che $$x$$ e $$y$$ del punto soddisfino l'equazione:

$$\begin{align*}
14 & = \frac{6(3)+b}{(3)-2} \\
14 & = \frac{18+b}{1} \\
b+18 & = 14 \\
b & = 14-18 \\
b & = -4
\end{align*}$$

L'iperbole trovata ha quindi equazione

$$y=\frac{6x-4}{x-2}$$

Per disegnarla partiamo disegnando gli asintoti.

$$\begin{tikzpicture}[scale=1.0544]
\begin{axis}
[axis lines=middle, axis line style=gray, 
xtick = {2}, ytick = {6},
xlabel=$x$,ylabel=$y$]
\addplot[black,dashed] coordinates {
(2,-5)
(2,15)
};
\addplot[black,dashed] coordinates {
(-2,6)
(4.5,6)
};
\end{axis}
\end{tikzpicture}$$

Per capire in quali quadranti sta l'iperbole, o ci ricordiamo le formule per i fuochi, oppure inseriamo una qualsiasi $$x$$ nell'equazione e calcoliamo la $$y$$. Se infatti mettiamo $$x=0$$ otteniamo $$y=2$$, quindi il punto $$(0;2)$$ appartiene all'iperbole. 

$$\begin{tikzpicture}[scale=1.0544]
\begin{axis}
[axis lines=middle, axis line style=gray, 
xtick = {2}, ytick = {2,6},
xlabel=$x$,ylabel=$y$]
\addplot[black,dashed] coordinates {
(2,-5)
(2,15)
};
\addplot[black,dashed] coordinates {
(-2,6)
(4.5,6)
};
\addplot[red, mark=*, only marks] coordinates {(0,2)};
\end{axis}
\end{tikzpicture}$$

L'iperbole quindi sta nel primo e terzo quadrante. Il suo grafico è 

$$\begin{tikzpicture}[scale=1.0544]
\begin{axis}
[axis lines=middle, axis line style=gray, enlarge x limits, 
xtick =none, ytick = none,
xlabel=$x$,ylabel=$y$]
\addplot
[domain=-1:1.9,samples=200,smooth,
thick,red]
{(6*x-4)/(x-2)};
\addplot
[domain=2.1:4.5,samples=200,smooth,
thick,red]
{(6*x-4)/(x-2)};
\addplot[black,dashed] coordinates {
(2,-80)
(2,100)
};
\addplot[black,dashed] coordinates {
(-1,6)
(4.5,6)
};
\addplot[red] coordinates {(3,-20)} node{$y=\frac{6x-4}{x-2}$};
\end{axis}
\end{tikzpicture}$$





