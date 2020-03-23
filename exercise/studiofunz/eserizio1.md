# STUDIO DI FUNZIONE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Studia e rappresenta graficamente la seguente funzione

$$y = \frac{\ln(x^2-1)}{x^2-4}$$

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

Le condizioni di esistenza che dobbiamo porre in questo caso riguardano l'esistenza della frazione e l'esistenza del logaritmo. Sappiamo che una frazione esiste solo se il denominatore è diverso da zero, quindi la prima C.E. è 

$$x^2-4 \neq 0$$

Per l'esistenza del logaritmo invece devo imporre che l'argomento del logaritmo sia positivo, ossia

$$x^2-1 > 0$$

Le mie C.E. sono quindi 

$$\begin{cases}
x^2-4 \neq 0 \\
x^2-1 > 0
\end{cases}$$

La prima condizione si risolve come 

$$\begin{align*}
x^2-4 & \neq 0 \\
x^2 & \neq 4 \\
x & \neq \pm 2
\end{align*}$$

mentre la seconda

$$\begin{align*}
x^2-1 & > 0 \\
x^2 & > 1 \\
& \downarrow \\
\text{equazione} & \; \; \text{associata} \\
x^2 & = 1 \\
x & = \pm 1 \\
& \downarrow \\
\text{avevo} > & \Rightarrow \text{intervalli esterni} \\
x < -1 & \cup x > 1
\end{align*}$$

Il sistema diventa quindi 

$$\begin{cases}
x \neq \pm 2 \\
x<-1 \cup x > 1
\end{cases}$$

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (-3,2) rectangle (-2,0);
\shade[left color=yellow, right color = yellow] (-2,2) rectangle (-1,0);
\shade[left color=yellow, right color = yellow] (3,2) rectangle (2,0);
\shade[left color=yellow, right color = yellow] (2,2) rectangle (1,0);
\draw (-3,0) -- (3,0);
\draw (-2,-0.2) -- (-2,2);
\draw (2,-0.2) -- (2,2);
\draw (-1,-0.2) -- (-1,2);
\draw (1,-0.2) -- (1,2);
\node at (-5,0.5) {$x<-1 \cup x > 1$};
\node at (-5,1.5) {$x \neq \pm 2$};
\draw (-3,1.5) -- (3,1.5);
\draw[fill = white] (-2,1.5) circle (0.1cm);
\draw[fill = white] (2,1.5) circle (0.1cm);
\draw (-3,0.5) -- (-1,0.5);
\draw (1,0.5) -- (3,0.5);
\draw[fill = white] (-1,0.5) circle (0.1cm);
\draw[fill = white] (1,0.5) circle (0.1cm);
\node at (-2,-0.5) {$-2$};
\node at (2,-0.5) {$2$};
\node at (-1,-0.5) {$-1$};
\node at (1,-0.5) {$1$};
\end{tikzpicture}$$

Noto che la soluzione (la parte gialla) è di conseguenza il dominio della funzione. Abbiamo quindi trovato che la funzione non esiste fra -1 e 1. Disegniamolo subito: in griglio le sezione dove la funzione non esiste, ossia dove non ci sarà disegnato nulla. Tratteggio invece le $$x$$ non incluse nel dominio. 

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-6, xmax=6,
	ymin=-6.5, ymax=6.5,
	restrict y to domain=-6:6,
	ytick=none,
	%xtick={-1,1},
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
%\addplot[red,domain=-6:6,semithick]{exp(x)};
%\addplot[black]{x+1};
\fill[grey!10]
(axis cs:-1,-6) --
(axis cs:1,-6) --
(axis cs:1,6) --
(axis cs:-1,6) --
cycle;
\addplot[black,dashed] coordinates {
(-1,-6)
(-1,6)
};
\addplot[black,dashed] coordinates {
(1,-6)
(1,6)
};
\addplot[black,dashed] coordinates {
(-2,-6)
(-2,6)
};
\addplot[black,dashed] coordinates {
(2,-6)
(2,6)
};
%\addplot[red, mark=*, only marks] coordinates {(-2,0) (2,0)};
%\addplot[] coordinates {(1,1.5)} node{$y=x+1$};
%\addplot[red] coordinates {(-1,0.6)} node{$y=e^x$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

### STEP 2

Vedere se la funzione è simmetrica significa vedere se è pari o dispari. Ricordiamo che una funzione $$f$$ è pari se 

$$f(-x) = f(x)$$

mentre è dispari se 

$$f(-x) = -f(x)$$

Andiamo quindi a calcolare nel nostro caso $$f(-x)$$:

$$\begin{align*}
f(-x) & = \frac{\ln((-x)^2-1)}{(-x)^2-4} \\
& = \frac{\ln(x^2-1)}{x^2-4} \\
& = f(x)
\end{align*}$$

La funzione è quindi pari: questo significa che il grafico sarà simmetrico rispetto all'asse $$y$$. 

### STEP 3

Andiamo ora a vedere quando $$y = f(x) = \frac{\ln(x^2-1)}{x^2-4} \geq 0$$. Otteniamo una disequazione fratta e dobbiamo quindi studiare separatamente numeratore e denominatore. 

**Numeratore** $$\geq 0$$:

$$\ln(x^2-1) \geq 0 \Rightarrow x^2-1 \geq 1$$

Ricordiamo infatti che un logaritmo è positivo, ossia maggiore di zero, quando il suo argomento è maggiore di uno. 

$$\begin{align*}
x^2-1 & \geq 1 \\
x^2 & \geq 2 \\
& \downarrow \\
\text{equazione} & \; \; \text{associata} \\
x^2 & = 2 \\
x & = \pm \sqrt{2} \\
& \downarrow \\
\text{avevo} \geq & \Rightarrow \text{intervalli esterni} \\
x \leq -\sqrt{2} & \cup x \geq \sqrt{2}
\end{align*}$$

**Denominatore** $$> 0$$:

$$\begin{align*}
x^2-4 & > 0 \\
x^2 & > 4 \\
& \downarrow \\
\text{equazione} & \; \; \text{associata} \\
x^2 & = 4 \\
x & = \pm 2 \\
& \downarrow \\
\text{avevo} > & \Rightarrow \text{intervalli esterni} \\
x < -2 & \cup x > 2
\end{align*}$$

**Segno frazione**:

$$\begin{tikzpicture}
\draw (-3,0) -- (3,0);
\draw (-2,3) -- (-2,-0.2);
\draw (-1,3) -- (-1,-0.2);
\draw (1,3) -- (1,-0.2);
\draw (2,3) -- (2,-0.2);
\node at (-2,-0.5) {$-2$};
\node at (-1,-0.5) {$-\sqrt{2}$};
\node at (1,-0.5) {$\sqrt{2}$};
\node at (2,-0.5) {$2$};
\draw (-3,2) -- (3,2);
\draw (-3,1) -- (3,1);
%Numeratore
\node at (-4.3,2.5) {\scriptsize Numeratore:};
\node at (-2.5,2.5) {$+$};
\node at (-1.5,2.5) {$+$};
\node at (0,2.5) {$-$};
\node at (1.5,2.5) {$+$};
\node at (2.5,2.5) {$+$};
\draw [fill = black](-1,2.5) circle (0.07cm);
\draw [fill = black](1,2.5) circle (0.07cm);
%Denominatore
\node at (-4.3,1.5) {\scriptsize Denominatore:};
\node at (-2.5,1.5) {$+$};
\node at (-1.5,1.5) {$-$};
\node at (0,1.5) {$-$};
\node at (1.5,1.5) {$-$};
\node at (2.5,1.5) {$+$};
\draw(-2,1.5) circle (0.07cm);
\draw(2,1.5) circle (0.07cm);
%Frazione
\node at (-4.3,0.5) {\scriptsize Frazione:};
\node at (-2.5,0.5) {$+$};
\node at (-1.5,0.5) {$-$};
\node at (0,0.5) {$+$};
\node at (1.5,0.5) {$-$};
\node at (2.5,0.5) {$+$};
\draw (-2,0.5) circle (0.07cm);
\draw (2,0.5) circle (0.07cm);
\draw[fill = black](-1,0.5) circle (0.07cm);
\draw[fill = black](1,0.5) circle (0.07cm);
\end{tikzpicture}$$

Abbiamo quindi che la nostra funzione è positiva negli intervalli $$x < -2 \cup -\sqrt{2} \leq x \leq \sqrt{2} \cup x > 2$$. Abbiamo inoltre trovato anche le intersezioni con l'asse $$x$$: sono infatti quei punti in cui la frazione si annulla, ossia $$x = \pm \sqrt{2}$$. Aggiorniamo il nostro grafico con queste nuove informazioni. Indico sempre con il grigio le zone in cui la funzione "non c'è"; i pallini rossi sull'asse delle $$x$$ indicano le intersezioni (i punti in cui la funzione è zero), ossia i punti $$x = \pm \sqrt{2}$$ nel nostro caso. 

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
%\addplot[red,domain=-6:6,semithick]{exp(x)};
%\addplot[black]{x+1};
\fill[grey!10]
(axis cs:-1,-6) --
(axis cs:1,-6) --
(axis cs:1,6) --
(axis cs:-1,6) --
cycle;
\fill[grey!10]
(axis cs:-10,-6) --
(axis cs:-2,-6) --
(axis cs:-2,0) --
(axis cs:-10,0) --
cycle;
\fill[grey!10]
(axis cs:-2,0) --
(axis cs:-1.414313,0) --
(axis cs:-1.414313,6) --
(axis cs:-2,6) --
cycle;
\fill[grey!10]
(axis cs:-1.414313,-6) --
(axis cs:-1,-6) --
(axis cs:-1,0) --
(axis cs:-1.414313,0) --
cycle;
\fill[grey!10]
(axis cs:2,0) --
(axis cs:1.414313,0) --
(axis cs:1.414313,6) --
(axis cs:2,6) --
cycle;
\fill[grey!10]
(axis cs:1.414313,-6) --
(axis cs:1,-6) --
(axis cs:1,0) --
(axis cs:1.414313,0) --
cycle;
\fill[grey!10]
(axis cs:10,-6) --
(axis cs:2,-6) --
(axis cs:2,0) --
(axis cs:10,0) --
cycle;
\addplot[black,dashed] coordinates {
(-1,-6)
(-1,6)
};
\addplot[black,dashed] coordinates {
(1,-6)
(1,6)
};
\addplot[black,dashed] coordinates {
(-2,-6)
(-2,6)
};
\addplot[black,dashed] coordinates {
(2,-6)
(2,6)
};
\addplot[red, mark=*, only marks] coordinates {(-1.414213,0) (1.414213,0)};
%\addplot[] coordinates {(1,1.5)} node{$y=x+1$};
%\addplot[red] coordinates {(-1,0.6)} node{$y=e^x$};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\end{axis}
\end{tikzpicture}$$

### STEP 4

Andiamo a vedere i limiti agli estremi del nostro dominio. 

$$\lim_{x \rightarrow +\infty} \frac{\ln(x^2-1)}{x^2-4} = "\frac{\infty}{\infty}"$$

Per risolvere la forma indeterminata possiamo procedere in due modi. Il primo è quello di ragionare sugli asintotici. Infatti il numeratore a più infinito si comporta come $$\ln(x^2)$$ mentre il denominatore come $$x^2$$. Quindi 

$$\frac{\ln(x^2-1)}{x^2-4} \sim \frac{\ln(x^2)}{x^2} \longrightarrow 0$$

poichè sappiamo che il logaritmo tende a infinito più lentamente di $$x$$. Ricordiamo infatti che per $$\mathbf{x \rightarrow + \infty}$$ l'ordine di infiniti è

$$\log_a(x) << x^b << c^x << x^x$$

con $$a>0,a\neq 1, b>0, c >1$$.

La seconda alternativa è quella di applicare il teorema di De l'Hopital e ottenere 

$$\begin{align*}
\lim_{x \rightarrow +\infty} \frac{\ln(x^2-1)}{x^2-4} &  = \lim_{x \rightarrow +\infty} \frac{\frac{1}{x^2-1} \cdot 2x}{2x} \\
& = \lim_{x \rightarrow +\infty} \frac{1}{x^2-1} \\
& = "\frac{1}{+\infty}" \\
& = 0
\end{align*}$$

Attenzione a usare questo metodo: si usa solo se ho forme indeterminate $$\frac{0}{0}, \frac{\infty}{\infty}$$ e SE so fare bene le derivate. 

Abbiamo quindi ottenuto che la funzione va a zero per $$x\rightarrow + \infty$$. Poichè abbiamo stabilito che la funzione è pari, ossia simmetrica rispetto l'asse $$y$$ ho che anche il limite per $$x \rightarrow -\infty$$ è zero. Passiamo ora ai limiti degli asintoti verticali. 

$$\lim_{x \rightarrow 2^+} \frac{\ln(x^2-1)}{x^2-4} = "\frac{\ln(3^+)}{0^+}" = +\infty$$

poichè sia a numeratore che a denominatore ho numeri positivi. 

$$\lim_{x \rightarrow 2^-} \frac{\ln(x^2-1)}{x^2-4} = "\frac{\ln(3^-)}{0^-}" = -\infty$$

poichè a numeratore ho un numero positivo mentre a denominatore ho un numero negativo. 

$$\lim_{x \rightarrow 1^+} \frac{\ln(x^2-1)}{x^2-4} = "\frac{\ln(0^+)}{-3^+}" = +\infty$$

poichè sia numeratore che denominatore sono negativi. 

Come già detto, poichè la funzione è pari abbiamo in automatico anche i limiti a -2 e -1. Riportiamo sul grafico quello che abbiamo trovato. Disegno in rosso la funzione. 

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
(axis cs:-1,-6) --
(axis cs:1,-6) --
(axis cs:1,6) --
(axis cs:-1,6) --
cycle;
\fill[grey!10]
(axis cs:-10,-6) --
(axis cs:-2,-6) --
(axis cs:-2,0) --
(axis cs:-10,0) --
cycle;
\fill[grey!10]
(axis cs:-2,0) --
(axis cs:-1.414313,0) --
(axis cs:-1.414313,6) --
(axis cs:-2,6) --
cycle;
\fill[grey!10]
(axis cs:-1.414313,-6) --
(axis cs:-1,-6) --
(axis cs:-1,0) --
(axis cs:-1.414313,0) --
cycle;
\fill[grey!10]
(axis cs:2,0) --
(axis cs:1.414313,0) --
(axis cs:1.414313,6) --
(axis cs:2,6) --
cycle;
\fill[grey!10]
(axis cs:1.414313,-6) --
(axis cs:1,-6) --
(axis cs:1,0) --
(axis cs:1.414313,0) --
cycle;
\fill[grey!10]
(axis cs:10,-6) --
(axis cs:2,-6) --
(axis cs:2,0) --
(axis cs:10,0) --
cycle;
\addplot[black,dashed] coordinates {
(-1,-6)
(-1,6)
};
\addplot[black,dashed] coordinates {
(1,-6)
(1,6)
};
\addplot[black,dashed] coordinates {
(-2,-6)
(-2,6)
};
\addplot[black,dashed] coordinates {
(2,-6)
(2,6)
};
\addplot[red, mark=*, only marks] coordinates {(-1.414213,0) (1.414213,0)};
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\addplot[red,domain=-6:-5,semithick]{ln(x^2-1)/(x^2-4)};
\addplot[red,domain=-2.07:-2,semithick]{ln(x^2-1)/(x^2-4)};
\addplot[red,domain=2:2.07,semithick]{ln(x^2-1)/(x^2-4)};
\addplot[red,domain=5:6,semithick]{ln(x^2-1)/(x^2-4)};
\addplot[red] coordinates {
(-1.1,5)
(-1.1,6)
};
\addplot[red] coordinates {
(-1.9,-5)
(-1.9,-6)
};
\addplot[red] coordinates {
(1.1,5)
(1.1,6)
};
\addplot[red] coordinates {
(1.9,-5)
(1.9,-6)
};
\end{axis}
\end{tikzpicture}$$

### STEP 5 

Calcoliamo la derivata prima: è una frazione, quindi applichiamo la formula della derivata di $$\frac{f(x)}{g(x)}$$: indico con $$D$$ o $$'$$ il simbolo di derivata.

$$\begin{align*}
y^{'} & = \frac{D(\ln(x^2-1))\cdot (x^2-4) - \ln(x^2-1) \cdot D(x^2-4)}{(x^2-4)^2} \\
& = \frac{\frac{1}{x^2-1}\cdot 2x(x^2-4)-\ln(x^2-1)\cdot 2x}{(x^2-4)^2} \\
& = \frac{2x \cdot \left( \frac{x^2-4}{x^2-1} - \ln(x^2-1)\right)}{(x^2-4)^2}
\end{align*}$$

Dovrei ora studiare il segno della derivata prima, ossia quando $$y^{'} \geq 0 $$. Dal momento che il denominatore è sempre positivo (è un quadrato, quindi è sempre positivo), chiedersi quando $$y^{'} \geq 0$$ equivale a chiedersi quando il numeratore è maggiore o uguale a zero. Studio quindi 

$$2x \cdot \left( \frac{x^2-4}{x^2-1} - \ln(x^2-1)\right) \geq 0$$

Visto che ho un prodotto, studio singolarmente i due fattori. 

Fattore 1: $$2x \geq 0 \Rightarrow x \geq 0$$

Fattore 2: $$\frac{x^2-4}{x^2-1} - \ln(x^2-1) \geq 0$$

Questo secondo fattore è un po' più complicato: bisognerebbe fare uno studio di funzione separatamente per le due funzioni, uno per $$\frac{x^2-4}{x^2-1}$$ e uno per $$\ln(x^2-1)$$. Per questo motivo nella descrizione dell'esercizio ho messo "incompleto": l'esercizio è volutamente difficile (tradotto: molto difficilmente in verifica potrebbe capitare da studiare una derivata così) e serve per far vedere i passaggi chiavi di uno studio di funzioni e offrire spunti vista la presenza di frazioni e logaritmi. Per questo non scrivo gli studi singoli delle due funzioni, ma se vi volete cimentare, visto che non sono difficili da studiare singolarmente, vi metto qui i grafici finali.

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=120,
	width=9.0cm,height=6.4cm,
	xmin=-6, xmax=6,
	ymin=-6.5, ymax=6.5,
	restrict y to domain=-8:8,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\addplot[red,domain=-6:6,semithick]{(x^2-4)/(x^2-1)};
\addplot[black, dashed,domain=-6:6,semithick]{1};
\addplot[black,dashed] coordinates {
(-1,-8)
(-1,8)
};
\addplot[black,dashed] coordinates {
(1,-8)
(1,8)
};
\addplot[] coordinates {(1.2,-0.5)} node{$1$};
\addplot[] coordinates {(-1,-0.5)} node{$-1$};
\addplot[] coordinates {(-0.3,1)} node{$1$};
\addplot[red] coordinates {(-4,4)} node{$\frac{x^2-4}{x^2-1}$};
\end{axis}
\end{tikzpicture}$$

***

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=1500,
	width=9.0cm,height=6.4cm,
	xmin=-6, xmax=6,
	ymin=-4, ymax=4,
	restrict y to domain=-8:8,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\addplot[red,domain=-5:5,semithick]{ln(x^2-1)};
\addplot[black,dashed] coordinates {
(-1,-8)
(-1,8)
};
\addplot[black,dashed] coordinates {
(1,-8)
(1,8)
};
\addplot[] coordinates {(1.2,-0.5)} node{$1$};
\addplot[] coordinates {(-1,-0.5)} node{$-1$};
\addplot[red] coordinates {(-4,4)} node{$\ln(x^2-1)$};
\end{axis}
\end{tikzpicture}$$

***

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=1500,
	width=9.0cm,height=6.4cm,
	xmin=-8, xmax=8,
	ymin=-6, ymax=3,
	restrict y to domain=-8:8,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\addplot[red,domain=-7:7,semithick]{(x^2-4)/(x^2-1) -ln(x^2-1)};
\addplot[black,dashed] coordinates {
(-1,-8)
(-1,8)
};
\addplot[black,dashed] coordinates {
(1,-8)
(1,8)
};
\addplot[] coordinates {(1.2,-0.5)} node{$1$};
\addplot[] coordinates {(-1,-0.5)} node{$-1$};
\addplot[red] coordinates {(-4.5,2)} node{$\frac{x^2-4}{x^2-1}-\ln(x^2-1)$};
\end{axis}
\end{tikzpicture}$$

Come si può vedere in quest'ultimo grafico, se definisco $$g(x):= \frac{x^2-4}{x^2-1}-\ln(x^2-1)$$, allora ho che $$g(x)$$ è sempre negativa: infatti sta sempre sotto l'asse delle $$x$$, ossia assume sempre valori ($$y$$) negativi. Questo significa che il Fattore 2 della mia derivata prima è sempre nativo. Il castello dei segni diventa quindi

$$\begin{tikzpicture}
\draw (-2,0) -- (2,0);
\draw (0,3) -- (0,-0.2);
\node at (0,-0.5) {$0$};
\draw (-2,2) -- (2,2);
\draw (-2,1) -- (2,1);
%Numeratore
\node at (-3.3,2.5) {\scriptsize Fattore 1:};
\node at (-1,2.5) {$-$};
\node at (1,2.5) {$+$};
\draw [fill = black](0,2.5) circle (0.07cm);
%Denominatore
\node at (-3.3,1.5) {\scriptsize Fattore 2:};
\node at (-1,1.5) {$-$};
\node at (1,1.5) {$-$};
%Frazione
\node at (-3.3,0.5) {\scriptsize Prodotto:};
\node at (-1,0.5) {$+$};
\node at (1,0.5) {$-$};
\draw [fill = black](0,0.5) circle (0.07cm);
\draw[->] (-1.8,-1) -- (-0.3,-0.5);
\draw[<-] (1.8,-1) -- (0.3,-0.5);
\end{tikzpicture}$$

La funzione è quindi crescente nell'intervallo $$(-\infty,0)$$ mentre è descrescente in $$(0,+\infty)$$. Sembrerebbe che $$0$$ sia un punto di massimo, ma zero è escluso dal dominio della funzione: essa quindi non ha nè massimi nè minimi. 

### STEP 6

Calcoliamo la derivata seconda.

$$\begin{align*}
y^{''} & = \frac{D\left( 2x\left(\frac{x^2-4}{x^2-1}-\ln(x^2-1)\right) \right)(x^2-4)^2 - \left(2x\left(\frac{x^2-4}{x^2-1}-\ln(x^2-1)\right)\right)D((x^2-4)^2)}{(x^2-4)^4} \\
& = \frac{D\left( 2x\left(\frac{x^2-4}{x^2-1}-\ln(x^2-1)\right) \right)(x^2-4)^2}{(x^2-4)^4} - \frac{\left(2x\left(\frac{x^2-4}{x^2-1}-\ln(x^2-1)\right)\right)D((x^2-4)^2)}{(x^2-4)^4} \\
& = \frac{\left( 2\left(\frac{x^2-4}{x^2-1}-\ln(x^2-1)\right)+2x\left(\frac{2x(x^2-1)-(x^2-4)2x}{(x^2-1)^2}- \frac{2x}{x^2-1}\right) \right)(x^2-4)^2}{(x^2-4)^4} + \\
& - \frac{\left(2x\left(\frac{x^2-4}{x^2-1}-\ln(x^2-1)\right)\right)2(x^2-4)2x}{(x^2-4)^4}
\end{align*}$$

Sistemare questa derivata seconda è fattibile, ma da pazzi, come già ci si poteva aspettare dalla derivata prima. Ci fermiamo quindi qui con lo studio, collegando tutti i pezzi di grafico già disegnati finora e ottenendo il grafico della funzione. 

$$\begin{tikzpicture}[scale=1.0544]\small
\begin{axis}[axis line style=gray,
	samples=2000,
	width=9.0cm,height=6.4cm,
	xmin=-6, xmax=6,
	ymin=-2, ymax=2,
	restrict y to domain=-8:8,
	ytick=none,
	xtick=none
	axis equal,
	axis x line=center,
	axis y line=center,
	xlabel=$x$,ylabel=$y$]
\path (axis cs:0,0) node [anchor=north west,yshift=-0.07cm] {0};
\addplot[red,domain=-5.5:5.5,semithick]{ln(x^2-1.2)/(x^2-4)};
\addplot[black,dashed] coordinates {
(-1,-2)
(-1,2)
};
\addplot[black,dashed] coordinates {
(-2,-2)
(-2,2)
};
\addplot[black,dashed] coordinates {
(1,-2)
(1,2)
};
\addplot[black,dashed] coordinates {
(2,-2)
(2,2)
};
\addplot[] coordinates {(1.2,-0.3)} node{$1$};
\addplot[] coordinates {(-1,-0.3)} node{$-1$};
\addplot[] coordinates {(2.2,-0.3)} node{$2$};
\addplot[] coordinates {(-2.05,-0.3)} node{$-2$};
\addplot[red] coordinates {(-3.8,1)} node{$\frac{\ln(x^2-1)}{x^2-4}$};
\end{axis}
\end{tikzpicture}$$











