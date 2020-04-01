# EQUAZIONI DIFFERENZIALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Risolvi la seguente equazione differenziale

$$2yy^{'}-y^{2}x-2x = 0$$

## Soluzione:

Come prima cosa isoliamo la derivata di $$y$$:

$$\begin{align*}
2yy^{'}-y^{2}x-2x & = 0 \\
2yy^{'} & = y^{2}x+2x \\
y^{'} & = \frac{y^{2}x+2x}{2y} \\
y^{'} & = \frac{x(y^2+2)}{2y} \\
y^{'} & = x\left(\frac{y^2+2}{2y}\right) \\
y^{'} & = \underbrace{x}_{\text{funzione di x}}\underbrace{\left(\frac{y^2+2}{2y}\right)}_{\text{funzione di y}}
\end{align*}$$

Siamo quindi di fronte a un'equazione differenziale del tipo 

$$y^{'} = g(x)\cdot h(y)$$

dove, nel nostro caso, $$g(x) = x$$ e $$h(y) = \frac{y^2+2}{2y}$$.

Per risolverla si applica il metodo della separazione delle variabili. 

Piccola parentesi per capire come funziona questo metodo:

Sappiamo che scrivere $$y$$ o scrivere $$f(x)$$ è lo stesso: modi diversi per scrivere la stessa identica cosa. Analogamente, ci sono vari modi per indicare la derivata: i più comuni sono $$'$$ oppure $$D$$. Un terzo modo è 

$$\frac{d(\text{cosa voglio derivare})}{d(\text{variabile rispetto a cui voglio fare la derivata})}$$

Per esempio, se voglio derivare la nostra funzione $$f(x)$$ rispetto alla variabile $$x$$ (tradotto: la derivata che facciamo sempre) posso scrivere equivalentemente

$$\frac{d f(x)}{dx}, D(f(x)), f^{'}(x)$$

E visto che scrivere $$f(x)$$ è come scrivere $$y$$ ho 

$$\frac{dy}{dx}, D(y), y^{'}$$

Ora, se invece di $$y^{'}$$ scrivo $$\frac{dy}{dx}$$ e lo tratto come se fosse una frazione, ottengo

$$\begin{align*}
y^{'} & = g(x)h(y) \\
\frac{dy}{dx} & = g(x)h(y)
\end{align*}$$

Moltiplico destra e sinistra per $$\frac{dx}{h(y)}$$:

$$\begin{align*}
\frac{dy}{dx} \cdot \frac{dx}{h(y)} & = g(x)h(y) \cdot \frac{dx}{h(y)} \\
\frac{dy}{h(y)} & = g(x)dx
\end{align*}$$

Integro destra e sinistra: 

$$\begin{align*}
\int \frac{dy}{h(y)} & = \int g(x)dx
\end{align*}$$

e calcolo infine e due integrali separatamente. 

Applichiamo questo metodo al nostro caso. 

$$\begin{align*}
\frac{dy}{dx} & = x\left(\frac{y^2+2}{2y}\right) \\
\frac{dy}{dx} \cdot \frac{dx}{\frac{y^2+2}{2y}}& = x\left(\frac{y^2+2}{2y}\right) \cdot \frac{dx}{\frac{y^2+2}{2y}} \\
\frac{dy}{\frac{y^2+2}{2y}} & = xdx \\
\frac{2y}{y^2+2}dy & = xdx \\
\int \frac{2y}{y^2+2}dy & = \int xdx
\end{align*}$$

Risolviamo ora i due integrali separatamente. Quello a destra è facile e otteniamo

$$\int xdx = \frac{x^2}{2}+c$$

Per quello a sinistra invece basta notare che a numeratore della frazione c'è esattamente la derivata del denominatore quindi 

$$\int \frac{2y}{y^2+2}dy = \ln(y^2+2)$$

***
Memo: 

$$\int \frac{f^{'}(x)}{f(x)}dx = \ln(|f(x)|)+c$$

Nel nostro caso la variabile è $$y$$ invece che $$x$$, $$f(y) = y^2+2 \Rightarrow f^{'}(y) = 2y$$, e non metto il valore assoluto ad argomento del logaritmo in quanto so già che $$y^2+2$$ è positivo: $$y^2$$ è positivo perchè è un quadrato, sommandoci +2 ottengo sempre qualcosa di positivo. 
***

Ora che abbiamo calcolato i due integrali abbiamo quindi che 

$$\begin{align*}
\int \frac{2y}{y^2+2}dy & = \int xdx \\
\ln(y^2+2) & = \frac{x^2}{2}+c \\
e^{\ln(y^2+2)} & = e^{\frac{x^2}{2}+c} \\
y^2+2 & = e^{\frac{x^2}{2}+c} \\
y^2 & = e^{\frac{x^2}{2}+c} -2 \\
y & = \pm \sqrt{e^{\frac{x^2}{2}+c}-2}
\end{align*}$$

Le soluzioni dell'equazione differenziali sono quindi 

$$y = \pm \sqrt{e^{\frac{x^2}{2}+c}-2}$$



