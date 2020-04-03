# INTEGRALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Calcola il seguente integrale

$$\int \frac{x+3}{\sqrt{x+2}}dx$$

## Soluzione:

Come prima cosa notiamo che a numeratore della frazione non abbiamo la derivata del denominatore. Quindi **non** siamo nel caso degli integrali del tipo 

$$\int \frac{f^{'}(x)}{f(x)}dx$$

Possiamo quindi procedere a risolvere l'integrale o utilizzando la formula per parti o per sostituzione. 

Ricordo che la formula per parti mi dice che

$$\int f^{'}(x)g(x)dx = f(x)g(x) - \int f(x)g^{'}(x)dx$$

In questo caso questo metodo di risoluzione non va bene: se volessi infatti utilizzare questo, dovrei porre $$f^{'}(x) = x+3$$ e $$g(x) = \frac{1}{\sqrt{x+2}}$$. Con questa scelta però, applicando la formula, nel nuovo integrale avrei $$g^{'}(x) = \frac{-\frac{1}{2\sqrt{x+2}}}{x+2} = -\frac{1}{2(x+2)\sqrt{x+2}}$$. Ossia non ottengo un integrale più facile rispetto a quello di partenza. 

Procediamo quindi per sostituzione. Come in quasi tutti i casi, sostituisco ciò che "mi dà fastidio", nel senso di quello che mi rende "difficile" l'integrale, ossia la radice: pongo

$$\sqrt{x+2} = t$$

Una volta individuata la sostituzione, la prima cosa da fare è trovare $$x$$ in funzione di $$t$$:

$$\begin{align*}
\sqrt{x+2} & = t \\
(\sqrt{x+2})^2 & = (t)^2 \\
x+2 & = t^2 \\
x & = t^2-2
\end{align*}$$

A questo punto, la seconda cosa da fare è calcolare $$dx$$: data in generale la relazione $$x = \star(t)$$, $$dx$$ sarà uguale alla derivata di $$\star(t)$$ rispetto a $$t$$ moltiplicata per $$dt$$.

Nel nostro caso, $$\star(t) = t^2-2$$. La sua derivata è $$D(t^2-2) = 2t$$. Quindi 

$$dx = D(t^2-2)dt = 2tdt$$

Abbiamo ora tutti gli elementi che ci servono per fare la sostituzione.

$$\begin{align*}
\int \frac{x+3}{\sqrt{x+2}}dx & = \int \frac{t^2-2+3}{t}\cdot 2tdt \\
& = \int \frac{2t(t^2+1)}{t}dt \\
& = \int 2(t^2+1)dt \\
& = 2 \int (t^2+1)dt \\
& = 2 \left[\int t^2dt + \int dt\right] \\
& = 2 \left[\frac{t^3}{3} + t \right] \\
& = 2t\left[\frac{t^2}{3}+1\right]
\end{align*}$$

Una volta che abbiamo risolto l'integrale in $$t$$, dobbiamo risostituire e riscrivere tutto in $$x$$:

$$\begin{align*}
2t\left[\frac{t^2}{3}+1\right] & = 2(\sqrt{x+2})\left[\frac{(\sqrt{x+2})^2}{3}+1\right] \\
& = 2\sqrt{x+2}\left[\frac{x+2}{3}+1\right] \\
& = 2\sqrt{x+2} \left[\frac{x+2+3}{3}\right] \\
& = \frac{2}{3}\sqrt{x+2}(x+5)
\end{align*}$$

Poichè l'integrale è indefinito, dobbiamo sempre aggiungere una costante $$c$$ alla fine. La soluzione è quindi 

$$\int \frac{x+3}{\sqrt{x+2}}dx = \frac{2}{3}\sqrt{x+2}(x+5) +c$$






