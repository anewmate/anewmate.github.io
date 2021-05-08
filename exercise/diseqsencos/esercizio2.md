# DISEQUAZIONI CON SENO E COSENO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Risolvi la seguente disequazione in $$\mathbb{R}$$

$$2(\sin(x)+3)-1 < 3(1-\sin(x))+2$$

## Soluzione:

Come prima cosa svolgiamo i conti e sistemiamo la disequazione

$$\begin{align*}
2(\sin(x)+3)-1 & < 3(1-\sin(x))+2 \\
2\sin(x)+6-1 & < 3-3\sin(x)+2 \\
2\sin(x)+3\sin(x) & < -6+1+3+2 \\
5\sin(x) & < 0 \\
\frac{5\sin(x)}{5} & < \frac{0}{5} \\
\sin(x) & < 0 
\end{align*}$$

Ci stiamo quindi chiedendo quando il seno è negativo. 

Risolviamo prima l'equazione associata: 

$$\sin(x) = 0$$

Nella circonferenza unitaria, gli angoli che hanno seno uguale a zero sono l'angolo $$0$$ e $$\pi$$. 

$$\sin(x) = 0 \rightarrow x = 0 \; \vee \; x = \pi$$

Poichè il seno si legge sull'asse delle $$y$$, devo prendere tutti quegli angoli che vanno da $$\pi$$ a $$2\pi$$, ossia che hanno $$y$$ negativa (in rosso nel grafico di seguito).

$$\begin{tikzpicture}
\draw [->] (-2,0) -- (2,0);
\draw [->] (0,-2) -- (0,2);
\draw (0,0) circle (1cm);
\node at (1.2,-0.3) {1};
\node at (-1.2,-0.3) {-1};
\node at (0.3,1.2) {1};
\node at (0.3,-1.2) {-1};
\draw [red,thick] (0,0) -- (0,-1);
\node at (-0.2,0.2) {\tiny $0$};
\draw[fill=red] (0,0) circle (0.05cm);
\draw[fill=red] (1,0) circle (0.05cm);
\draw[fill=red] (-1,0) circle (0.05cm);
\draw[red] (1,0) arc (0:-180:1);
\node [red] at (1.2,0.2) {\tiny $0$};
\node [red] at (-1.2,0.2) {\tiny $\pi$};
\end{tikzpicture}$$

La prima soluzione trovata per $$\sin(x) < 0$$ è quindi 

$$\pi < x < 2\pi$$

Poichè il seno è una funzione periodica, dobbiamo tenere conto che ritroviamo le soluzioni ogni giro della circonferenza, ossia ogni $$2\pi$$. Quindi, la soluzione finale è

$$\pi + 2k\pi < x < 2\pi + 2k\pi$$

con $$k = 0,1,2,3,\dots$$

