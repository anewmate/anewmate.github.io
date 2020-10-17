# Integrali 

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 6:

> Calcola il seguente integrale 

$$\int \left( \frac{2}{x^3}-x^2-\frac{1}{x}\right) dx $$ 
## Soluzione: 

Sapendo che l'integrale di una somma si può "spezzare" nella somma degli integrali, il primo passaggio da fare è 

$$\begin{align*}
\int \left( \frac{2}{x^3}-x^2-\frac{1}{x}\right) dx & = \int \frac{2}{x^3}dx -\int x^2 dx- \int \frac{1}{x} dx \\
& = 2 \cdot \int \frac{1}{x^3}dx -\int x^2 dx- \int \frac{1}{x} dx
\end{align*}$$

dove nel secondo passaggio ho utilizzato il fatto che le costanti si possono "portare fuori" dall'integrale. 

I tre integrali che abbiamo ottenuto sono immediati: ricordiamo la formula per risolverli. 

**Memo**: $$\int x^{\alpha}dx = \begin{cases}
\frac{x^{\alpha+1}}{\alpha +1} + c & \text{se} \ \alpha \neq -1 \\
\ln(|x|) + c & \text{se} \ \alpha = -1 
\end{cases}$$

Il primo integrale quindi è uguale a 

$$\begin{align*}
\int \frac{1}{x^3} dx & = \int x^{-3} dx \\
& =  \frac{x^{-3+1}}{-3+1} + c_1 \\
& = \frac{x^{-2}}{-2} + c_1 \\
& = - \frac{x^{-2}}{2} + c_1 \\
& = - \frac{1}{2x^2} + c_1 
\end{align*}$$

Il secondo integrale è uguale a 

$$\begin{align*}
\int x^2 dx & =  \frac{x^{2+1}}{2+1} + c_2 \\
& = \frac{x^{3}}{3} + c_2 \\
\end{align*}$$

Il terzo integrale è uguale a 

$$\begin{align*}
\int \frac{1}{x} dx & = \int x^{-1} dx \\
& =  \ln(|x|) + c_3 
\end{align*}$$

Possiamo ora mettere insieme tutti i pezzi e calcolare l'integrale iniziale

$$\begin{align*}
\int \left( \frac{2}{x^3}-x^2-\frac{1}{x}\right) dx
& = 2 \cdot \int \frac{1}{x^3}dx -\int x^2 dx- \int \frac{1}{x} dx \\
& = 2 \cdot \left(-\frac{1}{2x^2}+c_1\right) -\left(\frac{x^3}{3} + c_2 \right)- \left(\ln(|x|)+c_3\right) \\
& = -\frac{1}{x^2} +2c_1 - \frac{x^3}{3} - c_2 -\ln(|x|) -c_3 \\
& = -\frac{1}{x^2} - \frac{x^3}{3}-\ln(|x|) + c  
\end{align*}$$

dove nell'ultimo passaggio ho raggruppato assieme le costanti visto che somme e differenze di costanti rimangono costanti ($$c = 2c_1-c_2-c_3$$). 

