# EQUAZIONI DIFFERENZIALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Risolvi la seguente equazione differenziale

$$x^3y^{'}-2x-1 = 0$$

## Soluzione:

Come prima cosa isoliamo la derivata di $$y$$:

$$\begin{align*}
x^3y^{'}-2x-1 & = 0 \\
x^3y^{'} & = 2x+1 \\
y^{'} & = \frac{2x+1}{x^3} \\
y^{'} & = \frac{2x}{x^3} + \frac{1}{x^3} \\
y^{'} & = \underbrace{\frac{2}{x^2} + \frac{1}{x^3}}_{\text{funzione che dipende solo da x}}
\end{align*}$$

Siamo quindi di fronte a un'equazione differenziale del tipo 

$$y^{'} = f(x)$$

dove, nel nostro caso, $$f(x) = \frac{2}{x^2} + \frac{1}{x^3}$$.

Per risolverla basta integrare destra e sinistra **rispetto a $$\mathbf{x}$$**, ossia fare l'integrale in $$dx$$:

$$\begin{align*}
y^{'} & = \frac{2}{x^2} + \frac{1}{x^3} \\
\int y^{'} dx & = \int \left(\frac{2}{x^2} + \frac{1}{x^3}\right)dx \\
y & = \int \frac{2}{x^2}dx + \int \frac{1}{x^3}dx \\
& = 2 \int x^{-2} dx + \int x^{-3}dx \\
& = 2 \cdot \frac{x^{-1}}{-1} + \frac{x^{-2}}{-2} +c\\
& = -2x^{-1} -\frac{1}{2}x^{-2} +c\\
& = -\frac{2}{x} - \frac{1}{2x^2}+c
\end{align*}$$

Le soluzioni sono quindi tutte le funzioni del tipo 

$$y = -\frac{2}{x} - \frac{1}{2x^2}+c$$

**Nota** sul perchè prendo l'integrale in $$x$$: 

Sappiamo che scrivere $$y$$ o scrivere $$f(x)$$ è lo stesso: modi diversi per scrivere la stessa identica cosa. Quindi, quando considero la derivata, che posso indicare con $$'$$ oppure $$D$$ oppure $$\frac{d}{dx}$$, scrivere $$y^{'}$$ equivale a scrivere $$f^{'}(x)$$. Siccome l'obiettivo del problema è trovare $$y$$, ossia $$f(x)$$, nel momento in cui ho un'equazione del tipo

$$y^{'} = \text{funzione di x}$$

ossia 

$$f^{'}(x) = \text{funzione di x}$$

a sinistra dell'uguale ottengo $$f(x)$$ solo se considero l'integrale rispetto a $$x$$. In quel caso infatti, per il termine a sinistra dell'uguale ho 

$$\int y^{'} dx = \int f^{'}(x) dx = f(x) = y$$

proprio per definizione di integrale. Se prendessi l'integrale rispetto a $$y$$ otterei

$$\int \underbrace{f^{'}(x)}_{\text{non dipende da y}} dy = f^{'}(x) \int 1 \cdot dy = f^{'}(x) y$$

Dato che $$f^{'}(x)$$ non dipende da $$y$$ ($$f^{'}(x)$$ è una funzione di $$x$$, non di $$y$$) è come se fosse una costante che posso portare fuori dall'integrale. In questo caso non ottengo neanche lontanamente quello che mi interessa, ossia $$f(x)$$.

**Nota**: volendo essere rigorosi al 100%, poichè ogni integrale che risolvo è indefinito, avrei 

$$\begin{align*}
y^{'} & = \frac{2}{x^2} + \frac{1}{x^3} \\
\int y^{'} dx & = \int \left(\frac{2}{x^2} + \frac{1}{x^3}\right)dx \\
y +c_1 & = \int \frac{2}{x^2}dx + \int \frac{1}{x^3}dx \\
y +c_1 & = 2 \int x^{-2} dx + \int x^{-3}dx \\
y +c_1 & = 2 \cdot \frac{x^{-1}}{-1} +c_2 + \frac{x^{-2}}{-2} +c_3\\
y +c_1 & = -2x^{-1} -\frac{1}{2}x^{-2} +c_2+c_3\\
y +c_1 & = -\frac{2}{x} - \frac{1}{2x^2}+c_2+c_3 \\
y & = -\frac{2}{x} - \frac{1}{2x^2}+\underbrace{c_2+c_3-c_1}_{= c}
\end{align*}$$

Poichè la somma (e sottrazione) di costanti è una costante, scrivo sempre solo una cosante $$c$$ quando risolvo l'integrale a destra dell'uguaglianza. 



