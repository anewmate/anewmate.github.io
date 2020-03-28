# STUDIO DI FUNZIONE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Studia e rappresenta graficamente la seguente funzione

$$y = \frac{x^2-1}{|x-2|+3x}$$

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

Le condizioni di esistenza che dobbiamo porre in questo caso riguardano l'esistenza della frazione. Prima di fare questo però, ogni volta che abbiamo una funzione con un solo valore assoluto, ci conviene "dividere" la funzione tramite la definizione di valore assoluto e vedere cosa otteniamo. Ricordo la definizione di valore assoluto:

$$|\star(x)| = \begin{cases}
\star(x) & \text{se} \; \star(x) \geq 0 \\
-\star(x) & \text{se} \; \star(x) < 0
\end{cases}$$

dove $$\star(x)$$ è una qualiasi funzione di $$x$$. Per esempio,

$$\begin{align*}
|x^2-2x-1| & = \begin{cases}
x^2-2x-1 & \text{se} \; x^2-2x-1 \geq 0 \\
-x^2+2x+1 & \text{se} \; x^2-2x-1 < 0
\end{cases} \\
|3x-\ln(x)| & = \begin{cases}
3x-\ln(x) & \text{se} \; 3x-\ln(x) \geq 0 \\
-3x+\ln(x) & \text{se} \; 3x-\ln(x) < 0
\end{cases}
\end{align*}$$

Nel nostro caso, 

$$|x-2| = \begin{cases}
x-2 & \text{se} \; x-2 \geq 0 \\
-x+2 & \text{se} \; x-2 < 0
\end{cases}$$

Con questa definizione, la nostra funzione diventa 

$$y = \begin{cases}
\frac{x^2-1}{x-2+3x} & \text{se} \; x-2 \geq 0 \\
\\
\frac{x^2-1}{-x+2+3x} & \text{se} \; x-2 < 0
\end{cases}$$

$$y = \begin{cases}
\frac{x^2-1}{4x-2} & \text{se} \; x \geq 2 \\
\\
\frac{x^2-1}{2x+2} & \text{se} \; x < 2
\end{cases}$$

Inoltre, scomponendo sia numeratore che denominatore otteniamo 

$$y = \begin{cases}
\frac{(x+1)(x-1)}{2(2x-1)} & \text{se} \; x \geq 2 \\
\\
\frac{(x+1)(x-1)}{2(x+1)} & \text{se} \; x < 2
\end{cases}$$

$$y = \begin{cases}
\frac{(x+1)(x-1)}{2(2x-1)} & \text{se} \; x \geq 2 \\
\\
\frac{x-1}{2} & \text{se} \; x < 2
\end{cases}$$

Otteniamo quindi che la nostra funzione, nell'intervallo $$(-\infty,2)$$ in realtà altro non è che una retta. Le uniche C.E. da porre sono quindi quelle relative alla frazione nell'altro intervallo. 

Sappiamo che una frazione esiste solo se il denominatore è diverso da zero, quindi la prima C.E. è 

$$2(2x-1) \neq 0$$

Non ci sono invece restrizioni per l'esistenza della retta.

L'unica mia C.E. è quindi 

$$2(2x-1) \neq 0 \Rightarrow x \neq \frac{1}{2}$$

***
ATTENZIONE: visto che nell'intervallo $$(-\infty,2)$$ la mia funzione è una retta, non occorre studiarla perchè sappiamo già perfettamente come disegnarla e tutte le sue caratteristiche. Da qui in poi mi limito quindi a studiare ciò che succede in $$[2,+\infty)$$, ossia alla funzione $$y = \frac{(x+1)(x-1)}{2(2x-1)} = \frac{x^2-1}{4x-2}$$
***

### STEP 2

Vedere se la funzione è simmetrica significa vedere se è pari o dispari. Ricordiamo che una funzione $$f$$ è pari se 

$$f(-x) = f(x)$$

mentre è dispari se 

$$f(-x) = -f(x)$$

Andiamo quindi a calcolare nel nostro caso $$f(-x)$$:

$$\begin{align*}
f(-x) & = \frac{(-x)^2-1}{4(-x)-2} \\
& = \frac{x^2-1}{-4x-2} \\ 
& = \frac{x^2-1}{-(4x+2)} \\
& = -\frac{x^2-1}{4x+2} \\
f(-x) & \neq \begin{cases}
f(x) = \frac{x^2-1}{4x-2} \\
-f(x) = -\frac{x^2-1}{4x-2}
\end{cases}
\end{align*}$$

La funzione non è quindi nè pari nè dispari. 

### STEP 3

Andiamo ora a vedere quando $$y = f(x) = \frac{x^2-1}{4x-2} \geq 0$$.
 
Dobbiamo quindi risolvere una disequazione fratta. Andiamo a studiare separatamente il segno del numeratore, del denominatore e poi quello della frazione intera. 

#### NUMERATORE

Dobbiamo andare a vedere quando $$x^2-1 \geq 0$$.

$$\begin{align*}
x^2-1 & \geq 0 \\
x^2 & \geq 1 \\
& \downarrow  \\
\text{equazione} & \; \text{associata} \\
x^2 & = 1 \\
x & = \pm 1 \\
& \downarrow \\
\text{avevo} \geq & \Rightarrow \text{intervalli esterni}\\
x \leq -1 & \cup x \geq 1
\end{align*}$$ 

#### DENOMINIATORE

Dobbiamo andare a vedere quando $$4x-2 > 0$$. 

$$\begin{align*}
4x-2 & > 0 \\
4x & > 2 \\
\frac{4x}{4} & > \frac{2}{4} \\
x & > \frac{1}{2}
\end{align*}$$

#### FRAZIONE

Andiamo quindi a costruire il castello dei segni con quello che abbiamo trovato. In particolare, abbiamo che

$$\text{Numeratore} \geq 0: x \leq -1 \cup x \geq 1 \\
\text{Denominatore} > 0: x > \frac{1}{2}$$

Andiamo quindi a mettere una $$+$$ in questi intervalli. 

$$\begin{tikzpicture}
\draw (-2,0)--(2,0);
\draw (-1,-0.2)--(-1,3);
\draw (1,-0.2)--(1,3);
\draw (0,-0.2)--(0,3);
\node at (-1,-0.5) {$-1$};
\node at (0,-0.5) {$\frac{1}{2}$};
\node at (1,-0.5) {$1$};
\node at (-3.5,2.5) {\small Numeratore:};
\node at (-3.5,1.5) {\small Denominatore:};
\node at (-3.5,0.5) {\small Frazione:};
\draw (-2,1)--(2,1);
\draw (-2,2)--(2,2);
%Numeratore
\draw[fill=black] (-1,2.5) circle (0.1cm);
\draw[fill=black] (1,2.5) circle (0.1cm);
\node at (-1.5,2.5) {$+$};
\node at (1.5,2.5) {$+$};
\node at (-0.5,2.5) {$-$};
\node at (0.5,2.5) {$-$};
%Denominatore
\draw (0,1.5) circle (0.1cm);
\node at (-1.5,1.5) {$-$};
\node at (1.5,1.5) {$+$};
\node at (-0.5,1.5) {$-$};
\node at (0.5,1.5) {$+$};
%Frazione
\draw[fill=black] (-1,0.5) circle (0.1cm);
\draw[fill=black] (1,0.5) circle (0.1cm);
\draw (0,0.5) circle (0.1cm);
\node at (-1.5,0.5) {$-$};
\node at (1.5,0.5) {$+$};
\node at (-0.5,0.5) {$+$};
\node at (0.5,0.5) {$-$};
\end{tikzpicture}$$

Visto che stavamo cercando quando la frazione è positiva, le soluzioni sono $$-1 \leq x < \frac{1}{2} \vee x \geq 1$$. 

La funzione è però definita solo su $$[2,+\infty)$$, quindi è questo l'intervallo in cui ci interessa sapere se è positiva o no. Visto che abbiamo trovato che essa è positiva per $$x \geq 1$$, in particolare lo è quindi per $$x \geq 2$$. 

Quindi, la funzione, nell'intervallo in cui è definita, è sempre positiva. 

Andiamo subito a graficare quanto abbiamo trovato. Indico in griglio le regioni in cui non c'è la funzione e in rosso la funzione (disegno già la retta). 

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-6, xmax=6,
	ymin=-6.5, ymax=6.5,
	restrict y to domain=-6:6,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\fill[grey!10]
(axis cs:2,-6) --
(axis cs:6,-6) --
(axis cs:6,0) --
(axis cs:2,0) --
cycle;
\addplot[grey!10] coordinates {
(2,-1)
(4.5,-1)
};
\addplot[black,dashed] coordinates {
(2,-6)
(2,6)
};
\addplot[red,domain=-6:2,semithick]{(x-1)/2};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\addplot[black] coordinates {(2,-0.5)} node{$2$};
\end{axis}
\end{tikzpicture}$$

### STEP 4

Andiamo a vedere i limiti agli estremi del nostro dominio (solo $$[2,+\infty)$$ per il motivo descritto al passo 1).  

$$\lim_{x \rightarrow +\infty} \frac{x^2-1}{4x-2} = "\frac{\infty}{\infty}"$$

Per risolvere la forma indeterminata, visto che abbiamo una frazione di polinomi e stiamo facendo il limite a infinito, dobbiamo raccogliere sia a numeratore che a denominatore il termine di grado maggiore. 

$$\begin{align*}
\lim_{x \rightarrow +\infty} \frac{x^2-1}{4x-2} &  = \lim_{x \rightarrow +\infty} \frac{x^2\left(1-\frac{1}{x^2}\right)}{x\left(4-\frac{2}{x^2}\right)} \\
& = \lim_{x \rightarrow +\infty} \frac{x\left(1-\frac{1}{x^2}\right)}{\left(4-\frac{2}{x^2}\right)} \\
& = +\infty
\end{align*}$$

dove nel terzo passaggio ho che $$\frac{1}{x^2} \rightarrow 0$$ e $$\frac{2}{x^2} \rightarrow 0$$ quando $$x \rightarrow +\infty$$.

Poichè il limite a $$+\infty$$ è $$+\infty$$, dobbiamo andare a verificare se esiste un asintoto obliquo, ossia se la funzione tende a una retta del tipo $$y = mx + q$$ quando $$x\rightarrow + \infty$$. Ricordo che in generale il primo step è calcolare

$$\lim_{x\rightarrow +\infty} \frac{f(x)}{x} = m$$

Se il limite di $$\frac{f(x)}{x}$$ esiste finito, allora quel limite sarà il coefficiente di $$x$$ nella formula della retta. Il secondo step è calcolare

$$\lim_{x\rightarrow +\infty} f(x) -mx = q$$

Se il limite di $$f(x) -mx$$ esiste finito, allora quel limite sarà il termine noto nella formula della retta.

Andiamo quindi a calcolare

$$\lim_{x\rightarrow +\infty} \frac{f(x)}{x}$$

Nel nostro caso diventa

$$\begin{align*}
\lim_{x \rightarrow +\infty} \frac{\frac{x^2-1}{4x-2}}{x} &  = \lim_{x \rightarrow +\infty} \frac{x^2-1}{x(4x-2)} \\
& = \lim_{x \rightarrow +\infty} \frac{x^2-1}{4x^2-2x} \\
& =  \lim_{x \rightarrow +\infty} \frac{x^2\left(1-\frac{1}{x^2}\right)}{x^2\left(4-\frac{2}{x}\right)} \\
& = \lim_{x \rightarrow +\infty} \frac{\left(1-\frac{1}{x^2}\right)}{\left(4-\frac{2}{x}\right)} \\
& = \frac{1}{4}
\end{align*}$$ 

Avendo ottenuto un limite finito, potrebbe esistere un asintoto obliquo a $$+\infty$$. Abbiamo appena trovato $$m = \frac{1}{4}$$ e andiamo quindi a vedere quanto vale $$q$$.

$$\begin{align*}
\lim_{x \rightarrow -\infty} \frac{x^2-1}{4x-2} -\frac{1}{4}x & = \lim_{x \rightarrow -\infty} \frac{x^2-1}{2(2x-1)} -\frac{1}{4}x \\
& = \lim_{x \rightarrow -\infty} \frac{2(x^2-1)-(2x-1)x}{4(2x-1)} \\
& = \lim_{x \rightarrow -\infty} \frac{2x^2-2-2x^2+x}{4(2x-1)} \\
& = \lim_{x \rightarrow -\infty} \frac{x-2}{8x-4} \\
& = \lim_{x \rightarrow -\infty} \frac{x\left(1-\frac{2}{x}\right)}{x\left(8-\frac{4}{x}\right)} \\
& = \lim_{x \rightarrow -\infty} \frac{\left(1-\frac{2}{x}\right)}{\left(8-\frac{4}{x}\right)} \\
& = \frac{1}{8}
\end{align*}$$

Abbiamo quindi un asintoto obliquo a $$+\infty$$: ciò significa che la funzione per $$x\rightarrow +\infty$$ tende alla retta

$$y = \frac{1}{4}x + \frac{1}{8}$$ 

Ufficialmente avremmo anche un asintoto verticale $$x= \frac{1}{2}$$. Non occorre però calcolare i limiti destro e sinistro per $$x$$ che tende a $$\frac{1}{2}$$ perchè in quel punto in realtà la funzione è definita come la retta, e non come la frazione di polinomi. In altre parole, nel dominio dove è definita la frazione di polinomi, ossia in $$[2,+\infty)$$, la funzione non ha asintoti verticali.  

L'unica cosa che forse vale la pena approfondire un attimo, è andare a vedere cosa succede in $$x=2$$, ossia se la funzione lì è continua oppure no. 

$$\begin{align*}
\lim_{x \rightarrow 2^+} \frac{x^2-1}{4x-2} & = \frac{3}{6} = \frac{1}{2} \\
\lim_{x \rightarrow 2^-} \frac{x-1}{2} & = \frac{1}{2}
\end{align*}$$

La funzione è quindi continua in $$x=2$$. 

Riportiamo sul grafico quello che abbiamo trovato. Disegno in rosso la funzione e in verde l'asintoto obliquo.

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=1200,
	width=9.0cm,height=6.4cm,
	xmin=-3, xmax=6,
	ymin=-6.5, ymax=6.5,
	restrict y to domain=-6:6,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\fill[grey!10]
(axis cs:2,-6) --
(axis cs:5.7,-6) --
(axis cs:5.7,0) --
(axis cs:2,0) --
cycle;
\addplot[grey!10] coordinates {
(2,-1)
(4.5,-1)
};
\addplot[black,dashed] coordinates {
(2,-6)
(2,6)
};
\addplot[red,domain=-3:2,semithick]{(x-1)/2};
\addplot[red,domain=5:6,semithick]{(x^2-1)/(4*x-2)};
\addplot[green,domain=-3:6,dashed]{(1/4)*x+(1/8)};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\addplot[black] coordinates {(2,-0.5)} node{$2$};
\end{axis}
\end{tikzpicture}$$


### STEP 5 

Calcoliamo la derivata prima: è una frazione, quindi applichiamo la formula della derivata di $$\frac{f(x)}{g(x)}$$: indico con $$D$$ o $$'$$ il simbolo di derivata.

$$\begin{align*}
y^{'} & = \frac{D(x^2-1)\cdot (4x-2)-(x^2-1)\cdot D(4x-2)}{(4x-2)^2} \\
& = \frac{2x(4x-2)-(x^2-1)(4)}{(4x-2)^2} \\
& = \frac{8x^2-4x-4x^2+4}{(4x-2)^2} \\
& = \frac{4x^2-4x+4}{(4x-2)^2} \\
& = \frac{4(x^2-x+1)}{(2(2x-1))^2} \\
& = \frac{4(x^2-x+1)}{4(2x-1)^2} \\
& = \frac{x^2-x+1}{(2x-1)^2}
\end{align*}$$

Dovrei ora studiare il segno della derivata prima, ossia quando $$y^{'} \geq 0 $$:

$$\frac{x^2-x+1}{(2x-1)^2} \geq 0$$

Visto che il denominatore è sempre positivo (è un quadrato, e i quadrati sono sempre non-negativi), studiare quando quella frazione è maggiore o uguale di zero equivale a studiare quando il numeratore è maggiore o uguale di zero. 

$$x^2-x+1 \geq 0$$

Passo all'equazione associata. 

$$x^2-x+1 = 0$$

Calcolo il delta:

$$\Delta = 1-4(1)(1) = -3 < 0$$

Visto che abbiamo ottenuto un delta negativo e stavamo studiando un $$\geq$$, la soluzione è $$\forall \; x \in \mathbb{R}$$, ossia il numeratore è sempre positivo. 

***
**Memo** sulle disequazioni di secondo grado: arrivati a una formula del tipo $$ax^2+bx+c\gtrless 0$$ con $$\underline{\mathbf{a > 0}}$$, si risolve l'equazione associata $$ax^2+bx+c= 0$$ e

* Se $$\Delta < 0$$:
    * se $$ax^2+bx+c \geq 0 \Rightarrow \forall \; x \in \mathbb{R}$$
    * se $$ax^2+bx+c \leq 0 \Rightarrow \nexists x \in \mathbb{R}$$ 
* Se $$\Delta = 0$$: detta $$x_1$$ la soluzione dell'equazione associata,
    * se $$ax^2+bx+c \geq 0 \Rightarrow \forall \; x \in \mathbb{R}$$
    * se $$ax^2+bx+c \leq 0 \Rightarrow x=x_1$$
    * se $$ax^2+bx+c > 0 \Rightarrow \forall \; x \in \mathbb{R}, x \neq x_1$$
    * se $$ax^2+bx+c < 0 \Rightarrow \nexists x \in \mathbb{R}$$
* Se $$\Delta > 0$$: dette $$x_1,x_2$$ le soluzioni dell'equazione associata, con $$x_2 < x_1$$,
    * se $$ax^2+bx+c \geq 0 \Rightarrow x \leq x_2 \vee x \geq x_1$$
    * se $$ax^2+bx+c \leq 0 \Rightarrow x_2 \leq x \leq x_1$$ 

dove, nell'ultimo caso, gli estremi sono inclusi o esclusi a seconda se la disuguaglianza è stretta o no. 

*** 

Ottengo quindi che la derivata è sempre positiva, ossia $$y^{'} \geq 0 \; \forall \; x \in [2,+\infty)$$. Tradotto, la funzione è sempre crescente. 

$$\begin{tikzpicture}
\draw (-1,0)--(1,0);
\node at (-2,0.5) {$y^{'} \geq 0$:};
\node at (0,0.5) {$+$};
\draw[->] (-0.8,-0.6)--(0.8,-0.3);
\end{tikzpicture}$$

Non esistono quindi punti di massimo o minimo.  

### STEP 6

Calcoliamo la derivata seconda.

$$\begin{align*}
y^{'} & = \frac{x^2-x+1}{(2x-1)^2} \\
y^{''} & = \frac{D(x^2-x+1)\cdot (2x-1)^2 - (x^2-x+1)\cdot D((2x-1)^2)}{(2x-1)^4} \\
& = \frac{(2x-1)(2x-1)^2 - (x^2-x+1)2(2x-1)(2)}{(2x-1)^4} \\
& = \frac{(2x-1)[(2x-1)^2 - 4(x^2-x+1)]}{(2x-1)^4} \\
& = \frac{(2x-1)[4x^2+1-4x - 4x^2+4x-4]}{(2x-1)^4} \\
& = \frac{-3(2x-1)}{(2x-1)^4} 
\end{align*}$$

Andiamo ora a studiare quando questa è positiva. Non semplifico, volutamente, il numeratore con il denominatore perchè lasciando il denominatore così com'è ho che è sempre positivo in quanto è elevato alla quarta. Avendo un denominatore sempre positivo posso andare a studiare il segno solo del numeratore. Se avessi invece semplificato, avrei dovuto studiare il numeratore, il denominatore e poi l'intera frazione costruendo il castello dei segni. 

Quindi, lasciando la derivata seconda scritta così, studiare quando è positiva equivale a studiare quando 

$$-3(2x-1) \geq 0$$

Moltiplico tutto per -1 ricordandomi di cambiare il verso alla disuguaglianza (sto moltiplicando per un numero negativo):

$$\begin{align*}
3(2x-1) & \leq 0 \\
\frac{3(2x-1)}{3} & \leq \frac{0}{3} \\
2x-1 & \leq 0 \\
2x & \leq 1 \\
\frac{2x}{2} & \leq \frac{1}{2} \\
x & \leq \frac{1}{2}
\end{align*}$$ 

Dallo studio della derivata seconda possiamo quindi dire che esiste un punto di flesso in $$x=\frac{1}{2}$$. 

$$\begin{tikzpicture}
\draw (-1,0)--(1,0);
\draw (0,-0.2)--(0,1);
\node at (-2,0.5) {$y^{''}\geq 0$};
\node at (0,-0.5) {$\frac{1}{2}$};
\node at (-0.5,0.5) {$+$};
\node at (0.5,0.5) {$-$};
\draw (-0.9,-0.6) arc (-180:0:0.3);
\draw (0.4,-0.9) arc (180:0:0.3);
\end{tikzpicture}$$

Nel nostro intervallo, $$[2,+\infty)$$ la derivata seconda è negativa e quindi la funzione è concava. 

Dagli elementi che abbiamo trovato, il grafico è dato da 

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=1200,
	width=9.0cm,height=6.4cm,
	xmin=-3, xmax=6,
	ymin=-6.5, ymax=6.5,
	restrict y to domain=-6:6,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\fill[grey!10]
(axis cs:2,-6) --
(axis cs:5.7,-6) --
(axis cs:5.7,0) --
(axis cs:2,0) --
cycle;
\addplot[grey!10] coordinates {
(2,-1)
(4.5,-1)
};
\addplot[black,dashed] coordinates {
(2,-6)
(2,6)
};
\addplot[red,domain=-3:2,semithick]{(x-1)/2};
\addplot[red,domain=2:6,semithick]{(x^2-1)/(4*x-2)};
\addplot[green,domain=-3:6,dashed]{(1/4)*x+(1/8)};
\addplot[black] coordinates {(2,-0.5)} node{$2$};
\addplot[red] coordinates {(-1.5,2.5)} node{$\frac{x^2-1}{|x-2|+3x}$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

Visto così sembrano due rette, ma zoommando un po' intorno a $$x=2$$ il grafico è

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=1200,
	width=9.0cm,height=6.4cm,
	xmin=0, xmax=3,
	ymin=-1, ymax=1,
	restrict y to domain=-1:1,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\fill[grey!10]
(axis cs:2,-1) --
(axis cs:3,-1) --
(axis cs:3,0) --
(axis cs:2,0) --
cycle;
\addplot[grey!10] coordinates {
(2,-1)
(3,-1)
};
\addplot[black,dashed] coordinates {
(2,-1)
(2,1)
};
\addplot[red,domain=0:2,semithick]{(x-1)/2};
\addplot[red,domain=2:3,semithick]{(x^2-1)/(4*x-2)};
\addplot[green,domain=0:3,dashed]{(1/4)*x+(1/8)};
\addplot[red] coordinates {(1,-0.5)} node{$\frac{x^2-1}{|x-2|+3x}$};
\addplot[black] coordinates {(2,-0.5)} node{$2$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$




