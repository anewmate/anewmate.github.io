# DISEQUAZIONI IRRAZIONALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Risolvi la seguente disequazione irrazionale

$$x \leq -1 + \sqrt{1+2x}$$

## Soluzione:

Come prima cosa dobbiamo "sistemare" la disequazione in modo da arrivare a una forma del tipo $$\sqrt{A(x)} \gtrless B(x)$$:

$$\begin{align*}
x & \leq -1 + \sqrt{1+2x} \\
-\sqrt{1+2x} & \leq -1-x \\
(-1) \cdot -\sqrt{1+2x} & \leq (-1-x) \cdot (-1) \\
\sqrt{1+2x} & \; \textcolor{red}{\geq} \; x+1
\end{align*}$$

dove ho evidenziato in rosso il cambio di verso poichè ho moltiplicato tutto per un numero negativo. 

Possiamo ora applicare la formula. Siamo nel caso di indice di radice pari (uguale a $$2$$) con disequazione del tipo $$\sqrt{A(x)} \geq B(x)$$. Formula ci dice che la disuguaglianza è equivalente a risolvere 

$$\begin{align*}
 \begin{cases}
B(x) \geq 0 \\
A(x) \geq [B(x)]^2 
\end{cases} 
\vee \qquad \begin{cases}
A(x) \geq 0 \\
B(x) < 0
\end{cases}
\end{align*}$$

dove, nel nostro caso, $$A(x) = 1+2x$$ e $$B(x) = x+1$$.

I sistemi diventano quindi 

$$\begin{align*}
 \begin{cases}
x+1 \geq 0 \\
1+2x \geq (x+1)^2 
\end{cases} 
\vee \qquad \begin{cases}
1+2x \geq 0 \\
x+1 < 0
\end{cases}
\end{align*}$$

Partiamo con la risoluzione del primo sistema.

$$\begin{align*}
& \begin{cases}
x+1 \geq 0 \\
1+2x \geq (x+1)^2 
\end{cases} \\
&  \begin{cases}
x \geq -1 \\
1+2x \geq x^2+2x+1 
\end{cases} \\
& \begin{cases}
x \geq -1 \\
1+2x-x^2-2x -1\geq 0   
\end{cases} \\
&  \begin{cases}
x\geq -1\\
-x^2 \geq 0 
\end{cases} \\
&  \begin{cases}
x\geq -1\\
(-1) \cdot (-x^2) \geq 0 \cdot (-1)  
\end{cases} \\
&  \begin{cases}
x\geq -1\\
x^2 \leq 0 
\end{cases} \\
&  \begin{cases}
x\geq -1\\
x = 0 
\end{cases}
\end{align*}$$

Prima di vedere la soluzione di tutto il sistema, ricordiamo perchè $$x^2 \leq 0$$ ha soluzione $$x = 0$$: in generale, 

1. $$(*(x))^2 \geq 0 \rightarrow \forall \; x \in \mathbb{R}$$
1. $$(*(x))^2 > 0 \rightarrow  *(x) \neq 0 $$
1. $$(*(x))^2 \leq 0 \rightarrow *(x) = 0 $$ 
1. $$(*(x))^2 < 0 \rightarrow \nexists \; x \in \mathbb{R}$$ 

dove $$*(x)$$ è qualsiasi cosa scritta in funzione di $$x$$. Nel nostro caso $$*(x)$$ è $$x$$ e ricadiamo nel caso 3.

Risolviamo ora il sistema:

$$\begin{cases}
x\geq -1\\
x = 0 
\end{cases}$$

$$\begin{tikzpicture}
%\draw[fill=yellow] (-0.1,2) rectangle (0.1,0);
\draw[yellow,ultra thick] (0,-0.2)--(0,2);
\draw (-2,0)--(2,0);
\draw (-1,-0.2)--(-1,2);
\draw[line width=0.07mm] (0,-0.2)--(0,2);
\node at (-1,-0.5) {$-1$};
\node at (0,-0.5) {$0$};
\node at (-3,0.5) {\scriptsize $x = 0$};
\node at (-3,1.5) {\scriptsize $x \geq -1$};
\draw (-1,1.5) -- (2,1.5);
\draw[fill=black] (-1,1.5) circle (0.07);
\draw[fill=black] (0,0.5) circle (0.07);
\end{tikzpicture}$$

In ogni riga disegno la soluzione che ho trovato tramite una linea continua, facendo attenzione a includere o no gli estremi. Con i pallini neri indico che gli estremi sono inclusi. Ovviamente $$x=0$$ è solo un punto, corrispondente al numero $$0$$. 

La soluzione (in giallo nel grafico) è data dagli intervalli in cui compaiono tutte e due le soluzioni contemporaneamente: nel nostro caso visto che $$x=0$$ è contenuto in $$x \geq -1$$, sarà anche la soluzione di tutto il sistema. 

Passiamo a risolvere il secondo sistema.  

$$\begin{align*}
& \begin{cases}
1+2x \geq 0 \\
x+1 < 0
\end{cases} \\
& \begin{cases}
2x \geq -1 \\
x < -1
\end{cases} \\
& \begin{cases}
\frac{2x}{2} \geq \frac{-1}{2} \\
x < -1
\end{cases} \\
& \begin{cases}
x \geq -\frac{1}{2} \\
x < -1
\end{cases}
\end{align*}$$

$$\begin{tikzpicture}
%\draw[fill=yellow] (-0.1,2) rectangle (0.1,0);
%\draw[yellow,ultra thick] (0,-0.2)--(0,2);
\draw (-2.5,0)--(2,0);
\draw (-1,-0.2)--(-1,2);
\draw (0,-0.2)--(0,2);
\node at (-1,-0.5) {$-1$};
\node at (0,-0.5) {$-\frac{1}{2}$};
\node at (-3.5,0.5) {\scriptsize $x < -1$};
\node at (-3.5,1.5) {\scriptsize $x \geq -\frac{1}{2}$};
\draw (0,1.5) -- (2,1.5);
\draw (-1,0.5) -- (-2.5,0.5);
\draw[fill=black] (0,1.5) circle (0.07);
\draw[fill=white] (-1,0.5) circle (0.07);
\end{tikzpicture}$$

In questo caso non esiste nessun intervallo in cui contemporaneamente ci sono entrambe le soluzioni: il sistema è quindi impossibile, ossia non ha soluzione. Di solito ciò viene indicato con l'insieme vuoto:

$$\emptyset $$

Possiamo quindi riprendere in mano la soluzione totale:

$$\begin{align*}
 \begin{cases}
x+1 \geq 0 \\
1+2x \geq (x+1)^2 
\end{cases} 
& \vee \qquad \begin{cases}
1+2x \geq 0 \\
x+1 < 0
\end{cases} \\
\text{Soluzione sistema 1:}\qquad & \qquad \text{Soluzione sistema 2:} \\
x= 0 \qquad & \vee \qquad \emptyset
\end{align*}$$

Cosa dobbiamo fare con le due soluzioni che abbiamo trovato? Quel simbolo che sta in mezzo ai due sistemi ($$\vee$$) equivale a una "o", nel senso che ci vanno bene tutte e due le soluzioni: dobbiamo quindi prendere l'unione delle due soluzioni che troviamo. La soluzione finale del nostro esercizio è quindi 

$$x = 0 $$

**Memo**: l'insieme vuoto unito a qualsiasi cosa mi restituisce sempre la stessa cosa: 

$$\emptyset \; \vee \; * \; = \; *$$

dove $$*$$ è qualsiasi cosa. 

