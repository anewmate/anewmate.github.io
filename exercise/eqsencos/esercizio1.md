# EQUAZIONI GONIOMETRICHE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente equazione

$$2\sin\left(x-\frac{\pi}{3}\right)-1 = 0$$

## Soluzione: 

Come prima cosa devo isolare il termine con il seno; porto quindi l'uno a destra e divido tutto per due.

$$\begin{align*}
2\sin\left(x-\frac{\pi}{3}\right)-1 & = 0 \\
2\sin\left(x-\frac{\pi}{3}\right) & = 1 \\
\sin\left(x-\frac{\pi}{3}\right) &= \frac{1}{2}
\end{align*}$$

Sono quindi arrivata a un'equazione della forma $$\sin(\alpha) = h$$, dove $$\alpha = x- \frac{\pi}{3}$$ e $$h = \frac{1}{2}$$. Ricordiamo che 

$$\sin(\alpha) = h \qquad \begin{cases}
\text{determinata se} & -1 \leq h \leq 1 \\
\text{impossibile se} & h < -1 \vee h > 1
\end{cases}$$

Dato che $$h = \frac{1}{2}$$ è compreso fra -1 e 1, l'equazione è determinata, ossia ha soluzione. Sostanzialmente ci stanno chiedendo qual è quell'angolo $$\alpha$$ che ha seno uguale a $$\frac{1}{2}$$. 

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

L'angolo che ha seno uguale a $$\frac{1}{2}$$ è $$\frac{\pi}{6}$$ e $$\frac{5}{6}\pi$$, ossia $$\sin\left( \frac{\pi}{6}\right) = \sin\left( \frac{5}{6}\pi\right) = \frac{1}{2}$$. Nel nostro caso quindi otteniamo 

$$\alpha = x - \frac{\pi}{3} = \frac{\pi}{6}$$

oppure 

$$\alpha = x - \frac{\pi}{3} = \frac{5}{6}\pi$$

Ricordiamo però che le funzioni seno e coseno sono funzioni periodiche: ciò significa che ogni $$360$$°, ossia $$2\pi$$, sono di nuovo nello stesso punto della circonferenza goniometrica. Le soluzioni sono quindi 

$$\begin{align*}
x - \frac{\pi}{3} & = \frac{\pi}{6} + 2k\pi \\
x  & = \frac{\pi}{6} + \frac{\pi}{3} + 2k\pi \\
& = \frac{3}{6}\pi + 2k\pi \\
& = \frac{1}{2}\pi + 2k\pi
\end{align*}$$

oppure 

$$\begin{align*}
x - \frac{\pi}{3} & = \frac{5}{6}\pi + 2k\pi \\
x  & = \frac{5}{6}\pi + \frac{\pi}{3} + 2k\pi \\
& = \frac{7}{6}\pi + 2k\pi
\end{align*}$$