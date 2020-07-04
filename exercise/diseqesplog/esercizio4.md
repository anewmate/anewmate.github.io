# DISEQUAZIONI LOGARITMICHE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Risolvi la seguente disequazione

$$\log_{\frac{1}{3}}^2(x) -4\log_{\frac{1}{3}}(x) +3 < 0 $$

## Soluzione: 

Come prima cosa devo imporre le condizioni di esistenza (C.E.): affinchè la disequazione abbia senso tutti i logaritmi devono esistere, e ciò avviene quando i loro argomenti sono positivi. 

$$\begin{align*}
\text{C.E.:} & \qquad x > 0
\end{align*}
$$

Una volta trovate le condizioni di esistenza, posso andare a risolvere la disequazione. Noto subito che la base del logaritmo è minore di $$1$$, quindi nel momento in cui andrò a "togliere il logaritmo" devo ricordarmi di cambiare il verso della disuguaglianza. 

Noto anche che i logaritmi all'interno della disequazione sono tutti pari a $$\log_{\frac{1}{3}}(x)$$: procedo quindi per sostituzione. Pongo

$$t = \log_{\frac{1}{3}}(x)$$

e riscrivo la disequazione in $$t$$:

$$t^2-4t+3 < 0 $$ 

Ho trasformato quindi la mia disequazione logaritmica in $$x$$ in una disequazione di secondo grado in $$t$$. Vado a risolverla. 

$$\begin{align*}
t^2 -4t +3 & < 0 \\
& \downarrow \\
\text{equazione}  & \; \text{associata:} \\
t^2-4t+3 & = 0 \\
t_{1/2} & = \frac{4 \pm \sqrt{16-12}}{2} \\
& = \frac{4 \pm 2}{2} \\
t = 3 & \vee t = 1 \\
& \downarrow \\
\text{poichè avevo} \; < & \; \text{, intervallo interno: } \\
1 < t & < 3
\end{align*}$$ 

Ora che abbiamo trovato la soluzione in $$t$$, dobbiamo tornare indietro e trovare la soluzione in $$x$$.

$$\begin{align*}
1 < & \; t  < 3 \\
& \downarrow \\
1 < & \log_{\frac{1}{3}}(x)  < 3 
\end{align*}$$ 

che è equivalente a

$$\begin{cases}
\log_{\frac{1}{3}}(x) > 1  \\
\log_{\frac{1}{3}}(x) < 3
\end{cases}$$

Risolvo la prima disequazione del sistema. 

$$\begin{align*}
\log_{\frac{1}{3}}(x)  & > 1 \\
x & < \left(\frac{1}{3}\right)^1 \\
x & < \frac{1}{3}
\end{align*}$$ 

dove nel primo passaggio cambio il verso della disuguaglianza perchè la base del logaritmo è un numero minore di $$1$$.

Risolvo la seconda disequazione del sistema. 

$$\begin{align*}
\log_{\frac{1}{3}}(x)  & < 3 \\
x & > \left(\frac{1}{3}\right)^3 \\
x & > \frac{1}{27}
\end{align*}$$ 

Rimetto insieme il sistema:

$$\begin{cases}
x < \frac{1}{3}  \\
x > \frac{1}{27}
\end{cases}$$

ossia $$\frac{1}{27} < x < \frac{1}{3}$$. 

L'ultimo step da fare è intersecare la soluzione trovata con le C.E.:

$$\begin{cases}
x > 0 \\
\frac{1}{27} < x < \frac{1}{3}
\end{cases}$$

$$\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (1,1) rectangle (3,0);
\draw (-1,0) -- (4,0);
\draw[dashed] (0,1) -- (0,-0.2);
\draw[dashed] (3,0.5) -- (3,-0.2);
\draw[dashed] (1,0.5) -- (1,-0.2);
\node at (0,-0.5) {$0$};
\node at (3,-0.5) {$\frac{1}{3}$};
\node at (1,-0.5) {$\frac{1}{27}$};
\draw (0,1) -- (4,1);
\draw (1,0.5) -- (3,0.5);
\draw[black] (0,1) circle (1.5pt);
\draw[black] (3,0.5) circle (1.5pt);
\draw[black] (1,0.5) circle (1.5pt);
\end{tikzpicture}$$

La soluzione è quindi 

$$\frac{1}{27} < x < \frac{1}{3}$$



