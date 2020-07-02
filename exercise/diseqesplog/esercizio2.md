# DISEQUAZIONI LOGARITMICHE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Risolvi la seguente disequazione

$$\log_3(x^2-2x) > 1$$

## Soluzione: 

Come prima cosa devo imporre le condizioni di esistenza (C.E.): affinchè la disequazione abbia senso il logaritmo deve esistere, e ciò avviene quando il suo argomento è positivo. 

$$\begin{align*}
\text{C.E.:} & \qquad x^2-2x > 0 
\end{align*}
\begin{align*}
x^2-2x & > 0 \\
x(x-2) & > 0 \\
 & \downarrow \\
\text{equazione}  & \; \; \text{associata} \\
x(x-2) & = 0 \\
x = 0 \; & \vee \; x = 2 \\
& \downarrow \\
\text{poichè avevo} & >, \; \text{intervalli esterni} \\
x < 0 \; & \cup \; x > 2
\end{align*}
\begin{align*}
\text{C.E.:} & \qquad x < 0 \; \cup \; x > 2
\end{align*}$$

Una volta trovate le condizioni di esistenza, posso andare a risolvere la disequazione. Poichè la base del logaritmo è un numero maggiore di $$1$$, nel momento in cui "tolgo il logaritmo" il verso della disuguaglianza non cambia. 

$$\begin{align*}
\log_3(x^2-2x) & > 1 \\
x^2-2x & > 3^1 \\
x^2-2x-3 & > 0 \\
& \downarrow \\
\text{equazione}  & \; \; \text{associata} \\
x^2-2x-3 & = 0 \\
x_{1/2} & = \frac{2\pm \sqrt{4+12}}{2} = \frac{2\pm 4}{2}\\
x = 3 \; & \vee \; x = -1 \\
& \downarrow \\
\text{poichè avevo} & >, \; \text{intervalli esterni} \\
x < -1 \; & \cup \; x > 3
\end{align*}$$ 

L'ultimo step da fare è intersecare le soluzioni trovate con le C.E.:

$$\begin{cases}
x < -1 \; & \cup \; \; \; x > 3 \\
x < 0 \; & \cup \; \; \; x > 2
\end{cases}$$

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (-2,1) rectangle (-1,0);
\shade[left color=yellow, right color = yellow] (3,1) rectangle (4,0);
\draw (-2,0) -- (4,0);
\draw[dashed] (-1,1) -- (-1,-0.2);
\draw[dashed] (0,0.5) -- (0,-0.2);
\draw[dashed] (2,0.5) -- (2,-0.2);
\draw[dashed] (3,1) -- (3,-0.2);
\node at (-1,-0.5) {$-1$};
\node at (0,-0.5) {$0$};
\node at (2,-0.5) {$2$};
\node at (3,-0.5) {$3$};
\draw (-2,1) -- (-1,1);
\draw (3,1) -- (4,1);
\draw (-2,0.5) -- (0,0.5);
\draw (2,0.5) -- (4,0.5);
\draw[black] (-1,1) circle (1.5pt);
\draw[black] (0,0.5) circle (1.5pt);
\draw[black] (2,0.5) circle (1.5pt);
\draw[black] (3,1) circle (1.5pt);
\end{tikzpicture}$$

La soluzione è quindi 

$$x < -1 \; \cup \; x > 3$$



