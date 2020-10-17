# Integrali 

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 7:

> Calcola il seguente integrale 

$$\int \frac{x^2+4x+1}{2x} dx $$ 
## Soluzione: 

Dal momento che il denominatore della frazione da integrare è composto da solo un termine, posso "spezzare" la frazione in frazioni più semplici:  

$$\begin{align*}
\int \frac{x^2+4x+1}{2x} dx & = \int \left(\frac{x^2}{2x} + \frac{4x}{2x}+ \frac{1}{2x} \right)dx \\
& = \int \left(\frac{x}{2} + 2+ \frac{1}{2x} \right)dx \\ 
& = \int \frac{x}{2}dx  + \int 2 dx + \int \frac{1}{2x}dx
\end{align*}$$

dove nell'ultimo passaggio ho utilizzato il fatto che l'integrale di una somma è uguale alla somma degli integrali. 

I tre integrali che abbiamo ottenuto sono immediati: ricordiamo la formula per risolverli. 

**Memo**: $$\int x^{\alpha}dx = \begin{cases}
\frac{x^{\alpha+1}}{\alpha +1} + c & \text{se} \ \alpha \neq -1 \\
\ln(|x|) + c & \text{se} \ \alpha = -1 
\end{cases}$$

Il primo integrale quindi è uguale a 

$$\begin{align*}
\int \frac{x}{2} dx & = \frac{1}{2} \cdot \int x dx \\
& =  \frac{1}{2} \cdot \frac{x^{1+1}}{1+1} + c_1 \\
& = \frac{1}{2}\cdot \frac{x^{2}}{2} + c_1 \\
& =  \frac{x^{2}}{4} + c_1
\end{align*}$$

Il secondo integrale è uguale a 

$$\begin{align*}
\int 2 dx & =  2 \cdot \int 1 dx \\
& = 2 \cdot x  + c_2 \\
& = 2x + c_2 \\
\end{align*}$$

Il terzo integrale è uguale a 

$$\begin{align*}
\int \frac{1}{2x} dx & = \frac{1}{2} \cdot \int \frac{1}{x} dx \\
& = \frac{1}{2} \cdot \int x^{-1} dx\\
& =  \frac{1}{2} \cdot \ln(|x|) + c_3 
\end{align*}$$

Possiamo ora mettere insieme tutti i pezzi e calcolare l'integrale iniziale

$$\begin{align*}
\int \frac{x^2+4x+1}{2x} dx & = \int \frac{x}{2}dx  + \int 2 dx + \int \frac{1}{2x}dx \\
& = \frac{x^2}{4} + c_1 + 2x + c_2 + \frac{\ln(|x|)}{2} + c_3 \\
& = \frac{x^2}{4}+ 2x+ \frac{\ln(|x|)}{2} + c
\end{align*}$$

dove nell'ultimo passaggio ho raggruppato assieme le costanti visto che somme e differenze di costanti rimangono costanti ($$c = c_1+c_2+c_3$$). 

