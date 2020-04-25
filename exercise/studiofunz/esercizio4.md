# STUDIO DI FUNZIONE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Studia e rappresenta graficamente la seguente funzione

$$y = x^4-5x^2+4$$

## Soluzione: 

Come prima cosa ricordo a grandi linee gli step necessari per studiare una funzione 

1. trovare le condizioni di esistenza (C.E.)
1. vedere se la funzione è simmetrica
1. stabilire il segno della funzione, ossia guardare quando la funzione è maggiore o uguale a zero
1. limiti agli estremi e nei punti di discontinuità (se ci sono) 
1. studio della derivata prima per trovare massimi e minimi 
1. studio della derivata seconda per trovare punti di flesso

Il primo consiglio che darei è quello di disegnare SUBITO ogni cosa che trovo in ogni step, così non si perdono dati per strada. 

### Step 1
In questo caso non ci sono condizioni di esistenza, ossia la funzione è ben definita in tutto $$\mathbb{R}$$. Infatti, la funzione è un polinomio di quarto grado, quindi sappiamo già che ha come dominio $$\mathbb{R}$$ e non ha punti di discontinuità.

### STEP 2

Vedere se la funzione è simmetrica significa vedere se è pari o dispari. Ricordiamo che una funzione $$f$$ è pari se 

$$f(-x) = f(x)$$

mentre è dispari se 

$$f(-x) = -f(x)$$

Andiamo quindi a calcolare nel nostro caso $$f(-x)$$:

$$\begin{align*}
f(-x) & = (-x)^4-5(-x)^2+4 \\
& = x^4-5x^2+4 \\
& = f(x)
\end{align*}$$

La funzione è quindi pari: questo significa che il grafico sarà simmetrico rispetto all'asse $$y$$. 

### STEP 3

Andiamo ora a vedere quando $$y = f(x) = x^4-5x^2+4 \geq 0$$.

Per risolvere questa disequazione introduciamo una variabile ausiliaria: poniamo $$t = x^2$$. Così facendo, la disequazione diventa

$$t^2-5t+4 \geq 0$$

Abbiamo quindi trasformato una disequazione di quarto grado in una disequazione di secondo grado, che sappiamo risolvere. 

$$\begin{align*}
t^2-5t+4 & \geq 0 \\
& \downarrow \\
\text{equazione} & \; \text{associata} \\
t^2-5t+4 & = 0 \\
t_{1/2} & = \frac{-b\pm\sqrt{b^2-4ac}}{2a} \\
& = \frac{-(-5)\pm\sqrt{(-5)^2-4(1)(4)}}{2(1)} \\
& = \frac{+5\pm\sqrt{25-16}}{2} \\
& = \frac{5 \pm 3}{2} \\
& = \begin{cases}
4 \\
1
\end{cases} \\
& \downarrow \\
\text{poichè avevo} \geq & \Rightarrow \text{intervalli esterni:} \\
t \leq 1 \; \; & \vee \; \; t \geq 4
\end{align*}$$ 

Ora che ho trovato la soluzione in $$t$$, devo tornare indietro e sostituire $$t=x^2$$ per trovare le soluzioni in $$x$$.

Dalla prima disuguaglianza $$t \leq 1$$ ottengo 

$$\begin{align*}
t & \leq 1 \\
x^2 & \leq 1 \\
& \downarrow \\
\text{equazione} & \; \text{associata} \\
x^2 & = 1 \\
x & = \pm 1 \\
& \downarrow \\
\text{poichè avevo} \leq & \Rightarrow \text{intervalli interni:} \\
-1 \leq \; & x \leq 1
\end{align*}$$

Dalla seconda disuguaglianza $$t \geq 4$$ ottengo 

$$\begin{align*}
t & \geq 4 \\
x^2 & \geq 4 \\
& \downarrow \\
\text{equazione} & \; \text{associata} \\
x^2 & = 4 \\
x & = \pm 2 \\
& \downarrow \\
\text{poichè avevo} \geq & \Rightarrow \text{intervalli esterni:} \\
x \leq -2 \; \; & \vee \; \; x \geq 2
\end{align*}$$

Mettendo tutto insieme, abbiamo scoperto che la funzione è positiva in

$$x \leq -2 \vee -1 \leq x \leq 1 \vee x \geq 2$$

Riportiamo queste informazioni sul grafico. Indico con il grigio le zone in cui la funzione "non c'è"; i pallini rossi sull'asse delle $$x$$ indicano le intersezioni (i punti in cui la funzione è zero), ossia i punti $$x = \pm 2, x = \pm 1$$ nel nostro caso. 

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-3, xmax=3,
	ymin=-3, ymax=8,
	restrict y to domain=-3:8,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
%\addplot[red,domain=-6:6,semithick]{exp(x)};
%\addplot[black]{x+1};
\fill[grey!10]
(axis cs:-3,-3) --
(axis cs:-2,-3) --
(axis cs:-2,0) --
(axis cs:-3,0) --
cycle;
\fill[grey!10]
(axis cs:-2,0) --
(axis cs:-1,0) --
(axis cs:-1,8) --
(axis cs:-2,8) --
cycle;
\fill[grey!10]
(axis cs:-1,0) --
(axis cs:-1,-3) --
(axis cs:1,-3) --
(axis cs:1,0) --
cycle;
\fill[grey!10]
(axis cs:1,0) --
(axis cs:2,0) --
(axis cs:2,8) --
(axis cs:1,8) --
cycle;
\fill[grey!10]
(axis cs:2,0) --
(axis cs:3,0) --
(axis cs:3,-3) --
(axis cs:2,-3) --
cycle;
\addplot[red, mark=*, only marks] coordinates {(-1,0) (1,0) (-2,0) (2,0)};
\addplot[] coordinates {(1,-0.5)} node{\small $1$};
\addplot[] coordinates {(2,-0.5)} node{\small $2$};
\addplot[] coordinates {(-1,-0.5)} node{\small $-1$};
\addplot[] coordinates {(-2,-0.5)} node{\small $-2$};
%\addplot[red] coordinates {(-1,0.6)} node{$y=e^x$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

### STEP 4

Andiamo a vedere i limiti agli estremi del nostro dominio. 

$$\lim_{x \rightarrow +\infty} x^4-5x^2+4 = "+\infty-\infty"$$

Per risolvere la forma indeterminata basta semplicemente raccogliere il termine di grado maggiore, ossia $$x^4$$.

$$\begin{align*}
\lim_{x \rightarrow +\infty} x^4-5x^2+4 & = \lim_{x \rightarrow +\infty} x^4\left(1-\frac{5}{x^2}+\frac{4}{x^4}\right) \\
& = +\infty
\end{align*}$$  

perchè le due frazioni fra parentesi tendono a zero.

Abbiamo quindi ottenuto che la funzione va a $$+\infty$$ per $$x\rightarrow + \infty$$. Poichè abbiamo stabilito che la funzione è pari, ossia simmetrica rispetto l'asse $$y$$ ho che anche il limite per $$x \rightarrow -\infty$$ è $$+\infty$$. 

Siamo ufficialmente nel caso in cui potrebbero esserci degli asintoti obliqui. Dobbiamo andare a verificare se esiste un asintoto obliquo, ossia se la funzione tende a una retta del tipo $$y = mx + q$$ quando $$x\rightarrow + \infty$$. Ricordo che in generale il primo step è calcolare

$$\lim_{x\rightarrow +\infty} \frac{f(x)}{x} = m$$

Se il limite di $$\frac{f(x)}{x}$$ esiste finito, allora quel limite sarà il coefficiente di $$x$$ nella formula della retta. Il secondo step è calcolare

$$\lim_{x\rightarrow +\infty} f(x) -mx = q$$

Se il limite di $$f(x) -mx$$ esiste finito, allora quel limite sarà il termine noto nella formula della retta.

Andiamo quindi a calcolare

$$\lim_{x\rightarrow +\infty} \frac{f(x)}{x}$$

Nel nostro caso diventa

$$\lim_{x\rightarrow +\infty} \frac{x^4-5x^2+4}{x}$$

Come prima, raccogliamo il termine di grado maggiore a numeratore:

$$\begin{align*}
\lim_{x \rightarrow +\infty} \frac{x^4-5x^2+4}{x} & = \lim_{x \rightarrow +\infty} \frac{x^4\left(1-\frac{5}{x^2}+\frac{4}{x^4}\right)}{x} \\
& = \lim_{x \rightarrow +\infty} \frac{x^3\left(1-\frac{5}{x^2}+\frac{4}{x^4}\right)}{1} \\
& = +\infty
\end{align*}$$

Dal momento che non abbiamo trovato un limite finito, la funzione non ha asintoti obliqui nè a $$+\infty$$ nè a $$-\infty$$ visto che è una funzione simmetrica rispetto l'asse $$y$$. 

Riportiamo sul grafico quello che abbiamo trovato. Disegno in rosso la funzione. 

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-3, xmax=3,
	ymin=-3, ymax=8,
	restrict y to domain=-3:8,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\fill[grey!10]
(axis cs:-3,-3) --
(axis cs:-2,-3) --
(axis cs:-2,0) --
(axis cs:-3,0) --
cycle;
\fill[grey!10]
(axis cs:-2,0) --
(axis cs:-1,0) --
(axis cs:-1,8) --
(axis cs:-2,8) --
cycle;
\fill[grey!10]
(axis cs:-1,0) --
(axis cs:-1,-3) --
(axis cs:1,-3) --
(axis cs:1,0) --
cycle;
\fill[grey!10]
(axis cs:1,0) --
(axis cs:2,0) --
(axis cs:2,8) --
(axis cs:1,8) --
cycle;
\fill[grey!10]
(axis cs:2,0) --
(axis cs:3,0) --
(axis cs:3,-3) --
(axis cs:2,-3) --
cycle;
\addplot[red, mark=*, only marks] coordinates {(-1,0) (1,0) (-2,0) (2,0)};
\addplot[] coordinates {(1,-0.5)} node{\small $1$};
\addplot[] coordinates {(2,-0.5)} node{\small $2$};
\addplot[] coordinates {(-1,-0.5)} node{\small $-1$};
\addplot[] coordinates {(-2,-0.5)} node{\small $-2$};
\addplot[red,domain=-3:-2.35,semithick]{x^4-5*x^2+4};
\addplot[red,domain=3:2.35,semithick]{x^4-5*x^2+4};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

### STEP 5 

Calcoliamo la derivata prima: indico con $$D$$ o $$'$$ il simbolo di derivata.

$$\begin{align*}
y^{'} & = D(x^4-5x^2+4) \\
& = D(x^4)-5D(x^2)+D(4) \\
& = 4x^3-5(2x)+0 \\
& = 4x^3-10x
\end{align*}$$

Devo ora studiare il segno della derivata prima, ossia quando $$y^{'} \geq 0 $$. Nel nostro caso

$$4x^3-10x \geq 0$$

Raccolgo $$2x$$ e ottengo 

$$2x(2x^2-5) \geq 0$$

Visto che ho un prodotto, studio singolarmente i due fattori. 

Fattore 1: $$2x \geq 0 \Rightarrow x \geq 0$$

Fattore 2: $$2x^2-5 \geq 0 \Rightarrow x^2 \geq \frac{5}{2} \Rightarrow x \leq -\sqrt{\frac{5}{2}} \vee x \geq \sqrt{\frac{5}{2}}$$

Costruisco quindi il castello dei segni per stabilire il segno del prodotto

$$\begin{tikzpicture}
\draw (-2.5,0) -- (2.5,0);
\draw (0,3) -- (0,-0.2);
\draw (-1.5,3) -- (-1.5,-0.2);
\draw (1.5,3) -- (1.5,-0.2);
\node at (0,-0.5) {$0$};
\node at (-1.5,-0.5) {$-\sqrt{\frac{5}{2}}$};
\node at (1.5,-0.5) {$\sqrt{\frac{5}{2}}$};
\draw (-2.5,2) -- (2.5,2);
\draw (-2.5,1) -- (2.5,1);
%Numeratore
\node at (-3.5,2.5) {\scriptsize Fattore 1:};
\node at (-0.75,2.5) {$-$};
\node at (-2,2.5) {$-$};
\node at (0.75,2.5) {$+$};
\node at (2,2.5) {$+$};
\draw [fill = black](0,2.5) circle (0.07cm);
%Denominatore
\node at (-3.5,1.5) {\scriptsize Fattore 2:};
\node at (-0.75,1.5) {$-$};
\node at (-2,1.5) {$+$};
\node at (0.75,1.5) {$-$};
\node at (2,1.5) {$+$};
\draw [fill = black](-1.5,1.5) circle (0.07cm);
\draw [fill = black](1.5,1.5) circle (0.07cm);
%Frazione
\node at (-3.5,0.5) {\scriptsize Prodotto:};
\node at (-0.75,0.5) {$+$};
\node at (-2,0.5) {$-$};
\node at (0.75,0.5) {$-$};
\node at (2,0.5) {$+$};
\draw [fill = black](-1.5,0.5) circle (0.07cm);
\draw [fill = black](1.5,0.5) circle (0.07cm);
\draw [fill = black](0,0.5) circle (0.07cm);
\draw[->] (-2.5,-1) -- (-1.5,-2);
\draw[->] (-1.4,-2)--(0,-1);
\draw[->] (0.1,-1) -- (1.5,-2);
\draw[->] (1.6,-2)--(2.5,-1);
\end{tikzpicture}$$

La funzione è quindi decrescente negli intervalli $$\left(-\infty,-\sqrt{\frac{5}{2}}\right)$$ e $$\left(0, \sqrt{\frac{5}{2}}\right)$$ mentre è crescente in $$\left(-\sqrt{\frac{5}{2}},0\right)$$ e $$\left(\sqrt{\frac{5}{2}},+\infty\right)$$. 
Abbiamo quindi che zero è un massimo relativo della funzione (relativo perchè la funzione tende a infinito agli estremi), mentre $$\pm \sqrt{\frac{5}{2}}$$ sono minimi assoluti.  

### STEP 6

Calcoliamo la derivata seconda.

$$\begin{align*}
y^{''} & = D(4x^3-10x) \\
& = 4D(x^3)-10D(x) \\
& = 4(3x^2)-10(1) \\
& = 12x^2-10
\end{align*}$$

Devo ora studiare il segno della derivata seconda, ossia quando $$y^{''} \geq 0 $$. Nel nostro caso

$$\begin{align*}
12x^2-10 & \geq 0 \\
12x^2 & \geq 10 \\
x^2 & \geq \frac{10}{12} \\
x^2 & \geq \frac{5}{6} \\
& \downarrow \\
\text{equazione} \; & \; \text{associata} \\
x^2 & = \frac{5}{6} \\
x & = \pm \sqrt{\frac{5}{6}}\\
& \downarrow \\
\text{poichè avevo} \geq & \Rightarrow \text{intervalli esterni:} \\
x \leq -\sqrt{\frac{5}{6}} \; \; & \vee \; \; x \geq \sqrt{\frac{5}{6}}
\end{align*}$$

Dallo studio della derivata seconda possiamo quindi dire che esistono due punti di flesso: $$x=\pm \sqrt{\frac{5}{6}}$$. 

$$\begin{tikzpicture}
\draw (-2,0)--(2,0);
\draw (-1,-0.2)--(-1,1);
\draw (1,-0.2)--(1,1);
\node at (-3,0.5) {$y^{''}\geq 0$};
\node at (-1,-0.5) {$-\sqrt{\frac{5}{6}}$};
\node at (1,-0.5) {$\sqrt{\frac{5}{6}}$};
\node at (-1.5,0.5) {$+$};
\node at (1.5,0.5) {$+$};
\node at (0,0.5) {$-$};
\draw (-2,-1) arc (-180:0:0.4);
\draw (-0.4,-1.4) arc (180:0:0.4);
\draw (1.5,-1) arc (-180:0:0.4);
\end{tikzpicture}$$

La funzione è quindi convessa $$(y^{''} > 0)$$ in $$\left(-\infty, -\sqrt{\frac{5}{6}}\right) \cup \left(\sqrt{\frac{5}{6}},+\infty\right)$$ mentre è concava $$(y^{''} < 0)$$ in $$\left(-\sqrt{\frac{5}{6}}, \sqrt{\frac{5}{6}}\right)$$. 

Il grafico finale della funzione è quindi 


$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-3, xmax=3,
	ymin=-3, ymax=8,
	restrict y to domain=-3:8,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\fill[grey!10]
(axis cs:-3,-3) --
(axis cs:-2,-3) --
(axis cs:-2,0) --
(axis cs:-3,0) --
cycle;
\fill[grey!10]
(axis cs:-2,0) --
(axis cs:-1,0) --
(axis cs:-1,8) --
(axis cs:-2,8) --
cycle;
\fill[grey!10]
(axis cs:-1,0) --
(axis cs:-1,-3) --
(axis cs:1,-3) --
(axis cs:1,0) --
cycle;
\fill[grey!10]
(axis cs:1,0) --
(axis cs:2,0) --
(axis cs:2,8) --
(axis cs:1,8) --
cycle;
\fill[grey!10]
(axis cs:2,0) --
(axis cs:3,0) --
(axis cs:3,-3) --
(axis cs:2,-3) --
cycle;
\addplot[red, mark=*, only marks] coordinates {(-1,0) (1,0) (-2,0) (2,0)};
\addplot[black,dashed] coordinates {
((5/2)^(1/2),-9/4)
((5/2)^(1/2),0)
};
\addplot[black,dashed] coordinates {
(-(5/2)^(1/2),-9/4)
(-(5/2)^(1/2),0)
};
\addplot[] coordinates {(1,-0.5)} node{\small $1$};
\addplot[] coordinates {(2,-0.5)} node{\small $2$};
\addplot[] coordinates {(-1,-0.5)} node{\small $-1$};
\addplot[] coordinates {(-2,-0.5)} node{\small $-2$};
\addplot[] coordinates {((5/2)^(1/2),0.6)} node{\tiny $\sqrt{\frac{5}{2}}$};
\addplot[] coordinates {(-(5/2)^(1/2),0.6)} node{\tiny $-\sqrt{\frac{5}{2}}$};
\addplot[red,domain=-2.7:2.7,semithick]{x^4-5*x^2+4};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$



