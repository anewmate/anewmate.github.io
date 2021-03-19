# DISEQUAZIONE 2 GRADO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente disequazione

$$x(x+2\sqrt{2}) +2(\sqrt{2}x-6) < 3\sqrt{2}x$$

## Soluzione: 

Come prima cosa svolgo i conti in modo da arrivare a una forma del tipo $$ax^2 + bx + c$$ con $$a>0$$. 

$$\begin{align*}
x(x+2\sqrt{2}) +2(\sqrt{2}x-6) & < 3\sqrt{2}x \\
x^2 + 2\sqrt{2}x +2\sqrt{2}x-12 & < 3\sqrt{2} x \\
x^2 + 2\sqrt{2}x +2\sqrt{2}x-12 - 3\sqrt{2} x & < 0 \\
x^2 +\sqrt{2} x - 12 & \; \textcolor{red}{<} \; 0 
\end{align*}$$

Nel nostro caso quindi $$a = 1, b = \sqrt{2}, c = -12$$. Procediamo risolvendo l'equazione associata: 

$$\begin{align*}
x^2 +\sqrt{2} x - 12 & =  0 \\
x_{1/2} & = \frac{-b \pm \sqrt{b^2-4ac}}{2a} \\
& = \frac{-\sqrt{2} \pm \sqrt{2+48}}{2} \\
& =  \frac{-\sqrt{2} \pm \sqrt{50}}{2} \\
& =  \frac{-\sqrt{2} \pm \sqrt{5^2 \cdot 2}}{2} \\ 
& =  \frac{-\sqrt{2} \pm 5\sqrt{2}}{2} \\
\end{align*}$$

Le due soluzioni sono quindi $$x_1 = \frac{-\sqrt{2}+5\sqrt{2}}{2} = \frac{4\sqrt{2}}{2} = 2\sqrt{2}$$ e $$x_2 = \frac{-\sqrt{2}-5\sqrt{2}}{2} = \frac{-6\sqrt{2}}{2} = -3\sqrt{2}$$. 

Visto che volevamo l'espressione $$\textcolor{red}{\text{minore}}$$ di zero, la regola mi dice che devo considerare l'intervallo interno ai due valori trovati. La soluzione è quindi

$$-3\sqrt{2} < x < 2\sqrt{2}$$

**Memo**: Ricordiamo la regola in generale che ci dice. Se ho

1. espressione del tipo $$ax^2+bx+c \gtrless 0$$
1. $$\textbf{a}>0$$
1. delta positivo: $$\Delta > 0$$
1. $$x_1,x_2$$ soluzioni dell'equazione associata con $$x_2 < x_1$$

Allora $$ax^2+bx+c > 0$$ ha soluzione $$x < x_2 \cup x > x_1$$, mentre $$ax^2+bx+c < 0$$ ha soluzione $$x_2 < x < x_1$$. A parole, se voglio l'espressione positiva devo prendere l'unione degli intervalli esterni ai due valori che ottengo nell'equazione associata. Se invece voglio l'espressione negativa, devo prendere l'intervallo interno. In entrambi i casi, escludo o includo i punti estremi se la disuguaglianza è stretta oppure no.  

