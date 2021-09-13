# DISEQUAZIONI CON SENO E COSENO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Risolvi la seguente disequazione in $$[0,2\pi]$$

$$\sin\left(x-\frac{\pi}{3}\right) \geq 0$$

## Soluzione:

Che cosa ci sta chiedendo la disequazione? 

Sostanzialmente ci stiamo chiedendo quando il seno di un angolo è maggiore o uguale di zero. 

Ricordiamo quando il seno è positivo: guardando la circonferenza unitaria e ricordando che il seno di un angolo si legge sull'asse delle $$y$$, il seno è positivo per tutti gli angoli compresi fra $$0$$ e $$\pi$$ (in rosso in figura sotto). 

$$\begin{align*}
\sin(\text{\color{green}{angolo}} \; {\color{green}{\alpha}}) & \geq 0 \\
& \downarrow \\
0 \leq \color{green}{\text{angolo}} &  \; {\color{green}{\alpha}} \leq \pi
\end{align*}$$


$$\begin{tikzpicture}
\draw [->] (-2,0) -- (2,0);
\draw [->] (0,-2) -- (0,2);
\draw (0,0) circle (1cm);
\node at (1.2,-0.3) {1};
\node at (-1.2,-0.3) {-1};
\node at (0.3,1.2) {1};
\node at (0.3,-1.2) {-1};
%\draw [red,thick] (0,0) -- (0,-1);
\node at (-0.2,0.2) {\tiny $0$};
%\draw[fill=red] (0,0) circle (0.05cm);
\draw[fill=red] (1,0) circle (0.05cm);
\draw[fill=red] (-1,0) circle (0.05cm);
\draw[red] (1,0) arc (0:180:1);
\node [red] at (1.2,0.2) {\tiny $0$};
\node [red] at (-1.2,0.2) {\tiny $\pi$};
\end{tikzpicture}$$

Nel nostro caso quindi 

$$0 \leq x-\frac{\pi}{3} \leq \pi$$

Attenzione: non metto la periodicità (il $$+2k\pi$$) perchè il testo mi dice di risolvere la disquazione in $$[0,2\pi]$$. 

La prima parte della disquazione diventa: 

$$\begin{align*}
x - \frac{\pi}{3} & \geq 0 \\
x & \geq \frac{\pi}{3}
\end{align*}$$

mentre la seconda parte della disquazione diventa: 

$$\begin{align*}
x - \frac{\pi}{3} & \leq \pi \\
x & \leq \pi + \frac{\pi}{3} \\
x & \leq \frac{3\pi+\pi}{3} \\
x & \leq \frac{4}{3}\pi 
\end{align*}$$

La soluzione è quindi 

$$\frac{\pi}{3} \leq x \leq \frac{4}{3}\pi $$
