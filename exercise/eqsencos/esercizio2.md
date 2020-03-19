# EQUAZIONI GONIOMETRICHE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente equazione

$$\cos(3x) = -1 - \cos(3x)$$

## Soluzione: 

Come prima cosa devo isolare il termine con il coseno:

$$\begin{align*}
\cos(3x) & = -1 - \cos(3x) \\
\cos(3x) + \cos(3x) & = -1 \\
2\cos(3x) & = -1 \\
\cos(3x) & = -\frac{1}{2}
\end{align*}$$

Sono quindi arrivata a un'equazione della forma $$\cos(\alpha) = h$$, dove $$\alpha = 3x$$ e $$h = -\frac{1}{2}$$. Ricordiamo che 

$$\cos(\alpha) = h \qquad \begin{cases}
\text{determinata se} & -1 \leq h \leq 1 \\
\text{impossibile se} & h < -1 \vee h > 1
\end{cases}$$

Dato che $$h = -\frac{1}{2}$$ è compreso fra -1 e 1, l'equazione è determinata, ossia ha soluzione. Sostanzialmente ci stanno chiedendo qual è quell'angolo $$\alpha$$ che ha coseno uguale a $$-\frac{1}{2}$$. 

Memo: Circonferenza goniometrica

$$\begin{tikzpicture}
\draw [->] (-2,0) -- (2,0);
\draw [->] (0,-2) -- (0,2);
\draw (0,0) circle (1cm);
\node at (1.2,-0.3) {1};
\node at (-1.2,-0.3) {-1};
\node at (0.3,1.2) {1};
\node at (0.3,-1.2) {-1};
\draw (0,0) -- (1.73205080757/1.2,1/1.2);
\draw [red,thick] (1.73205080757/2,0) -- (1.73205080757/2,0.5);
\draw [green,thick] (0,0) -- (1.73205080757/2,0);
\node [green] at (0.5,-0.3) {\tiny $\cos(\alpha)$};
\node [red] at (1.5,0.3) {\tiny $\sin(\alpha)$};
\node at (0.35,0.1) {\tiny $\alpha$};
\end{tikzpicture}$$

L'angolo che ha coseno uguale a $$-\frac{1}{2}$$ è $$\frac{2}{3}\pi$$ e $$-\frac{2}{3}\pi$$, ossia $$\cos \left( \frac{2}{3}\pi\right) = \cos\left( -\frac{2}{3}\pi\right) = -\frac{1}{2}$$. Nel nostro caso quindi otteniamo 

$$\alpha = 3x = \frac{2}{3}\pi$$

oppure 

$$\alpha = 3x = -\frac{2}{3}\pi$$

Ricordiamo però che le funzioni seno e coseno sono funzioni periodiche: ciò significa che ogni $$360$$°, ossia $$2\pi$$, sono di nuovo nello stesso punto della circonferenza goniometrica. Le soluzioni sono quindi 

$$\begin{align*}
3x & = \frac{2}{3}\pi + 2k\pi \\
x & = \frac{2}{9}\pi + \frac{2}{3}k\pi
\end{align*}$$

oppure 

$$\begin{align*}
3x & = -\frac{2}{3}\pi + 2k\pi \\
x & = -\frac{2}{9}\pi + \frac{2}{3}k\pi
\end{align*}$$