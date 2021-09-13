# DISEQUAZIONI CON VALORE ASSOLUTO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Risolvi la seguente disequazione che contiene valori assoluti:

$$|x^2-4| > 4x-8$$

Soluzione: 

Come prima cosa ricordiamo la definizione generale di valore assoluto:

$$\begin{align*}
|\ast(x)| & = \begin{cases}
\ast(x) & \text{se} \ \ast(x) \geq 0 \\
-\ast(x) & \text{se} \ \ast(x) < 0
\end{cases}
\end{align*}
$$

Il valore assoluto è uguale al suo argomento se l'argomento è positivo, mentre è uguale a meno l'argomento, se l'argomento è negativo. 

***
Esempi in breve: 

$$\begin{align*}
|5x+1| & = \begin{cases}
5x+1 & \text{se} \ 5x+1 \geq 0 \\
-5x-1 & \text{se} \ 5x-1 < 0
\end{cases}
\end{align*}
\begin{align*}
|-x^3+2x| & = \begin{cases}
-x^3+2x & \text{se} \ -x^3+2x \geq 0 \\
x^3-2x & \text{se} \ -x^3+2x < 0
\end{cases}
\end{align*}
\begin{align*}
|e^x-2x^2+\sin(x)| & = \begin{cases}
e^x-2x+\sin(x) & \text{se} \ e^x-2x+\sin(x) \geq 0 \\
-e^x+2x-\sin(x) & \text{se} \ e^x-2x+\sin(x) < 0
\end{cases}
\end{align*}
$$

L'ultimo esempio è stato scritto solo per rimarcare il fatto che non importa cosa c'è ad argomento del valore assoluto, sempre così si definsce.
***

Visto che il valore assoluto è definito per casi, il caso in cui l'argomento è positivo e il caso in cui l'argomento è negativo, anche le disequazioni col valore assoluto si risolvono per casi. In particolare, nel nostro esempio il valore assoluto diventa 

$$\begin{align*}
|x^2-4| & = \begin{cases}
x^2-4 & \text{se} \ x^2-4 \geq 0 \\
-x^2+4 & \text{se} \ x^2-4 < 0
\end{cases}
\end{align*}
$$

La disequazione di partenza si divide quindi in due disequazioni, a seconda di come è definito il valore assoluto.
### Caso 1: $$x^2-4 \geq 0 $$ 

Nell'intervallo $$x^2-4 \geq 0$$, il valore assoluto è uguale a $$x^2-4$$. La disequazione quindi diventa 

$$ x^2-4 > 4x-8$$

Porto tutto a sinistra:

$$\begin{align*}
x^2-4x-4+8 & > 0 \\
x^2-4x+4 & > 0 \\
(x-2)^2 & > 0
\end{align*}$$

Quando un quadrato è meggiore di zero? Sempre, ma facendo attenzione che ho il $$>$$ e non il $$\geq$$. Quindi $$(x-2)^2 > 0$$ ha come soluzione $$x-2 \neq 0$$ ossia $$x \neq 2$$. 

ATTENZIONE: la soluzione che ho trovato è definita soltanto nell'intervallo $$x^2-4 \geq 0$$, perchè è qui che stiamo lavorando. Che intervallo è $$x^2-4 \geq 0$$? Ricordando le disequazioni di secondo grado, 

$$\begin{align*}
x^2-4 & \; {\color{red}{\geq}} \;  0 \\
& \downarrow \\
\text{equazione} \; & \; \text{associata:} \\
x^2-4 & = 0 \\
x^2 & = 4 \\
x & = \pm \sqrt{4} \\
x & = \pm 2 \\
& \downarrow  \\
\text{poichè avevo} \; {\color{red}{\geq}} & \rightarrow \text{intervalli esterni:} \\
x \leq -2 & \vee \; x \geq 2 
\end{align*}$$

Devo quindi intersecare la soluzione della disequazione con l'intervallo in cui sto lavorando: 

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (-2,2) rectangle (0,0);
\shade[left color=yellow, right color = yellow] (2,2) rectangle (4,0);
\draw [->](-2,0) -- (4,0);
\draw (0,-0.2) -- (0,0.2);
\node at (0,-0.5) {$-2$};
\node at (2,-0.5) {$2$};
\draw (2,-0.2) -- (2,0.2);
\draw (-2,2) -- (4,2);
\draw [dashed] (2,0) -- (2,2);
\draw[fill = black] (0,1) circle (2pt);
\draw[fill = black] (2,1) circle (2pt);
\draw (-2,1) -- (0,1);
\draw (2,1) -- (4,1);
\draw [dashed] (0,0) -- (0,1);
\draw[fill=white] (2,2) circle (2pt);
\node at (-4,1) {$x \leq -2 \vee x \geq 2$};
\node at (-4,2) {$x \neq 2$};
\end{tikzpicture}
$$

La soluzione del primo caso è quindi 

$$x \leq -2 \; \vee \; x > 2$$

### Caso 2: $$x^2-4 < 0$$ 

Nell'intervallo $$x^2-4 < 0$$, il valore assoluto è uguale a $$-x^2+4$$. La disequazione quindi diventa 

$$ -x^2+4 > 4x-8$$

Porto tutto a sinistra:

$$\begin{align*}
-x^2-4x+4+8 & > 0 \\
-x^2-4x+12 & > 0 \\
(-1) \cdot (-x^2-4x+12) & \;  {\color{red}{<}} \; 0 \cdot (-1) \\
x^2+4x-12 & < 0 
\end{align*}$$

Risolviamo questa disequazione di secondo grado: 

$$\begin{align*}
x^2+4x-12 & \; {\color{red}{<}} \;  0 \\
& \downarrow \\
\text{equazione} \; & \; \text{associata:} \\
x^2+4x-12 & = 0 \\
x_{1/2} & = \frac{-4 \pm \sqrt{16 + 48}}{2} \\
& = \frac{-4 \pm 8}{2}\\
& = \begin{cases}
-6 \\
2
\end{cases}\\
& \downarrow \\
\text{poichè avevo} \; {\color{red}{<}} & \rightarrow \text{intervalli interni:} \\
-6 < & \; x < 2
\end{align*}$$
 

ATTENZIONE: la soluzione che ho trovato è definita soltanto nell'intervallo $$x^2-4 < 0$$, perchè è qui che stiamo lavorando. Che intervallo è $$x^2-4 < 0$$? Ricordando le disequazioni di secondo grado, 

$$\begin{align*}
x^2-4 & \; {\color{red}{<}} \;  0 \\
& \downarrow \\
\text{equazione} \; & \; \text{associata:} \\
x^2-4 & = 0 \\
x^2 & = 4 \\
x & = \pm \sqrt{4} \\
x & = \pm 2 \\
& \downarrow  \\
\text{poichè avevo} \; {\color{red}{<}} & \rightarrow \text{intervalli interni:} \\
 -2 < & \; x < 2 
\end{align*}$$

Devo quindi intersecare la soluzione della disequazione con l'intervallo in cui sto lavorando: 

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (1,2) rectangle (3,0);
\draw [->](-2,0) -- (4,0);
\draw (-1,-0.2) -- (-1,0.2);
\node at (-1,-0.5) {$-6$};
\node at (3,-0.5) {$2$};
\draw (3,-0.2) -- (3,0.2);
\node at (1,-0.5) {$-2$};
\draw (1,-0.2) -- (1,0.2);
\draw (-1,2) -- (3,2);
\draw [dashed] (3,0) -- (3,2);
\draw [dashed] (1,0) -- (1,2);
\draw (3,1) -- (1,1);
\draw [dashed] (-1,2) -- (-1,0);
\draw[fill=white] (3,2) circle (2pt);
\draw[fill = white] (-1,2) circle (2pt);
\draw[fill = white] (3,1) circle (2pt);
\draw[fill = white] (1,1) circle (2pt);
\node at (-4,1) {$-2<x<2$};
\node at (-4,2) {$-6<x<2$};
\end{tikzpicture}
$$

La soluzione del secondo caso è quindi 

$$-2 < x < 2$$

### Totale 
Visto che entrambi i casi hanno soluzioni, la soluzione finale di tutto l'esercizio è data dall'unione delle due soluzioni dei due casi: unendo $$x \leq -2 \vee x >2$$ (in verde nel grafico sotto) con $$-2 < x < 2$$ (in blu nel grafico sotto) ottengo tutti i numeri tranne $$2$$, quindi la soluzione finale è $$x \neq 2$$. 

$$\begin{tikzpicture}
\draw [->](-3,0) -- (3,0);
\draw (-2,-0.2) -- (-2,0.2);
\draw (2,-0.2) -- (2,0.2);
\node at (-2,-0.5) {$-2$};
\node at (2,-0.5) {$2$};
\draw[fill=green] (-2,1) circle (2pt);
\draw[color=green] (-3,1) -- (-2,1); 
\draw[color=green] (2,1) -- (3,1); 
\draw[color=blue] (-2,1) -- (2,1); 
\draw[fill=white] (2,1) circle (2pt);
\end{tikzpicture}
$$

