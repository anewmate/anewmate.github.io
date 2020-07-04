# DISEQUAZIONI LOGARITMICHE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Risolvi la seguente disequazione

$$\log_3\left(\log_3(x+1)\right) < 0 $$

## Soluzione: 

Come prima cosa devo imporre le condizioni di esistenza (C.E.): affinchè la disequazione abbia senso tutti i logaritmi devono esistere, e ciò avviene quando i loro argomenti sono positivi. 

$$\begin{align*}
\text{C.E.:} & \qquad \begin{cases}
\log_3(x+1) > 0 \\
x+1 > 0 
\end{cases} 
\end{align*}
$$

La prima condizione serve per l'esistenza del logaritmo "più esterno", mentre la seconda condizione serve per l'esistenza del logaritmo "più interno". In altre parole

$$\textcolor{red}{\log_3}\left(\log_3(x+1)\right)$$ ha come $$\textcolor{red}{\text{argomento}} \; \log_3(x+1)$$ che quindi deve essere positivo. 

$$\log_3\left(\textcolor{green}{\log_3}(x+1)\right)$$ ha come $$\textcolor{green}{\text{argomento}}$$ $$x+1$$ che quindi deve essere positivo. 

Risolviamo la prima disequazione.

$$\begin{align*}
\log_3(x+1) & > 0 \\
x+1 & > 3^0 \\
x+1 & > 1 \\
x & > 0
\end{align*}$$

Le condizioni di esistenza sono quindi 

$$\begin{align*}
\text{C.E.:} & \qquad \begin{cases}
x > 0 \\
x > -1 
\end{cases} 
\end{align*}
\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (0,1) rectangle (2,0);
\draw (-2,0) -- (2,0);
\draw[dashed] (-1,0.5) -- (-1,-0.2);
\draw[dashed] (0,1) -- (0,-0.2);
\node at (-1,-0.5) {$-1$};
\node at (0,-0.5) {$0$};
\draw (-1,0.5) -- (2,0.5);
\draw (0,1) -- (2,1);
\draw[black] (-1,0.5) circle (1.5pt);
\draw[black] (0,1) circle (1.5pt);
\end{tikzpicture}
\begin{align*}
\text{C.E.:} & \qquad x > 0
\end{align*}
$$

Una volta trovate le condizioni di esistenza, posso andare a risolvere la disequazione. Poichè la base del logaritmo è un numero maggiore di $$1$$, nel momento in cui "tolgo il logaritmo" il verso della disuguaglianza non cambia. 

$$\begin{align*}
\log_3\left(\log_3(x+1)\right) & < 0 \\
\log_3(x+1) & < 3^0 \\
\log_3(x+1) & < 1 \\
x+1 & < 3^1 \\
x & < 3-1 \\
x & < 2
\end{align*}$$ 

L'ultimo step da fare è intersecare la soluzione trovata con le C.E.:

$$\begin{cases}
x > 0 \\
x < 2
\end{cases}$$

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (0,1) rectangle (2,0);
\draw (-2,0) -- (4,0);
\draw[dashed] (0,1) -- (0,-0.2);
\draw[dashed] (2,0.5) -- (2,-0.2);
\node at (0,-0.5) {$0$};
\node at (2,-0.5) {$2$};
\draw (0,1) -- (4,1);
\draw (-2,0.5) -- (2,0.5);
\draw[black] (0,1) circle (1.5pt);
\draw[black] (2,0.5) circle (1.5pt);
\end{tikzpicture}$$

La soluzione è quindi 

$$0 < x < 2$$



