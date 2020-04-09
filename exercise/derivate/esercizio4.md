# DERIVATE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Data la seguente funzione, verifica se nell’intervallo indicato a fianco valgono le ipotesi del teorema di Lagrange e
trova il punto (o i punti) la cui esistenza è assicurata dal teorema:

$$f(x) = |x^2-1| \qquad [2,3]$$

## Soluzione:

Come prima cosa ricordiamo l'enunciato del teorema di Lagrange:

Se una funzione $$f(x)$$ è:
* continua in un intervallo limitato e chiuso $$[a,b]$$,
* derivabile in ogni punto interno a esso,

allora esiste almeno un punto $$c$$, interno all’intervallo,
per cui vale la relazione

$$f^{'}(c) = \frac{f(b)-f(a)}{b-a}$$

Per capire se questo teorema è applicabile nel nostro caso, dobbiamo andare a vedere se le due ipotesi sono vere per la $$f(x)$$ che abbiamo. 

Prima cosa da verificare: $$f(x)$$ continua in $$[2,3]$$

Ricordiamo che il valore assoluto è una funzione continua: se l'argomento del valore assoluto è continuo, allora lo è anche il valore assoluto. Tradotto nel nostro caso: se $$x^2-1$$ è una funzione continua, allora anche $$|x^2-1|$$ è una funzione continua. La funzione $$x^2-1$$ è una funzione polinomiale (in particolare è una parabola essendo di secondo grado), quindi è continua su tutto $$\mathbb{R}$$. Essendo continua su tutto $$\mathbb{R}$$, in particolare lo è su $$[2,3]$$. Quindi anche $$|x^2-1|$$ è continua su $$[2,3]$$ e la prima ipotesi è verificata.

 

Seconda cosa da verificare: $$f(x)$$ derivabile in $$(2,3)$$

Ricordiamo che il valore assoluto non è derivabile solo nei punti in cui il suo argomento si annulla. Nel nostro caso quindi, la funzione non è derivabile nei punti $$x$$ tali che

$$x^2-1 = 0$$

Risolvendo quest'equazione abbiamo

$$\begin{align*}
x^2-1 & = 0 \\
x^2 & = 1 \\
x & = \pm 1
\end{align*}$$

La funzione quindi non è derivabile in $$x=-1$$ e $$x=1$$. Lo è in tutti gli altri punti. 

A noi interessa che sia derivabile nell'intervallo $$(2,3)$$: poichè in questo intervallo non è compreso nè $$x=-1$$ nè $$x=1$$, la funzione in questo intervallo è derivabile. Quindi, è soddisfatta anche la seconda ipotesi del teorema.

Posso quindi applicare il teorema: esso mi dice che esiste un punto $$c$$ tale che

$$f^{'}(c) = \frac{f(3)-f(2)}{3-2}$$

A destra dell'uguaglianza ottengo:

$$\begin{align*}
f(2) & = |(2)^2-1| \\
& = |4-1| \\
& = |3| \\
& = 3 \\
f(3) & = |(3)^2-1| \\
& = |9-1| \\
& = |8| \\
& = 8 
\end{align*}$$

Quindi 

$$\frac{f(3)-f(2)}{3-2} = \frac{8-3}{1} = 5$$

A sinistra dell'uguale invece, prima di calcolare la derivata noto che, usando la definizione di valore assoluto ho

$$\begin{align*}
f(x) = |x^2-1| & = \begin{cases}
x^2-1 & \text{se} \; x^2-1 \geq 0 \\
-x^2+1 & \text{se} \; x^2-1 < 0
\end{cases} \\
& = \begin{cases}
x^2-1 & \text{se} \; x \leq -1 \cup x \geq 1\\
-x^2+1 & \text{se} \; -1 < x < 1
\end{cases} \\
\end{align*}$$

Poichè stiamo considerando l'intervallo $$[2,3]$$, siamo nel primo caso della funzione (ossia negli $$x \geq 1$$), ossia $$f(x) = x^2-1$$. Quello che voglio dire è che, nell'intervallo $$[2,3]$$ la funzione è $$f(x) = x^2-1$$. Dobbiamo quindi calcolare la derivata di questa funzione.

$$f^{'}(x) = D(x^2-1) = 2x$$

Quindi, la derivata calcolata in $$x=c$$ è

$$f^{'}(c) = 2c$$

Mettendo insieme tutti i pezzi, ho quindi che

$$\begin{align*}
f^{'}(c) & = \frac{f(3)-f(2)}{3-2} \\
2c & = 5 \\
\frac{2c}{2} & = \frac{5}{2} \\
c & = \frac{5}{2}
\end{align*}$$

Il punto $$c$$ che il teorema mi assicura esistere è quindi 

$$c = \frac{5}{2}$$






