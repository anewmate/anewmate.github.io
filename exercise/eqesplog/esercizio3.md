# EQUAZIONI LOGARITMICHE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Risolvi la seguente equazione

$$\log_2(2x-1)+\log_2(x) = \log_2(x+4)$$

## Soluzione: 

Come prima cosa devo imporre le condizioni di esistenza (C.E.): affinchè l'equazione abbia senso tutti i logaritmi devono esistere e ciò avviene quando tutti gli argomenti sono positivi. 

$$\begin{align*}
\text{C.E.:} & \qquad \begin{cases}
2x-1 > 0 \\
x > 0 \\
x+4 > 0
\end{cases} \\
\text{C.E.:} & \qquad \begin{cases}
x > \frac{1}{2} \\
x > 0 \\
x > -4
\end{cases} \\
\end{align*}
\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (4,1.5) rectangle (5,0);
\draw (0,0) -- (5,0);
\draw[dashed] (1,0.5) -- (1,-0.2);
\draw[dashed] (3,1) -- (3,-0.2);
\draw[dashed] (4,1.5) -- (4,-0.2);
\node at (1,-0.5) {$-4$};
\node at (3,-0.5) {$0$};
\node at (4,-0.5) {$\frac{1}{2}$};
\draw (1,0.5) -- (5,0.5);
\draw (3,1) -- (5,1);
\draw (4,1.5) -- (5,1.5);
\draw[black] (1,0.5) circle (1.5pt);
\draw[black] (3,1) circle (1.5pt);
\draw[black] (4,1.5) circle (1.5pt);
\end{tikzpicture}
\begin{align*}
\text{C.E.:} & \qquad x > \frac{1}{2}
\end{align*}$$

Una volta trovate le condizioni di esistenza, posso andare a risolvere l'equazione. In questo caso devo solo "sistemare" la parte a sinistra dell'uguale: invece di avere la somma di due logaritmi voglio avere un unico logaritmo. Uso quindi le proprietà dei logaritmi e in particolare la proprietà 

$$\log_a(b) + \log_a(c) = \log_a(b \cdot c)$$

Nel nostro caso $$a = 2$$, $$b = 2x-1$$, $$c = x$$. Quindi 

$$\log_2(2x-1) +\log_2(x) = \log_2((2x-1) \cdot x)$$

Riprendendo l'equazione otteniamo quindi

$$\begin{align*} 
\log_2(2x-1)+\log_2(x) & = \log_2(x+4) \\
\log_2((2x-1) \cdot x) & = \log_2(x+4)
\end{align*}$$

Ora che abbiamo un'uguaglianza fra due logaritmi con la stessa base, possiamo risolvere l'equazione imponendo che gli argomenti dei due logaritmi siano uguali. 

$$\begin{align*} 
\log_2((2x-1) \cdot x) & = \log_2(x+4) \\
(2x-1) \cdot x & = x+4 \\
2x^2-x & = x+4 \\
2x^2 -2x -4 & = 0 \\
2(x^2-x-2) & = 0 \\
x^2-x-2 & = 0 \\
x_{1/2} & = \frac{1\pm\sqrt{1+8}}{2} = \frac{1\pm3}{2}
\end{align*}$$



Abbiamo quindi trovato due potenziali soluzioni $$x = 2$$ e $$x = -1$$. L'ultimo step da fare è controllare se effettivamente le soluzioni che abbiamo trovato sono compatibili con le C.E.. Dato che le C.E. erano $$x > \frac{1}{2}$$, $$x = 2$$ soddisfa le C.E. mentre $$x = -1$$ non le soddisfa e quindi non è una soluzione accettabile. L'unica soluzione dell'esercizio è quindi $$x = 2$$.   


