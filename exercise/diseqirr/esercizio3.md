# DISEQUAZIONI IRRAZIONALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Risolvi la seguente disequazione irrazionale

$$1 > \sqrt{x^2-2x}-x$$

## Soluzione:

Come prima cosa dobbiamo "sistemare" la disequazione in modo da arrivare a una forma del tipo $$\sqrt{A(x)} \gtrless B(x)$$:

$$\begin{align*}
1 & > \sqrt{x^2-2x}-x \\
-\sqrt{x^2-2x} & > -1-x \\
(-1) \cdot -\sqrt{x^2-2x} & > (-1-x) \cdot (-1) \\
\sqrt{x^2-2x} & \; \textcolor{red}{<} \; x+1
\end{align*}$$

dove ho evidenziato in rosso il cambio di verso poichè ho moltiplicato tutto per un numero negativo. 

Possiamo ora applicare la formula. Siamo nel caso di indice di radice pari (uguale a $$2$$) con disequazione del tipo $$\sqrt{A(x)} < B(x)$$. Formula ci dice che la disuguaglianza è equivalente a risolvere 

$$\begin{cases}
A(x) \geq 0 \\
B(x) > 0 \\
A(x) < [B(x)]^2 
\end{cases}
\end{cases}$$

dove, nel nostro caso, $$A(x) = x^2-2x$$ e $$B(x) = x+1$$.

Il sistema diventa quindi 

$$\begin{cases}
x^2-2x \geq 0 \\
x+1 > 0 \\
x^2-2x < \left(x+1\right)^2 
\end{cases}$$

Partiamo con la risoluzione della prima disequazione.

$$x^2-2x \geq 0$$

Vediamo subito che si tratta di una disequazione di secondo grado. Ricordiamo come si risolvono. 

<hr>

**Memo**: Ricordiamo la regola in generale che ci dice. Se ho

1. espressione del tipo $$ax^2+bx+c \gtrless 0$$
1. $$\textbf{a}>0$$
1. delta positivo: $$\Delta > 0$$
1. $$x_1,x_2$$ soluzioni dell'equazione associata con $$x_2 < x_1$$

Allora $$ax^2+bx+c > 0$$ ha soluzione $$x < x_2 \cup x > x_1$$, mentre $$ax^2+bx+c < 0$$ ha soluzione $$x_2 < x < x_1$$. A parole, se voglio l'espressione positiva devo prendere l'unione degli intervalli esterni ai due valori che ottengo nell'equazione associata. Se invece voglio l'espressione negativa, devo prendere l'intervallo interno. In entrambi i casi, escludo o includo i punti estremi se la disuguaglianza è stretta oppure no.   

<hr>

Andiamo quindi a risolvere la nostra:

$$\begin{align*}
x^2-2x & \; \textcolor{red}{\geq} \;  0\\
& \downarrow \\
\text{equazione} & \; \text{associata:} \\
x^2-2x & = 0 \\
x(x-2) & = 0 \\
& \downarrow \\
x = 0 & \vee x-2 = 0 \\
x = 0 & \vee x = 2 \\
\text{poichè avevo} \; \textcolor{red}{\geq} \; & \rightarrow \text{intervalli esterni:} \\
x \leq 0 & \; \vee x \geq 2
\end{align*}$$

La soluzione della prima disequazione del sistema è quindi 

$$x \leq 0 \; \vee \; x \geq 2$$

Passiamo a risolvere la seconda disequazione del sistema.

$$\begin{align*}
x+1 > 0 \\
x > -1
\end{align*}$$

Infine, andiamo a risolvere la terza disequazione del sistema. 

$$\begin{align*}
x^2-2x & < \left(x+1\right)^2 \\
x^2-2x & < x^2+2x+1 \\
x^2-2x-x^2-2x-1 & < 0 \\
-4x-1 & < 0 \\
-4x & < 1 \\
\frac{-4x}{-4} & < \frac{1}{-4} \\
x & \; \textcolor{red}{>} \; -\frac{1}{4}
\end{align*}$$

dove ho evidenziato in rosso il cambio di verso in quanto ho diviso per un numero negativo.

Possiamo ora riprendere in mano il sistema di partenza.

$$\begin{align*}
& \begin{cases}
x^2-2x \geq 0 \\
x+1 > 0 \\
x^2-2x < \left(x+1\right)^2 
\end{cases} \\
& \begin{cases}
x \leq 0 \vee x \geq 2 \\
x > -1 \\
x > -\frac{1}{4} 
\end{cases} \\
\end{align*}$$

$$\begin{tikzpicture}
\draw[fill=yellow] (-0.25,3) rectangle (0.5,0);
\draw[fill=yellow] (2,3) rectangle (3,0);
\draw (-2,0)--(3,0);
\draw (-1,-0.2)--(-1,3);
\draw (-0.25,-0.2)--(-0.25,3);
\draw (0.5,-0.2)--(0.5,3);
\draw (2,-0.2)--(2,3);
\node at (-0.25,-0.5) {$-\frac{1}{4}$};
\node at (-1,-0.5) {$-1$};
\node at (0.5,-0.5) {$0$};
\node at (2,-0.5) {$2$};
\node at (-3,0.5) {\scriptsize $x > -\frac{1}{4}$};
\node at (-3,1.5) {\scriptsize $x > -1$};
\node at (-3.5,2.5) {\scriptsize $x \leq 0 \vee x \geq 2$};
\draw (0.5,2.5) -- (-2,2.5);
\draw (2,2.5) -- (3,2.5);
\draw (-1,1.5) -- (3,1.5);
\draw (-0.25,0.5) -- (3,0.5);
\draw[fill=black] (0.5,2.5) circle (0.07);
\draw[fill=black] (2,2.5) circle (0.07);
\draw[fill=white] (-1,1.5) circle (0.07);
\draw[fill=white] (-0.25,0.5) circle (0.07);
\end{tikzpicture}$$

La soluzione del sistema è data dagli intervalli in cui compaiono tutte e tre le soluzioni contemporaneamente: nel nostro caso ci sono due intervalli che soddisfano questa condizione (in giallo nel grafico). La disequazione di partenza ha quindi soluzione:

$$-\frac{1}{4} < x \leq 0 \; \vee \; x \geq 2$$

Nota su come costruire il grafico: in ogni riga disegno la soluzione che ho trovato tramite una linea continua, facendo attenzione a includere o no gli estremi. Con i pallini neri indico che l'estremo è incluso, mentre con i pallini bianchi che è escluso. 

**SUPER ATTENZIONE**: quando la soluzione di una disequazione è l'unione di due intervalli (come nel nostro caso, la prima disequazione), questi due intervalli vanno disegnati **nella stessa riga**, così come abbiamo fatto con $$x \leq 0 \vee x \geq 2$$. 
