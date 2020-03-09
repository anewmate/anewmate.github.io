# DISEQUAZIONI CON VALORE ASSOLUTO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente disequazione che contiene valori assoluti:

$$\biggl| -3 + \frac{1}{2}x\biggl| > 2x-\frac{5}{2}$$

Soluzione: 

Come prima cosa ricordiamo la definione generale di valore assoluto:

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
\biggl|-3+\frac{1}{2}x\biggl| & = \begin{cases}
-3+\frac{1}{2}x & \text{se} \ -3+\frac{1}{2}x \geq 0 \\
+3-\frac{1}{2}x & \text{se} \ -3+\frac{1}{2}x < 0
\end{cases}
\end{align*}
$$

La disequazione di partenza si divide quindi in due disequazioni, a seconda di come è definito il valore assoluto.
## Caso 1: $$-3+\frac{1}{2}x\geq 0$$ 

Nell'intervallo $$-3+\frac{1}{2}x\geq 0$$, ossia $$\frac{1}{2}x \geq 3$$, ossia $$x \geq 6$$, il valore assoluto è uguale a $$-3+\frac{1}{2}x$$. La disequazione quindi diventa 

$$ -3 + \frac{1}{2}x > 2x-\frac{5}{2}$$

Porto a sinistra tutti i termini con la $$x$$ e a destra tutti i termini senza:

$$ \frac{1}{2}x -2x > -\frac{5}{2}+3$$

Sommo gli elementi e ottengo 

$$\frac{x-4x}{2} > \frac{-5+6}{2}$$

$$-\frac{3}{2}x > \frac{1}{2}$$

Moltiplico sia a destra che a sinistra per $$-\frac{2}{3}$$ in modo da isolare la $$x$$, ricordandomi di cambiare il verso della disuguaglianza perchè sto moltiplicando per un numero negativo:

$$x < \frac{1}{2} \cdot \left(- \frac{2}{3}\right) \qquad \rightarrow \qquad x < - \frac{1}{3}$$

ATTENZIONE: la soluzione che ho trovato è definita soltanto nell'intervallo $$x \geq 6$$, perchè è qui che stiamo lavorando. Devo quindi intersecare le due cose: 

$$\begin{tikzpicture}
\draw [->](-2,0) -- (8,0);
\draw (-1/3,-0.2) -- (-1/3,0.2);
\node at (-1/3,-0.5) {$-\frac{1}{3}$};
\node at (6,-0.5) {$6$};
\draw (6,-0.2) -- (6,0.2);
\fill[black] (6,2) circle (2pt);
\draw (6,2) -- (8,2);
\draw [dashed] (6,0) -- (6,2);
\draw[black] (-1/3,1) circle (2pt);
\draw (-1/3,1) -- (-2,1);
\draw [dashed] (-1/3,0) -- (-1/3,1);
\node at (-5,1) {$x < -\frac{1}{3}$};
\node at (-5,2) {$x \geq 6$};
\end{tikzpicture}
$$

Le due soluzioni non si intersecano, quindi questo caso non ha soluzioni. Di solito si indica con: $$S = \emptyset$$, dove $$S$$ sta per soluzione e $$\emptyset$$ è il simbolo dell'insieme vuoto.

## Caso 2: $$-3+\frac{1}{2}x < 0$$ 

Nell'intervallo $$-3+\frac{1}{2}x < 0$$, ossia $$\frac{1}{2}x < 3$$, ossia $$x < 6$$, il valore assoluto è uguale a $$+3-\frac{1}{2}x$$. La disequazione quindi diventa 

$$ +3 - \frac{1}{2}x > 2x-\frac{5}{2}$$

Porto a sinistra tutti i termini con la $$x$$ e a destra tutti i termini senza:

$$ -\frac{1}{2}x -2x > -\frac{5}{2}-3$$

Sommo gli elementi e ottengo 

$$\frac{-x-4x}{2} > \frac{-5-6}{2}$$

$$-\frac{5}{2}x > -\frac{11}{2}$$

Moltiplico sia a destra che a sinistra per $$-\frac{2}{5}$$ in modo da isolare la $$x$$, ricordandomi di cambiare il verso della disuguaglianza perchè sto moltiplicando per un numero negativo:

$$x < -\frac{11}{2} \cdot \left(- \frac{2}{5}\right) \qquad \rightarrow \qquad x < + \frac{11}{5}$$

ATTENZIONE: la soluzione che ho trovato è definita soltanto nell'intervallo $$x < 6$$, perchè è qui che stiamo lavorando. Devo quindi intersecare le due cose: 

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (-2,2) rectangle (-1/3,0);
\draw [->](-2,0) -- (8,0);
\draw (-1/3,-0.2) -- (-1/3,0.2);
\node at (-1/3,-0.5) {$\frac{11}{5}$};
\node at (6,-0.5) {$6$};
\draw (6,-0.2) -- (6,0.2);
\draw (6,2) circle (2pt);
\draw (6,2) -- (-2,2);
\draw [dashed] (6,0) -- (6,2);
\draw[black] (-1/3,1) circle (2pt);
\draw (-1/3,1) -- (-2,1);
\draw [dashed] (-1/3,0) -- (-1/3,1);
\node at (-5,1) {$x < \frac{11}{5}$};
\node at (-5,2) {$x < 6$};
\end{tikzpicture}
$$

Nota: $$\frac{11}{5} = \frac{66}{30} < \frac{180}{30} = 6$$.

Le due soluzioni si intersecano dove c'è il giallo, quindi questo caso ha soluzioni. In particolare la soluzione è 

$$x < \frac{11}{5}$$

che è anche la soluzione totale dell'esercizio visto che il caso precedente non aveva soluzioni. 

Nota: se entrambi i casi hanno soluzioni, la soluzione finale di tutto l'esercizio è data dall'unione delle due soluzioni dei due casi.


