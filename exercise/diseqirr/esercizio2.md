# DISEQUAZIONI IRRAZIONALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente disequazione irrazionale

$$2\sqrt{1-x+x^2} < 1-2x$$

## Soluzione:

Come prima cosa notiamo che la disequazione è già scritta *quasi* "bene", nel senso che vogliamo arrivare ad avere a sinistra della disuguaglianza solo il termine con la radice e a destra della disuguaglianza tutto il resto. Per avere solo la radice a sinistra, devo quindi dividere tutto per $$2$$:

$$\begin{align*}
2\sqrt{1-x+x^2} & < 1-2x \\
\frac{2\sqrt{1-x+x^2}}{2} & < \frac{1-2x}{2} \\
\sqrt{1-x+x^2} & < \frac{1-2x}{2}
\end{align*}$$

Possiamo ora applicare la formula. Siamo nel caso di indice di radice pari (uguale a $$2$$) con disequazione del tipo $$\sqrt{A(x)} < B(x)$$. Formula ci dice che la disuguaglianza è equivalente a risolvere 

$$\begin{cases}
A(x) \geq 0 \\
B(x) > 0 \\
A(x) < [B(x)]^2 
\end{cases}
\end{cases}$$

dove, nel nostro caso, $$A(x) = 1-x+x^2$$ e $$B(x) = \frac{1-2x}{2}$$.

Il sistema diventa quindi 

$$\begin{cases}
1-x+x^2 \geq 0 \\
\frac{1-2x}{2} > 0 \\
1-x+x^2 < \left(\frac{1-2x}{2}\right)^2 
\end{cases}
\end{cases}$$

Partiamo con la risoluzione della prima disequazione.

$$x^2-x+1 \geq 0$$

Vediamo subito che si tratta di una disequazione di secondo grado. Ricordiamo come si risolvono. 

<hr>

**Memo**: Ricordiamo la regola in generale che ci dice. Se ho

1. espressione del tipo $$ax^2+bx+c \gtrless 0$$
1. $$\textbf{a}>0$$
1. delta positivo: $$\Delta > 0$$
1. $$x_1,x_2$$ soluzioni dell'equazione associata con $$x_2 < x_1$$

Allora $$ax^2+bx+c > 0$$ ha soluzione $$x < x_2 \cup x > x_1$$, mentre $$ax^2+bx+c < 0$$ ha soluzione $$x_2 < x < x_1$$. A parole, se voglio l'espressione positiva devo prendere l'unione degli intervalli esterni ai due valori che ottengo nell'equazione associata. Se invece voglio l'espressione negativa, devo prendere l'intervallo interno. In entrambi i casi, escludo o includo i punti estremi se la disuguaglianza è stretta oppure no.  

**Memo**: Ricordiamo la regola in generale che ci dice. Se ho

1. espressione del tipo $$ax^2+bx+c \gtrless 0$$
1. $$\textbf{a}>0$$
1. delta negativo: $$\Delta < 0$$

Allora $$ax^2+bx+c > 0$$ ha soluzione $$\forall \; x \in \mathbb{R}$$, mentre $$ax^2+bx+c < 0$$ ha soluzione $$\nexists \; x \in \mathbb{R}$$. A parole, se $$a > 0$$ e delta è negativo, l'espressione $$ax^2+bx+c$$ è sempre positiva: quindi la disuguaglianza con il maggiore è sempre verificata mentre non lo è mai quella con il minore. 

<hr>

Andiamo quindi a risolvere la nostra:

$$\begin{align*}
x^2-x+1 & \geq 0 \\
& \downarrow \\
\text{equazione} & \; \text{associata:} \\
x^2-x+1 & = 0 \\
x_{1/2} & = \frac{-b\pm \sqrt{b^2-4ac}}{2a} \\
& = \frac{-(-1) \pm \sqrt{1-4(1)(1)}}{2(1)} \\
& = \frac{+1 \pm \sqrt{-3}}{2} \\
\end{align*}$$

Abbiamo ottenuto un delta negativo: $$\Delta = -3$$. Secondo le regole ricordate prima, la disequazione è sempre verificata e ha quindi come soluzione 

$$\forall \; x \in \mathbb{R}$$

Passiamo a risolvere la seconda disequazione del sistema.

$$\begin{align*}
\frac{1-2x}{2} & > 0 \\
2 \cdot \frac{1-2x}{2} & > 0 \cdot 2 \\
1-2x & > 0 \\
-2x & > -1 \\
\text{moltiplico destra e sinistra }& \downarrow  \text{per $-1$ cambiando il verso}\\
2x & < 1 \\
\frac{2x}{2} & < \frac{1}{2} \\
x & < \frac{1}{2}
\end{align*}$$

Infine, andiamo a risolvere la terza disequazione del sistema. 

$$\begin{align*}
1-x+x^2 & < \left(\frac{1-2x}{2}\right)^2  \\
1-x+x^2 & < \frac{(1-2x)^2}{4} \\
4 \cdot (1-x+x^2) & < \frac{(1-2x)^2}{4} \cdot 4 \\
4-4x+4x^2 & < 1-4x+4x^2 \\
4-4x+4x^2-1+4x-4x^2 & < 0 \\
3 & < 0 
\end{align*}$$

Abbiamo quindi ottenuto una disuguaglianza palesemente falsa: $$3$$ **non** è minore di zero. Ciò vuol dire che la disequazione che stavamo provando a risolvere non ha soluzione:

$$\nexists \; x \in \mathbb{R}$$

Possiamo ora riprendere in mano il sistema di partenza.

$$\begin{align*}
& \begin{cases}
1-x+x^2 \geq 0 \\
\frac{1-2x}{2} > 0 \\
1-x+x^2 < \left(\frac{1-2x}{2}\right)^2 
\end{cases} \\
& \begin{cases}
\forall \; x \in \mathbb{R} \\
x < \frac{1}{2} \\
\nexists \; x \in \mathbb{R} 
\end{cases} \\
\end{align*}$$

$$\begin{tikzpicture}
%\draw[fill=yellow] (-1,2) rectangle (1,0);
\draw (-2,0)--(2,0);
\draw (0,-0.2)--(0,3);
\node at (0,-0.5) {$\frac{1}{2}$};
\node at (-3,0.5) {\scriptsize $\nexists \; x \in \mathbb{R}$};
\node at (-3,1.5) {\scriptsize $x < \frac{1}{2}$};
\node at (-3,2.5) {\scriptsize $\forall \; x \in \mathbb{R}$};
\draw (0,1.5) circle (0.07);
\draw (0,1.5) -- (-2,1.5);
\draw (-2,2.5) -- (2,2.5);
\end{tikzpicture}$$

La soluzione del sistema è data dagli intervalli in cui compaiono tutte e tre le soluzioni contemporanemente: nel nostro caso non c'è nessun intervallo in cui ciò succede. La disequazione di partenza non ha quindi soluzione:

$$\nexists \; x \in \mathbb{R}$$

<hr>

**Memo**: quando in un sistema di disequazioni/equazioni una soluzione di almeno una delle disequazioni/equazioni è l'insieme vuoto (ossia $$\nexists \; x \in \mathbb{R}$$), in automatico anche il sistema non ammette soluzioni. 

Ciò deriva dal fatto che mettere a sistema significa intersecare le soluzioni delle disequazioni/equazioni: dalle regole insiemistiche sappiamo che il vuoto intersecato con qualsiasi cosa dà sempre il vuoto. 