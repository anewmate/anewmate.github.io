# STUDIO DI FUNZIONE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Studia e rappresenta graficamente la seguente funzione

$$y = e^{\frac{x^2-1}{2x}}$$

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

Le condizioni di esistenza che dobbiamo porre in questo caso riguardano l'esistenza della frazione. Sappiamo che una frazione esiste solo se il denominatore è diverso da zero, quindi la prima C.E. è 

$$2x \neq 0$$

Non ci sono invece restrizioni per l'esistenza dell'esponenziale.

L'unica mia C.E. è quindi 

$$2x \neq 0 \Rightarrow x \neq 0$$

### STEP 2

Vedere se la funzione è simmetrica significa vedere se è pari o dispari. Ricordiamo che una funzione $$f$$ è pari se 

$$f(-x) = f(x)$$

mentre è dispari se 

$$f(-x) = -f(x)$$

Andiamo quindi a calcolare nel nostro caso $$f(-x)$$:

$$\begin{align*}
f(-x) & = e^{\frac{(-x)^2-1}{2(-x)}} \\
& = e^{\frac{x^2-1}{-2x}} \\
& = e^{-\frac{x^2-1}{2x}} \\
f(-x) & \neq \begin{cases}
f(x) = e^{\frac{x^2-1}{2x}} \\
-f(x) = -e^{\frac{x^2-1}{2x}}
\end{cases}
\end{align*}$$

La funzione non è quindi nè pari nè dispari. 

### STEP 3

Andiamo ora a vedere quando $$y = f(x) = e^{\frac{x^2-1}{2x}} \geq 0$$. Dal momento che un'esponenziale è sempre positivo, la disequazione è sempre verificata. Ricordiamo infatti che 

$$e^{\star(x)} \geq 0 \qquad \forall \; x \in \mathbb{R}$$

dove $$\star(x)$$ è una qualsiasi funzione di $$x$$. Nel nostro caso $$\star(x) = \frac{x^2-1}{2x}$$ e $$e^{\frac{x^2-1}{2x}} \geq 0$$ è verificata per ogni $$x$$ in $$\mathbb{R}$$. Andiamo a raffigurare subito quello che abbiamo trovato. A parole abbiamo sostanzialmente provato che la funzione non assume mai valori negativi, ossia $$y$$ negative. Indico in griglio le regioni in cui non c'è la funzione.  

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
(axis cs:-6,-6) --
(axis cs:6,-6) --
(axis cs:6,0) --
(axis cs:-6,0) --
cycle;
\addplot[grey!10] coordinates {
(-1,-1)
(4.5,-1)
};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

### STEP 4

Andiamo a vedere i limiti agli estremi del nostro dominio. 

$$\lim_{x \rightarrow +\infty} e^{\frac{x^2-1}{2x}} = "e^{\frac{\infty}{\infty}}"$$

Per risolvere la forma indeterminata possiamo procedere in due modi. Il primo è quello di ragionare sugli asintotici. Infatti, nella frazione, il numeratore a più infinito si comporta come $$x^2$$ mentre il denominatore come $$x$$. Quindi 

$$e^{\frac{x^2-1}{2x}} \sim e^{\frac{x^2}{x}} = e^{x} \longrightarrow +\infty$$

La seconda alternativa è quella di fare effettivamente i conti raccogliendo i termini di grado maggiore nella frazione:

$$\begin{align*}
\lim_{x \rightarrow +\infty} e^{\frac{x^2-1}{2x}} &  = \lim_{x \rightarrow +\infty} e^{\frac{x^2\left(1-\frac{1}{x^2}\right)}{2x}} \\
& = \lim_{x \rightarrow +\infty} e^{\frac{x\left(1-\frac{1}{x^2}\right)}{2}} \\
& = "e^{+\infty}" \\
& = +\infty
\end{align*}$$

dove nel terzo passaggio ho che $$\frac{1}{x^2} \rightarrow 0$$ quando $$x \rightarrow +\infty$$.

Poichè il limite a $$+\infty$$ è $$+\infty$$, dobbiamo andare a verificare se esiste un asintoto obliquo, ossia se la funzione tende a una retta del tipo $$y = mx + q$$ quando $$x\rightarrow + \infty$$. Ricordo che in generale il primo step è calcolare

$$\lim_{x\rightarrow +\infty} \frac{f(x)}{x} = m$$

Se il limite di $$\frac{f(x)}{x}$$ esiste finito, allora quel limite sarà il coefficiente di $$x$$ nella formula della retta. Il secondo step è calcolare

$$\lim_{x\rightarrow +\infty} f(x) -mx = q$$

Se il limite di $$f(x) -mx$$ esiste finito, allora quel limite sarà il termine noto nella formula della retta.

Andiamo quindi a calcolare

$$\lim_{x\rightarrow +\infty} \frac{f(x)}{x}$$

Abbiamo già notato che $$e^{\frac{x^2-1}{2x}} \sim e^x$$ quando $$x$$ è molto grande. Quindi

$$\begin{align*}
\lim_{x \rightarrow +\infty} \frac{e^{\frac{x^2-1}{2x}}}{x} &  \sim \lim_{x \rightarrow +\infty} \frac{e^x}{x} \\
& = "\frac{\infty}{\infty}" \\
& \overset{\text{De l'Hopital}}{=} \lim_{x \rightarrow +\infty} \frac{e^x}{1} \\
& = +\infty
\end{align*}$$

Alternativamente a De l'Hopital, possiamo proseguire sulla strada degli ordini di infinito: ricordiamo infatti che per $$\mathbf{x \rightarrow + \infty}$$ l'ordine di infiniti è

$$\log_a(x) << x^b << c^x << x^x$$

con $$a>0,a\neq 1, b>0, c >1$$.

Abbiamo quindi che l'esponenziale di $$x$$ tende a più infinito molto più velocemente di $$x$$, quindi nella frazione $$\frac{e^x}{x}$$ "vince" il numeratore che porta tutto al suo limite, ossia $$e^{+\infty} = +\infty$$. 

Non avendo ottenuto un limite finito, non esiste un asintoto obliquo a $$+\infty$$. 

Passiamo ora al limite a meno infinito. 

$$\begin{align*}
\lim_{x \rightarrow -\infty} e^{\frac{x^2-1}{2x}} &  = \lim_{x \rightarrow -\infty} e^{\frac{x^2\left(1-\frac{1}{x^2}\right)}{2x}} \\
& = \lim_{x \rightarrow -\infty} e^{\frac{x\left(1-\frac{1}{x^2}\right)}{2}} \\
& = "e^{-\infty}" \\
& = 0
\end{align*}$$

Per $$x\rightarrow -\infty$$ abbiamo quindi l'asintoto orizzontale $$y=0$$ (ossia l'asse delle $$x$$). 

Passiamo ora ai limiti dell' asintoto verticale. 

$$\begin{align*}
\lim_{x \rightarrow 0^+} e^{\frac{x^2-1}{2x}} &  = "e^{\frac{-1^+}{0^+}}" \\
& = "e^{-\infty}" \\
& = 0
\end{align*}$$

poichè a numeratore della frazione a esponente ho un numero negativo e a denominatore un numero positivo.

$$\begin{align*}
\lim_{x \rightarrow 0^-} e^{\frac{x^2-1}{2x}} &  = "e^{\frac{-1^-}{0^-}}" \\
& = "e^{+\infty}" \\
& = +\infty
\end{align*}$$

poichè a numeratore e a denominatore della frazione a esponente ho un numero negativo.


Riportiamo sul grafico quello che abbiamo trovato. Disegno in rosso la funzione. 

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=500,
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
(axis cs:-6,-6) --
(axis cs:6,-6) --
(axis cs:6,0) --
(axis cs:-6,0) --
cycle;
\addplot[grey!10] coordinates {
(-1,-1)
(4.5,-1)
};
\addplot[black, mark=o, only marks] coordinates {(0,0)};
\addplot[red,domain=-6:-5,semithick]{exp((x^2-1)/(2*x))};
\addplot[red,domain=-0.3:-0.1,semithick]{exp((x^2-1)/(2*x))};
\addplot[red,domain=0.1:0.5,semithick]{exp((x^2-1)/(2*x))};
\addplot[red,domain=3.5:4.5,semithick]{exp((x^2-1)/(2*x))};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$


### STEP 5 

Calcoliamo la derivata prima: è una funzione composta, quindi applichiamo la formula della derivata di $$f(g(x))$$: indico con $$D$$ o $$'$$ il simbolo di derivata.

$$\begin{align*}
y^{'} & = e^{\frac{x^2-1}{2x}} \cdot \frac{2x(2x)-(x^2-1)(2)}{(2x)^2} \\
& = e^{\frac{x^2-1}{2x}} \cdot \frac{4x^2-2x^2+2}{4x^2} \\
& = e^{\frac{x^2-1}{2x}} \cdot \frac{2x^2+2}{4x^2} \\
& = e^{\frac{x^2-1}{2x}} \cdot \frac{2(x^2+1)}{4x^2} \\
& = e^{\frac{x^2-1}{2x}} \cdot \frac{x^2+1}{2x^2}
\end{align*}$$

***
Ricordiamo in breve come si calcola una derivata composta:

$$D(f(g(x))) = f^{'}(g(x))\cdot g^{'}(x)$$

Nel nostro caso $$f(x) = e^x$$ e $$g(x) = \frac{x^2-1}{2x}$$. Infatti 

$$f(g(x)) = e^{\frac{x^2-1}{2x}}$$

ossia al posto della $$x$$ nella definizione di $$f$$ devo mettere $$g(x)$$. Con queste definizioni ho

$$\begin{align*}
f^{'}(x) & = e^x \\
g^{'}(x) & = \text{derivata di una frazione} \\
& = \frac{D(x^2-1)\cdot 2x - (x^2-1) \cdot D(2x)}{(2x)^2} \\
& = \frac{2x\cdot 2x - (x^2-1) \cdot 2}{(2x)^2}
\end{align*}$$

Mettendo insieme i pezzi ho che $$f^{'}(g(x))$$ è $$e^{\frac{x^2-1}{2x}}$$ e la derivata finale 

$$D\left(e^{\frac{x^2-1}{2x}}\right) = e^{\frac{x^2-1}{2x}} \cdot \frac{2x\cdot 2x - (x^2-1) \cdot 2}{(2x)^2}$$

***

Dovrei ora studiare il segno della derivata prima, ossia quando $$y^{'} \geq 0 $$:

$$e^{\frac{x^2-1}{2x}} \cdot \frac{x^2+1}{2x^2} \geq 0$$

Andiamo ad analizzare singolarmente i tre elementi che costituiscono questa derivata: l'esponenziale, il numeratore e il denominatore. 

Come abbiamo detto prima, un esponenziale è sempre positivo: quindi il fattore $$e^{\frac{x^2-1}{2x}}$$ è sempre maggiore o uguale a zero. 

Il numeratore è $$x^2+1$$: sappiamo che un quadrato è sempre positivo, quindi $$x^2$$ è sempre maggiore o uguale di zero. Se a questo $$x^2$$ ci aggiungiamo $$+1$$, a maggior ragione otteniamo un elemento maggiore o uguale di zero. Quindi anche il numeratore è sempre positivo.

$$\text{qualcosa positivo} + \text{qualcosa positivo} = \text{qualcosa positivo}$$

Il denominatore è $$2x^2$$: analogamente al numeratore, so che $$x^2$$ è sempre positivo poichè è un quadrato. Se moltiplico $$x^2$$ per $$+2$$ ottengo sempre qualcosa di positivo. Quindi anche il denominatore è positivo. 

$$\text{qualcosa positivo} \cdot  \text{qualcosa positivo} = \text{qualcosa positivo}$$

Quindi, quando vado a moltiplicare fra loro tutti e tre i fattori, sto moltiplicando sempre cose positive: il risultato non può che essere positivo. 

Ottengo quindi che la derivata è sempre positiva, ossia $$y^{'} \geq 0 \; \forall \; x \in \mathbb{R}$$. Tradotto, la funzione è sempre crescente. 

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
y^{'} & = e^{\frac{x^2-1}{2x}} \cdot \frac{x^2+1}{2x^2} \\
y^{''} & = D\left(e^{\frac{x^2-1}{2x}}\right) \cdot \frac{x^2+1}{2x^2} + e^{\frac{x^2-1}{2x}} \cdot D\left(\frac{x^2+1}{2x^2}\right) \\
& = e^{\frac{x^2-1}{2x}} \cdot \frac{x^2+1}{2x^2} \cdot \frac{x^2+1} {2x^2} + e^{\frac{x^2-1}{2x}} \cdot \frac{2x(2x^2)-(x^2+1)(4x)}{4x^4} \\
& = e^{\frac{x^2-1}{2x}} \left(\frac{(x^2+1)^2}{4x^4} + \frac{4x^3-4x^3-4x}{4x^4} \right) \\
& = e^{\frac{x^2-1}{2x}} \left(\frac{(x^2+1)^2-4x}{4x^4} \right) \\
& = e^{\frac{x^2-1}{2x}} \left(\frac{x^4+1+2x^2-4x}{4x^4} \right)
\end{align*}$$

Andiamo ora a studiare quando questa è positiva. Con ragionamento analogo a quello fatto per la derivata prima, abbiamo che l'esponenziale è sempre positivo, così come il fattore $$4x^4$$. Quindi, studiare $$y^{''} \geq 0$$ equivale a studiare $$x^4+2x^2-4x+1 \geq 0$$. 

Cerchiamo di scomporre questo polinomio utilizzando Ruffini. Vediamo che per $$x=1$$ abbiamo

$$(1)^4+2(1)^2-4(1)+1 = 0$$

quindi $$x=1$$ è una radice del polinomio. 

$$\begin{tikzpicture}
\draw (-0.5,0) -- (3,0);
\draw (0,1.5)--(0,-0.5);
\draw (2.2,1.5)--(2.2,-0.5);
\node at (0.25,1) {$1$};
\node at (0.75,1) {$0$};
\node at (1.25,1) {$2$};
\node at (1.75,1) {$-4$};
\node at (2.5,1) {$1$};
\node at (-0.25,0.5) {$1$};
\node at (0.25,-0.25) {$1$};
\node at (0.75,0.5) {$1$};
\node at (0.75,-0.25) {$1$};
\node at (1.25,0.5) {$1$};
\node at (1.25,-0.25) {$3$};
\node at (1.75,0.5) {$3$};
\node at (1.75,-0.25) {$-1$};
\node at (2.5,0.5) {$-1$};
\node at (2.5,-0.25) {$0$};
\end{tikzpicture}$$

Posso quindi scomporre $$x^4+2x^2-4x+1$$ come 

$$(x-1)(x^3+x^2+3x-1)$$

Notizia buona: possiamo dire subito che $$x=1$$ è un punto di flesso in quanto la derivata seconda si annulla in questo punto. 

Notizia cattiva: non possiamo dire nulla sul polinomio di terzo grado $$x^3+x^2+3x-1$$ in quanto non lo sappiamo scomporre ulteriormente.

Dallo studio della derivata seconda possiamo quindi dire solo che esiste un punto di flesso in $$x=1$$. 

Dagli elementi che abbiamo trovato ipotizziamo che il grafico sia

 
$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=500,
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
(axis cs:-6,-6) --
(axis cs:6,-6) --
(axis cs:6,0) --
(axis cs:-6,0) --
cycle;
\addplot[grey!10] coordinates {
(-1,-1)
(4.5,-1)
};
\addplot[dashed,black] coordinates {
(1,0)
(1,1)
};
\addplot[dashed,black] coordinates {
(0,1)
(1,1)
};
\addplot[black, mark=o, only marks] coordinates {(0,0)};
\addplot[red,domain=-6:-0.1,semithick]{exp((x^2-1)/(2*x))};
\addplot[red,domain=0.1:4.5,semithick]{exp((x^2-1)/(2*x))};
\addplot[red] coordinates {(-3.8,2)} node{$e^{\frac{x^2-1}{2x}}$};
\addplot[black] coordinates {(1,-0.5)} node{$1$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$




