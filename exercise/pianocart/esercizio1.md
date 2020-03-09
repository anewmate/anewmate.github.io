# PIANO CARTESIANO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> I punti $$A(2;1)$$ e $$B(6;4)$$ sono vertici del triangolo $$ABC$$. Sapendo che $$M\left(\frac{1}{2};-1\right)$$ è il punto medio del lato $$AC$$, determina le coordinate di $$C$$ e il perimetro del triangolo.

## Soluzione: 

Come prima cosa grafichiamo i dati del problema:

$$\begin{tikzpicture}
\draw[->] (-1,0) -- (7,0);
\draw[->] (0,-1.5) -- (0,4.5);
\draw[fill=black] (2,1) circle (2pt);
\draw[fill=black] (6,4) circle (2pt);
\draw[fill=black] (1/2,-1) circle (2pt);
\node at (1.5,1) {A};
\node at (5.7,4.3) {B};
\node at (0.9,-1) {M};
\end{tikzpicture}
$$

Ricordiamo la formula del punto medio:

> Il punto medio del segmento $$AB$$ è $$M(x_M;y_M)$$ dove

$$x_M = \frac{x_A + x_B}{2}, \qquad y_M = \frac{y_A + y_B}{2}$$

Tradotta nel nostro caso diventa: il punto medio del segmento $$AC$$ è $$M(x_M;y_M)$$ dove

$$x_M = \frac{x_A + x_C}{2}, \qquad y_M = \frac{y_A + y_C}{2}$$

Nel nostro caso $$x_M = \frac{1}{2}$$, $$y_M = -1$$, $$x_A = 2$$, $$y_A = 1$$. Quindi, usando le formule appena scritte ho 

$$\frac{1}{2} = \frac{2 + x_C}{2}, \qquad -1 = \frac{1 + y_C}{2}$$

L'equazione per $$x_C$$ diventa, moltiplicando destra e sinistra per $$2$$:

$$1 = 2 + x_C \qquad \rightarrow \qquad x_C = 1-2 = -1$$

L'equazione per $$y_C$$ diventa, moltiplicando destra e sinistra per $$2$$:

$$-2 = 1 + y_C \qquad \rightarrow \qquad y_C = -2 - 1 = -3$$

Il punto $$C$$ ha quindi coordinate $$C(-1,-3)$$.

Il tringolo è quindi

$$\begin{tikzpicture}
\draw[->] (-1.5,0) -- (7,0);
\draw[->] (0,-3.5) -- (0,4.5);
\draw[fill=black] (2,1) circle (2pt);
\draw[fill=black] (6,4) circle (2pt);
\draw[fill=black] (1/2,-1) circle (2pt);
\draw[fill=black] (-1,-3) circle (2pt);
\node at (1.5,1) {A};
\node at (5.7,4.3) {B};
\node at (0.9,-1) {M};
\node at (-1.4,-3) {C};
\draw[red] (-1,-3) -- (2,1);
\draw[red] (2,1) -- (6,4);
\draw[red] (6,4) -- (-1,-3); 
\end{tikzpicture}
$$

Per calcolare il perimetro detro trovare la lunghezza di ogni segmento. Ricordiamo la formula della lunghezza di un segmento:

> La distanza fra due punti $$A(x_A;y_A)$$ e $$B(x_B;y_B)$$ è data da 

$$\overline{AB} = \sqrt{(x_B-x_A)^2 + (y_B-y_A)^2}$$

Quindi, 

$$\begin{align*}
\overline{AB}  & = \sqrt{(x_B-x_A)^2 + (y_B-y_A)^2} = \sqrt{(6-2)^2 + (4-1)^2} = \sqrt{25} = 5 \\
\overline{AC} & = \sqrt{(x_C-x_A)^2 + (y_C-y_A)^2} = \sqrt{(-1-2)^2 + (-3-1)^2} = \sqrt{25} = 5\\
\overline{BC} & = \sqrt{(x_C-x_B)^2 + (y_C-y_B)^2} = \sqrt{(-1-6)^2 + (-3-4)^2} = \sqrt{98} = 7\sqrt{2}\\
\end{align*}$$ 

Il perimetro è quindi:

$$5+5+7\sqrt{2} = 10 + 7\sqrt{2}$$

Nota: $$\sqrt{98} = \sqrt{7^2 \cdot 2} = \sqrt{7^2} \cdot \sqrt{2} = 7 \sqrt{2}$$
