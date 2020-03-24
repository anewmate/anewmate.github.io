# INTEGRALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Calcola il seguente integrale, se è convergente

$$\int_{-1}^{0} \ln\left(\frac{1}{x+1}\right)dx$$

## Soluzione: 

Come prima cosa ricordiamo che quando si hanno integrali definiti, prima si calcola l'integrale indefinito (ossia senza estremi di integrazione) e poi si applica il teorema fondamentale del calcolo integrale.

Come seconda cosa ricordiamo che quando si hanno esponenziali o logaritmi come argomenti dell'integrali, se a occhio non si vede qual è la tecnica giusta per risolverli, il primo tentativo che si può fare è quello dell'integrazione per parti. Ricordo la formula:

$$\int f^{'}(x)g(x)dx = f(x)g(x) - \int f(x)g^{'}(x)dx$$

Nel nostro caso $$f^{'}(x) = 1$$ mentre $$g(x) = \ln\left(\frac{1}{x+1}\right)$$.

Da $$f^{'}(x) = 1$$ ottengo $$f(x) = x$$: se infatti mi chiedo qual è quella funzione che derivata fa 1, ottengo subito $$x$$.

Da $$g(x) = \ln\left(\frac{1}{x+1}\right)$$ ottengo $$g^{'}(x) = \frac{1}{\frac{1}{x+1}}\cdot \left(-\frac{1}{(x+1)^2}\right) = (x+1) \cdot \left(-\frac{1}{(x+1)^2}\right) = -\frac{1}{x+1}$$. Si tratta infatti di una derivata composta che, ricordo, si risolve in generale come 

$$\ln(\star(x)) = \frac{1}{\star(x)} \cdot D(\star(x))$$

dove $$\star(x)$$ è una qualsiasi funzione di $$x$$, nel nostro caso $$\star(x) = \frac{1}{x+1}$$. 

Quindi 

$$\begin{align*}
\int \ln\left(\frac{1}{x+1}\right)dx & = x\ln\left(\frac{1}{x+1}\right) - \int x \cdot \left(-\frac{1}{x+1}\right)dx \\
& = x\ln\left(\frac{1}{x+1}\right) + \int  \frac{x}{x+1}dx
\end{align*}$$

Per risolvere il secondo integrale che ci troviamo, ci dobbiamo ricordare che quando abbiamo l'integrale di una frazione in cui sia a numeratore che a denominatore ci sono dei polinomi dello stesso grado, la tecnica consiste nel riscrivere il numeratore come il denominatore per poter poi spezzare la frazione in più frazioni. In particolare, vorrei far "comparire" a numeratore $$x+1$$. Ci riesco aggiungendo (e sottraendo, altrimenti non ottengo qualcosa di equivalente) 1 a numeratore. 

$$\begin{align*}
\int \frac{x}{x+1}dx & = \int \frac{x+1-1}{x+1}dx \\
& = \int \left(\frac{x+1}{x+1}+ \frac{-1}{x+1}\right)dx \\
& = \int 1 dx - \int \frac{1}{x+1}dx \\
& = x - \ln(x+1) \\
& = x + \ln((x+1)^{-1}) \\
& = x + \ln\left(\frac{1}{x+1}\right)
\end{align*}$$ 

La soluzione se l'integrale fosse indefinito sarebbe dunque

$$\int \ln\left(\frac{1}{x+1}\right)dx = x\ln\left(\frac{1}{x+1}\right) + x + \ln\left(\frac{1}{x+1}\right)+c$$

Ma visto che l'integrale va calcolato fra -1 e 0, il teorema fondamentale del calcolo integrale mi dice che 

$$\int_{-1}^{0} \ln\left(\frac{1}{x+1}\right)dx = \left[x\ln\left(\frac{1}{x+1}\right) + x + \ln\left(\frac{1}{x+1}\right)\right]_{-1}^{0}$$

Se chiamo $$F(x) = x\ln\left(\frac{1}{x+1}\right) + x + \ln\left(\frac{1}{x+1}\right)$$, posso vedere subito che $$F$$ non è definita in $$x=-1$$. Quindi

$$\int_{-1}^{0} \ln\left(\frac{1}{x+1}\right)dx = F(0) - \lim_{x\rightarrow -1}F(x)$$

Vediamo subito che $$F(0) = 0\ln(1)+0+\ln(1) = 0$$ poichè il logaritmo di 1 è zero. Andiamo invece a calcolare quel limite.

$$\begin{align*}
\lim_{x\rightarrow -1} x\ln\left(\frac{1}{x+1}\right) + x + \ln\left(\frac{1}{x+1}\right) & = \lim_{x\rightarrow -1}  x +(x+1)\ln\left(\frac{1}{x+1}\right)\\
& = "-1 + 0 \cdot \infty"
\end{align*}$$

Devo quindi risolvere quella forma indeterminata $$0\cdot \infty$$.
$$\begin{align*}
\lim_{x \rightarrow -1}(x+1)\ln\left(\frac{1}{x+1}\right) & = \lim_{x \rightarrow -1} \frac{\ln\left(\frac{1}{x+1}\right)}{\frac{1}{x+1}} \\
& \overset{\text{De l'Hopital}}{=} \lim_{x \rightarrow -1} \frac{(x+1)\cdot \left(-\frac{1}{(x+1)^2}\right)}{-\frac{1}{(x+1)^2}} \\
& = \lim_{x \rightarrow -1} x+1 \\
& = 0
\end{align*}$$

dove noto che posso applicare il teorema di De l'Hopital poichè nella prima uguaglianza il temine a destra è una forma indeterminata del tipo $$\frac{\infty}{\infty}$$.

Abbiamo quindi che 

$$\begin{align*}
\lim_{x\rightarrow -1} F(x) & = \lim_{x\rightarrow -1}  x +(x+1)\ln\left(\frac{1}{x+1}\right)\\
& = -1 + 0 \\
& = -1
\end{align*}$$

L'integrale di partenza ha quindi soluzione 

$$\begin{align*}
\int_{-1}^{0} \ln\left(\frac{1}{x+1}\right)dx & = F(0) - \lim_{x\rightarrow -1}F(x) \\
& = 0 - (-1) \\
& = 1 
\end{align*}$$

















