# DISEQUAZIONI CON VALORE ASSOLUTO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Risolvi la seguente disequazione che contiene valori assoluti:

$$3|x|-2 < 2|x| +3$$

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
3|x|-2 & < 2|x| +3 \\
3|x| -2|x| & < +2+3 \\
|x| & < 5
\end{align*}
$$

Mi sto quindi chiedendo quando un valore assoluto è minore di un numero positivo. Ho due possibilità per risolvere questa disequazione. 

### CASO 1: mi ricordo la formula 

Siamo arrivati a una disequazione in cui ho solo un valore assoluto a sinistra e solo un numero positivo a destra, ossia $$|A(x)| < k$$ con $$k \geq 0$$. Se mi ricordo le formule, so che 

$$|A(x)| < k \; \; \text{è equivalente a} \; \; -k < A(x) < k$$

Nel nostro caso la soluzione arriva direttamente visto che $$A(x) = x$$ e $$k = 5$$

$$-5 < x < 5$$

### CASO 2: non mi ricordo la formula

Se non mi ricordo la formula scritta prima, posso risolvere comunque la disequazione, ma devo sapere la definizione di valore assoluto (quella scritta all'inizio). 

$$|x| = \begin{cases}
x  & \text{se} \ x \geq 0 \\
-x  & \text{se} \ x < 0
\end{cases}$$

Utilizzando quella infatti spezzo la disequazione in due casi: 

$$\begin{align*}
|x| < 5  \rightarrow & \begin{cases}
x < 5 & \text{se} \ x \geq 0 \\
-x < 5 & \text{se} \ x < 0
\end{cases} \\
& \begin{cases}
x < 5 & \text{se} \ x \geq 0 \\
(-1) \cdot (-x) \; {\color{red}{>}} \;  5 \cdot (-1) & \text{se} \ x < 0
\end{cases} \\
& \begin{cases}
x < 5 & \text{se} \ x \geq 0 \\
x > -5 & \text{se} \ x < 0
\end{cases}
\end{align*}
$$

Dalla prima riga ottengo le soluzioni $$0 \leq x < 5$$, mentre dalla seconda riga ottengo $$-5 < x < 0$$. 

Dovendo unire le due soluzioni trovate, ritroviamo esattamente la stessa soluzione trovata al Caso 1: 

$$ -5 < x < 5$$

