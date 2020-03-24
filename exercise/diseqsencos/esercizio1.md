# DISEQUAZIONI CON SENO E COSENO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente disequazione

$$4\cos^2(x) +4\cos(x) -3 \geq 0$$

## Soluzione:

Come prima cosa risolviamo l'equazione associata

$$4\cos^2(x) +4\cos(x) -3 = 0$$

Se poniamo $$\cos(x) = t$$ otteniamo 

$$4t^2 +4t - 3 = 0$$

e possiamo applicare la formula risolutiva per le equazioni di secondo grado. Visto che il termine di primo grado ha coefficiente pari, utilizziamo la formula con $$\frac{\Delta}{4}$$: ricordiamo la formula per l'equazione generale $$ax^2+bx+c = 0$$ con $$a\neq 0$$ e $$b$$ pari.

$$x_{1/2} = \frac{-\frac{b}{2}\pm \sqrt{\left(-\frac{b}{2}\right)^2 - ac}}{a}$$

Nel nostro caso quindi abbiamo

$$\begin{align*}
t_{1/2} & = \frac{-2 \pm \sqrt{4-(4)(-3)}}{4} \\
& = \frac{-2 \pm \sqrt{4+12}}{4} \\
& = \frac{-2 \pm 4}{4} \\
& = \begin{cases}
\frac{1}{2} \\
-\frac{3}{2}
\end{cases}
\end{align*}$$

Abbiamo quindi ottenuto $$t = \cos(x) = \frac{1}{2}$$ e $$t = \cos(x) = - \frac{3}{2}$$. 

Dallo studio delle disequazioni di secondo grado sappiamo che la disequazione $$4\cos^2(x) +4\cos(x) -3 \geq 0$$ è soddisfatta per i valori esterni all'intervallo delle soluzioni dell'equazione associata, cioè

$$\cos(x) \leq - \frac{3}{2} \ \cup \ \cos(x) \geq \frac{1}{2}$$

Rappresentiamo graficamente sulla circonferenza goniometrica ciò che abbiamo trovato. 

Spendiamo subito due parole sulla prima disuguaglianza, $$\cos(x) \leq - \frac{3}{2}$$: per definizione di coseno, sappiamo che esso è sempre incluso fra -1 e 1, ossia $$-1\leq \cos(x) \leq 1$$. Poichè $$-\frac{3}{2} < -1$$, il coseno non può mai essere minore di $$-\frac{3}{2}$$; questa disequazione è quindi impossibile, ossia $$\nexists \; x  \in \mathbb{R}$$ tale che $$\cos(x) \leq - \frac{3}{2}$$.

Per la seconda disequazione, ricordiamo che l'angolo che ha coseno uguale a $$\frac{1}{2}$$ è $$\frac{\pi}{3}$$. 

$$\begin{tikzpicture}
\draw [->] (-2,0) -- (2,0);
\draw [->] (0,-2) -- (0,2);
\draw (0,0) circle (1cm);
\node at (1.2,-0.3) {1};
\node at (-1.2,-0.3) {-1};
\node at (0.3,1.2) {1};
\node at (0.3,-1.2) {-1};
\draw (0,0) -- (0.5,1.73205080757/2);
\draw (0,0) -- (0.5,-1.73205080757/2);
\draw[dashed] (0.5,-1.73205080757/2)--(0.5,1.73205080757/2);
\draw [red,thick] (0.5,0) -- (1,0);
\node at (0.4,-0.2) {\tiny $\frac{1}{2}$};
\draw[fill=red] (0.5,0) circle (0.05cm);
\draw[fill=red] (0.5,1.73205080757/2) circle (0.05cm);
\draw[fill=red] (0.5,-1.73205080757/2) circle (0.05cm);
\draw[red] (0.5,1.73205080757/2) arc (60:-60:1);
\node [red] at (0.8,1.73205080757/2) {\tiny $\frac{\pi}{3}$};
\node [red] at (0.9,-1.73205080757/2) {\tiny $-\frac{\pi}{3}$};
\end{tikzpicture}$$

Quindi $$\cos(x) \geq \frac{1}{2}$$ se 

$$-\frac{\pi}{3} \leq x \leq \frac{\pi}{3}$$

Poichè il coseno è una funzione periodica, dobbiamo tenere conto che ritroviamo le soluzioni ogni giro della circonferenza, ossia ogni $$2\pi$$. Quindi, la soluzione finale è

$$-\frac{\pi}{3} + 2k\pi \leq x \leq \frac{\pi}{3} + 2k\pi$$

