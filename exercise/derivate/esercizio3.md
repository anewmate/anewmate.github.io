# DERIVATE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Data la seguente funzione, verifica se nell’intervallo indicato a fianco valgono le ipotesi del teorema di Rolle e
trova il punto (o i punti) la cui esistenza è assicurata dal teorema:

$$f(x) = 4x^2-2x \qquad [-1,3]$$

## Soluzione:

Come prima cosa ricordiamo l'enunciato del teorema di Rolle:

Data una funzione $$f(x)$$ definita in un intervallo limitato
e chiuso $$[a,b]$$ con le seguenti proprietà:
* $$f(x)$$ è continua in $$[a,b]$$,
* $$f(x)$$ è derivabile in $$(a,b)$$,
* $$f(a) = f(b)$$,

allora esiste almeno un punto $$c$$, interno all’intervallo,
per il quale risulta $$f^{'}(c) = 0$$.

Per capire se questo teorema è applicabile nel nostro caso, dobbiamo andare a vedere se le tre ipotesi sono vere per la $$f(x)$$ che abbiamo. 

Prima cosa da verificare: $$f(x)$$ continua in $$[-1,3]$$

Dato che $$f(x)$$ è una funzione polinomiale ( di fatto è una parabola essendo un polinomio di secondo grado), essa è continua su tutto $$\mathbb{R}$$. In particolare, quindi, è continua in $$[-1,3]$$. 

Seconda cosa da verificare: $$f(x)$$ derivabile in $$[-1,3]$$

Per lo stesso motivo del punto precedente, dato che $$f(x)$$ è una funzione polinomiale, essa è derivabile in tutta $$\mathbb{R}$$. In particolare, è derivabile in $$(-1,3)$$.

**MEMO:** In generale una funzione polinomiale è una funzione del tipo 

$$f(x) = a_nx^n + a_{n-1}x^{n-1} + \cdots + a_2x^2 + a_1x + a_0$$

dove $$a_0,\dots, a_n$$ sono numeri reali. Fra le varie proprietà delle funzioni polinomiali, c'è in particolare il fatto che una funzione polinomiale è continua su tutto $$\mathbb{R}$$ e derivabile su tutto $$\mathbb{R}$$. 

Terza cosa da verificare: $$f(-1) = f(3)$$

Calcoliamo le due quantità separatamente:

$$\begin{align*}
f(-1) & = 4\cdot (-1)^2-2\cdot(-1) \\
& = 4\cdot (1)+2 \\
& = 6 \\
f(3) & = 4\cdot (3)^2-2\cdot (3) \\
& = 4\cdot (9)-6 \\
& = 30 
\end{align*}$$

Vediamo quindi che $$f(-1)$$ non è uguale a $$f(3)$$: $$f(-1) \neq f(3)$$.

Venendo meno questa ipotesi del teorema, esso non è applicabile. Ricordo infatti che per poter applicare un teorema devono essere valide TUTTE le ipotesi. 





