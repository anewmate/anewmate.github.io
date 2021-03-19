# DISEQUAZIONE 2 GRADO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Risolvi la seguente disequazione

$$(x+1)^3 > x(x^2-2)+(x-2)(x+1)$$

## Soluzione: 

Come prima cosa svolgo i conti in modo da arrivare a una forma del tipo $$ax^2 + bx + c$$ con $$a>0$$. 

**Memo**: $$(A+B)^3 = A^3 + 3A^2B+3AB^2+B^3$$

$$\begin{align*}
(x+1)^3 & > x(x^2-2)+(x-2)(x+1) \\
x^3+3x^2+3x+1 & > x^3-2x+x^2+x-2x-2 \\
3x^2+3x+1 & > x^2-3x-2 \\
3x^2+3x+1 -x^2+3x+2 & > 0 \\
2x^2+6x+3 & \; \textcolor{red}{>} \; 0  
\end{align*}$$

Nel nostro caso quindi $$a = 2, b = 6, c = 3$$. Procediamo risolvendo l'equazione associata: 

$$\begin{align*}
2x^2 +6x +3 & =  0 \\
x_{1/2} & = \frac{-b \pm \sqrt{b^2-4ac}}{2a} \\
& = \frac{-6 \pm \sqrt{36-24}}{4} \\
& =  \frac{-6 \pm \sqrt{12}}{4} \\
& =  \frac{-6 \pm \sqrt{2^2 \cdot 3}}{4} \\ 
& =  \frac{-6 \pm 2\sqrt{3}}{4} \\
& = \frac{2(-3 \pm \sqrt{3})}{4} \\
& = \frac{-3 \pm \sqrt{3}}{2}
\end{align*}$$

Le due soluzioni sono quindi $$x_1 = \frac{-3+\sqrt{3}}{2}$$ e $$x_2 = \frac{-3-\sqrt{3}}{2}$$. 

Visto che volevamo l'espressione $$\textcolor{red}{\text{maggiore}}$$ di zero, la regola mi dice che devo considerare gli intervalli esterni ai due valori trovati. La soluzione è quindi

$$x < \frac{-3-\sqrt{3}}{2}\; \;  \vee \; \; x > \frac{-3+\sqrt{3}}{2}$$

**Memo**: Ricordiamo la regola in generale che ci dice. Se ho

1. espressione del tipo $$ax^2+bx+c \gtrless 0$$
1. $$\textbf{a}>0$$
1. delta positivo: $$\Delta > 0$$
1. $$x_1,x_2$$ soluzioni dell'equazione associata con $$x_2 < x_1$$

Allora $$ax^2+bx+c > 0$$ ha soluzione $$x < x_2 \cup x > x_1$$, mentre $$ax^2+bx+c < 0$$ ha soluzione $$x_2 < x < x_1$$. A parole, se voglio l'espressione positiva devo prendere l'unione degli intervalli esterni ai due valori che ottengo nell'equazione associata. Se invece voglio l'espressione negativa, devo prendere l'intervallo interno. In entrambi i casi, escludo o includo i punti estremi se la disuguaglianza è stretta oppure no.  

