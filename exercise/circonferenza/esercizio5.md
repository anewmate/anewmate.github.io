# Circonferenza
<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 5:

> Determina la lunghezza della corda che la circonferenza di equazione $$x^2+y^2-12x+2y-37 = 0 $$ stacca sulla retta di equazione $$y = 2x+4$$. 
  
## Soluzione: 

Dal testo possiamo già intuire che la circonferenza e la retta sono secanti e si intersecano in due punti che saranno gli estremi della corda di cui dobbiamo calcolare la lunghezza. Partiamo quindi calcolando le coordinate dei due punti di intersezione mettendo a sistema l'equazione della circonferenza con quella della retta: 

$$\begin{align*}
& \begin{cases}
x^2+y^2-12x+2y-37 = 0 \\
y = 2x+4 
\end{cases} \\
& \begin{cases}
x^2+(2x+4)^2-12x+2(2x+4)-37 = 0 \\
y = 2x+4 
\end{cases}
\end{align*}$$ 

dove nel secondo sistema ho sostituito la $$y$$ nella prima equazione. Lavoro quindi solo con la prima equazione in $$x$$:

$$\begin{align*}
x^2+(2x+4)^2-12x+2(2x+4)-37 & = 0 \\
x^2+4x^2+16x+16-12x+4x+8-37 & = 0 \\
5x^2 +8x -13 & = 0 \\
x_{1/2} & = \frac{-8\pm \sqrt{64+260}}{10} \\
& = \frac{-8\pm 18}{10}
\end{align*}$$

Abbiamo quindi $$x_1 = 1$$ e $$x_2 = -\frac{13}{5}$$. Per trovare le corrispettive $$y$$ uso la seconda equazione $$y = 2x+4$$:

$$\begin{align*}
& \begin{cases}
x = 1\\
y = 2x+4 = 2(1)+4 = 6
\end{cases} \\
& \begin{cases}
x = -\frac{13}{5} \\
y = 2x+4 = 2\left(-\frac{13}{5}\right)+4 = \frac{-26+20}{5} = -\frac{6}{5} 
\end{cases}
\end{align*}$$ 

I due punti di intersezione sono quindi $$A(1;6)$$ e $$B\left(-\frac{13}{5};-\frac{6}{5}\right)$$. Per calcolare quanto è lunga la corda, basta quindi calcolare la distanza fra questi due punti:

$$\begin{align*}
AB & = \sqrt{(x_B-x_A)^2+(y_B-y_A)^2} \\
& = \sqrt{\left(-\frac{13}{5}-1\right)^2+\left(-\frac{6}{5}-6\right)^2} \\
& = \sqrt{\left(\frac{-13-5}{5}\right)^2+ \left(\frac{-6-30}{5}\right)^2} \\
& = \sqrt{\frac{324}{25} + \frac{1296}{25}} \\
& = \sqrt{\frac{1620}{25}} \\
& = \frac{\sqrt{18^2 \cdot 5}}{\sqrt{5^2}} \\
& = \frac{18\sqrt{5}}{5}
\end{align*}$$


