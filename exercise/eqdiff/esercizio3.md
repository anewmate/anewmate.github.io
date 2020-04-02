# EQUAZIONI DIFFERENZIALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Risolvi la seguente equazione differenziale

$$y^{'}+3x^2y = x^2$$

> che soddisfa la condizione $$y(0) = \frac{4}{3}$$.

## Soluzione:

Come prima cosa notiamo che abbiamo sia $$y$$ che $$y^{'}$$ di primo grado: siamo quindi di fronte a un'equazione differenziale lineare. 

Sappiamo che in generale si scrive nella forma

$$y^{'} + a(x) \cdot y = b(x)$$

e ha soluzione

$$y = e^{-A(x)}\left(\int e^{A(x)}b(x)dx + c\right)$$

dove $$A(x) = \int a(x)dx$$ (senza $$+c$$).

Nel nostro caso $$a(x) = 3x^2$$ mentre $$b(x) = x^2$$. Calcoliamo subito $$A(x)$$.  

$$\begin{align*}
A(x) & = \int a(x)dx \\
& = \int 3x^2dx \\
& = 3 \int x^2 dx \\
& = 3 \cdot \left(\frac{x^3}{3}\right) \\
& = x^3
\end{align*}$$

La soluzione è quindi data da

$$y = e^{-x^3}\left(\int e^{x^3}x^2dx +c\right)$$

Calcoliamo separatamente l'integrale nella parentesi.

$$\int e^{x^3}x^2 dx$$

Analizziamo un attimo questo integrale: ad argomento abbiamo un esponenziale ($$e^{x^3}$$) moltiplicato per qualcosa ($$x^2$$) di molto simile alla derivata dell'esponente ($$x^3$$). Se calcoliamo infatti la derivata di $$e^{x^3}$$ otteniamo 

$$D\left(e^{x^3}\right) = e^{x^3} \cdot D(x^3) = e^{x^3} \cdot 3x^2 = 3e^{x^3}x^2$$

che è quasi quello che abbiamo ad argomento dell'integrale. Visto che ci "manca solo quel 3" moltiplichiamo (e dividiamo, se no non otteniamo un'equivalenza) l'argomento per 3:

$$\begin{align*}
\int e^{x^3}x^2 dx & = \int \frac{1}{3} \cdot 3 \cdot e^{x^3}x^2 dx \\
& = \frac{1}{3} \int 3e^{x^3}x^2dx \\
& = \frac{1}{3} \int D\left(e^{x^3}\right)dx \\
& = \frac{1}{3}e^{x^3}
\end{align*}$$ 

La funzione $$y$$ che cercavamo diventa quindi 

$$\begin{align*}
y & = e^{-x^3}\left(\int e^{x^3}x^2dx +c\right) \\
& = e^{-x^3}\left(\frac{1}{3}e^{x^3} +c\right) \\
& = \frac{1}{3}e^{x^3}e^{-x^3} + ce^{-x^3} \\
& = \frac{1}{3}e^{x^3-x^3} + ce^{-x^3} \\
& = \frac{1}{3}e^{0} + \frac{c}{e^{x^3}} \\
& = \frac{1}{3} \cdot 1 +\frac{c}{e^{x^3}} \\
& = \frac{1}{3} + \frac{c}{e^{x^3}}
\end{align*}$$

La soluzione generale è quindi 

$$y = \frac{1}{3} + \frac{c}{e^{x^3}}$$

Dobbiamo però trovare la soluzione particolare tale che $$y(0) = \frac{4}{3}$$. Ciò significa che devo trovare $$c$$ imponendo quella condizione, ossia che la mia funzione calcolata in $$x=0$$ sia uguale a $$\frac{4}{3}$$. Come prima cosa quindi calcoliamo la funzione in zero:

$$\begin{align*}
y(0) & = \frac{1}{3} + \frac{c}{e^{(0)^3}} \\
& = \frac{1}{3} + \frac{c}{e^{0}} \\
& = \frac{1}{3} + \frac{c}{1} \\
& = \frac{1}{3} + c
\end{align*}$$

La condizione ci dice che questa quantità deve essere uguale a $$\frac{4}{3}$$:

$$\begin{align*}
\frac{1}{3} + c & = \frac{4}{3} \\
c & = \frac{4}{3} - \frac{1}{3} \\
c & = \frac{4-1}{3} \\
c & = \frac{3}{3} \\
c & = 1
\end{align*}$$

Ora che abbiamo trovato $$c$$ possiamo scrivere la rispettiva soluzione con questo valore:

$$y = \frac{1}{3} + \frac{1}{e^{x^3}}$$

che è la soluzione del nostro problema.


