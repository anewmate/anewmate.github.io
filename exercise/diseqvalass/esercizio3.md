# DISEQUAZIONI CON VALORE ASSOLUTO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Risolvi la seguente disequazione che contiene valori assoluti:

$$3+|x-2| > 8 - |x-2|$$

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

Visto che all'interno della disequazione c'è lo stesso valore assoluto, la sistemiamo portando i valori assoluti a sinistra e il resto a destra: 

$$\begin{align*}
3+|x-2| & > 8 - |x-2| \\
|x-2| +|x-2| & > -3+8 \\
2|x-2| & > 5 \\
\frac{2|x-2|}{2} & > \frac{5}{2} \\
|x-2| & > \frac{5}{2}
\end{align*}
$$

dove nell'ultimo passaggio ho diviso tutto per $$2$$ per isolarmi il valore assoluto. 

Mi sto quindi chiedendo quando un valore assoluto è maggiore di un numero positivo. Ho due possibilità per risolvere questa disequazione. 

### CASO 1: mi ricordo la formula 

Siamo arrivati a una disequazione in cui ho solo un valore assoluto a sinistra e solo un numero positivo a destra, ossia $$|A(x)| > k$$ con $$k \geq 0$$. Se mi ricordo le formule, so che 

$$|A(x)| > k \; \; \text{è equivalente a} \; \;  A(x) < -k \; \vee \; A(x) > k$$

Nel nostro caso $$A(x) = x-2$$ e $$k = \frac{5}{2}$$ e la soluzione diventa quindi 

$$\begin{align*}
x-2  < -\frac{5}{2} \; & \vee \; x-2 > \frac{5}{2}  \\
x  < -\frac{5}{2}+2 \; & \vee \; x > \frac{5}{2}+ 2  \\
x  < \frac{-5+4}{2} \; & \vee \; x > \frac{5+4}{2}  \\
x < -\frac{1}{2} \; & \vee \; x > \frac{9}{2}  
\end{align*}
$$

### CASO 2: non mi ricordo la formula

Se non mi ricordo la formula scritta prima, posso risolvere comunque la disequazione, ma devo sapere la definizione di valore assoluto (quella scritta all'inizio). 

$$|x-2| = \begin{cases}
x-2  & \text{se} \ x-2 \geq 0 \\
-x+2  & \text{se} \ x-2 < 0
\end{cases}$$

Utilizzando quella infatti spezzo la disequazione in due casi: 

$$\begin{align*}
|x-2| > \frac{5}{2}  \rightarrow & \begin{cases}
x-2 > \frac{5}{2} & \text{se} \ x-2 \geq 0 \\
-x+2 > \frac{5}{2} & \text{se} \ x -2 < 0
\end{cases} \\
\end{align*}
$$

La prima disequazione può essere scritta come il sistema 

$$\begin{align*}
\begin{cases}
x-2 > \frac{5}{2} \\
x-2 \geq 0 
\end{cases} \\
\end{align*}
$$

che risolta diventa 

$$\begin{align*}
\begin{cases}
x > \frac{5}{2}+2 \\
x\geq 2 
\end{cases} \\ 
\begin{cases}
x > \frac{9}{2} \\
x \geq 2
\end{cases} \\
\end{align*}
$$

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (3,2) rectangle (5,0);
\draw [->](0,0) -- (5,0);
\draw (1,-0.2) -- (1,0.2);
\node at (1,-0.5) {$2$};
\node at (3,-0.5) {$\frac{9}{2}$};
\draw (3,-0.2) -- (3,0.2);
\draw[fill=black] (1,1) circle (2pt);
\draw (3,2) -- (5,2);
\draw [dashed] (3,0) -- (3,2);
\draw (1,1) -- (5,1);
\draw [dashed] (1,0) -- (1,1);
\draw[fill=white] (3,2) circle (2pt);
\node at (-1,1) {$x \geq 2$};
\node at (-1,2) {$x > \frac{9}{2}$};
\end{tikzpicture}
$$

ossia $$x > \frac{9}{2}$$. 

La seconda disequazione può essere scritta come il sistema 

$$\begin{align*}
\begin{cases}
-x+2 > \frac{5}{2} \\
x-2 < 0 
\end{cases} \\
\end{align*}
$$

che risolta diventa 

$$\begin{align*}
\begin{cases}
-x > \frac{5}{2}-2 \\
x < 2 
\end{cases} \\ 
\begin{cases}
-x > \frac{1}{2} \\
x < 2
\end{cases} \\
\begin{cases}
x < -\frac{1}{2} \\
x < 2
\end{cases} \\
\end{align*}
$$

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (-1,2) rectangle (1,0);
\draw [->](-1,0) -- (4,0);
\draw (1,-0.2) -- (1,0.2);
\node at (1,-0.5) {$-\frac{1}{2}$};
\node at (3,-0.5) {$2$};
\draw (3,-0.2) -- (3,0.2);
\draw (1,2) -- (-1,2);
\draw [dashed] (1,0) -- (1,2);
\draw (3,1) -- (-1,1);
\draw [dashed] (3,0) -- (3,1);
\draw[fill=white] (3,1) circle (2pt);
\draw[fill=white] (1,2) circle (2pt);
\node at (-2,1) {$x < 2$};
\node at (-2,2) {$x < -\frac{1}{2}$};
\end{tikzpicture}
$$

ossia $$x < -\frac{1}{2}$$. 

Dovendo prendere tutte e due le soluzioni trovate, la soluzione dell'intero esercizio anche in questo caso è 

$$x < -\frac{1}{2} \; & \vee \; x > \frac{9}{2} $$


