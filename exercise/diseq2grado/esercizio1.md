# DISEQUAZIONE 2 GRADO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente disequazione

$$(x-1)^2 + 10x -7(x+1) < 0$$

## Soluzione: 

Come prima cosa svolgo i conti in modo da arrivare a una forma del tipo $$ax^2 + bx + c$$ con $$a>0$$. Ricordo che lo sviluppo del quadrato si svolge come 

$$(A-B)^2 = A^2 + B^2 - 2AB$$

Quindi ottengo 

$$x^2 + 1 -2x + 10x -7x - 7 < 0$$

Sommo tutti i termini con lo stesso grado e ottengo 

$$x^2 + x -6 < 0$$

Data la formula generale $$ax^2 + bx + c$$, nel nostro caso abbiamo $$a=+1$$, $$b=+1$$, e $$c=-6$$. Dato che $$a$$ è positivo, possiamo procedere e risolvere l'equazione associata:

$$x^2 + x - 6 = 0$$

Applico la formula 

$$x_{1/2} = \frac{-b\pm \sqrt{b^2-4ac}}{2a}$$

ottenendo

$$x_{1/2} = \frac{-1\pm \sqrt{1-4(1)(-6)}}{2}$$

Le due soluzioni sono quindi $$x = 2$$ e $$x = -3$$. 

Visto che volevamo l'espressione minore di zero, la regola mi dice che devo considerare l'intervallo interno ai due valori trovati. La soluzione è quindi

$$-3 < x < 2$$

MEMO: Ricordiamo la regola in generale che ci dice. Se ho

1. espressione del tipo $$ax^2+bx+c \gtrless 0$$
1. $$\textbf{a}>0$$
1. delta positivo: $$\Delta > 0$$
1. $$x_1,x_2$$ soluzioni dell'equazione associata con $$x_2 < x_1$$

Allora $$ax^2+bx+c > 0$$ ha soluzione $$x < x_2 \cup x > x_1$$, mentre $$ax^2+bx+c < 0$$ ha soluzione $$x_2 < x < x_1$$. A parole, se voglio l'espressione positiva devo prendere l'unione degli intervalli esterni ai due valori che ottengo nell'equazione associata. Se invece voglio l'espressione negativa, devo prendere l'intervallo interno. In entrambi i casi, escludo o includo i punti estremi se la disuguaglianza è stretta oppure no.  