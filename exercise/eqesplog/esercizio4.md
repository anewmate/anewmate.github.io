# EQUAZIONI LOGARITMICHE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Risolvi la seguente equazione

$$\frac{\ln(x)-2}{\ln(x)+1} + \frac{\ln(x)+1}{\ln(x)} = \frac{2\ln(x)+5}{2\ln(x)+2}$$

## Soluzione: 

Come prima cosa devo imporre le condizioni di esistenza (C.E.): affinchè l'equazione abbia senso tutte le frazioni e tutti i logaritmi devono esistere, e ciò avviene quando tutti i denominatori sono diversi da zero e quando tutti gli argomenti dei logaritmi sono positivi. 

$$\begin{align*}
\text{C.E.:} & \qquad \begin{cases}
x > 0 \\
\ln(x)+1 \neq 0 \\
\ln(x) \neq 0 \\
2\ln(x)+2 \neq 0
\end{cases} \\
\text{C.E.:} & \qquad \begin{cases}
x > 0 \\
\ln(x) \neq -1 \\
\ln(x) \neq 0 \\
\ln(x) \neq -1
\end{cases} \\
\text{C.E.:} & \qquad \begin{cases}
x > 0 \\
x \neq e^{-1} \\
x \neq e^0
\end{cases} \\
\text{C.E.:} & \qquad \begin{cases}
x > 0 \\
x \neq \frac{1}{e} \\
x \neq 1
\end{cases} 
\end{align*}
\begin{tikzpicture}
\shade[left color=yellow, right color = yellow] (1,1.5) rectangle (2.48,0);
\shade[left color=yellow, right color = yellow] (2.52,1.5) rectangle (3.98,0);
\shade[left color=yellow, right color = yellow] (4.02,1.5) rectangle (5,0);
\draw (0,0) -- (5,0);
\draw[dashed] (1,0.5) -- (1,-0.2);
\draw[dashed] (2.5,1) -- (2.5,-0.2);
\draw[dashed] (4,1.5) -- (4,-0.2);
\node at (1,-0.5) {$0$};
\node at (2.5,-0.5) {$\frac{1}{e}$};
\node at (4,-0.5) {$1$};
\draw (1,0.5) -- (5,0.5);
\draw (0,1) -- (5,1);
\draw (0,1.5) -- (5,1.5);
\draw[black] (1,0.5) circle (1.5pt);
\draw[black] (2.5,1) circle (1.5pt);
\draw[black] (4,1.5) circle (1.5pt);
\end{tikzpicture}
\begin{align*}
\text{C.E.:} & \qquad x > 0, x \neq \frac{1}{e}, x \neq 1
\end{align*}$$

Una volta trovate le condizioni di esistenza, posso andare a risolvere l'equazione. In questo caso noto che i logaritmi all'interno dell'equazione sono tutti uguali e pari a $$\ln(x)$$: posso quindi procedere per sostituzione. Pongo 

$$t = \ln(x)$$

e riscrivo l'equazione in $$t$$:

$$\frac{t-2}{t+1} + \frac{t+1}{t} = \frac{2t+5}{2t+2}$$

Abbiamo quindi trasformato la nostra equazione logaritmica in $$x$$ in un'equazione fratta di primo grado in $$t$$. Andiamo a risolverla facendo denominatore comune.

$$\frac{2t(t-2)+2(t+1)(t+1)}{2t(t+1)} = \frac{t(2t+5)}{2t(t+1)}$$

$$2t(t+1) \cdot \frac{2t(t-2)+2(t+1)(t+1)}{2t(t+1)} = \frac{t(2t+5)}{2t(t+1)} \cdot 2t(t+1)$$

$$2t(t-2)+2(t+1)(t+1) = t(2t+5)$$

$$2t^2-4t+2t^2+4t+2 = 2t^2+5t$$

$$2t^2-5t+2 = 0$$

$$t_{1/2} = \frac{+5\pm\sqrt{25-16}}{4} = \frac{5\pm 3}{4}$$

Abbiamo quindi trovato due soluzioni in $$t$$: $$t = \frac{1}{2}$$ e $$t = 2$$.

Noi però stavamo cercando soluzioni in $$x$$ e non in $$t$$: devo quindi tornare indietro e ricordarmi che avevo posto $$t = \ln(x)$$.

Da $$t = \frac{1}{2}$$ ottengo

$$\begin{align*}
\ln(x) & = \frac{1}{2} \\
x & = e^{\frac{1}{2}} = \sqrt{e}
\end{align*}$$

mentre da $$t = 2$$ ottengo 

$$\begin{align*}
\ln(x) & = 2 \\
x & = e^{2} 
\end{align*}$$

L'ultimo step da fare è controllare se effettivamente le soluzioni che abbiamo trovato sono compatibili con le C.E.. Dato che $$x = \sqrt{e}$$ e $$x = e^2$$ sono entrambe maggiori di zero e diverse da $$\frac{1}{e}$$ e $$1$$, sono entrambe soluzioni accettabili. L'equazione ha quindi due soluzioni

$$\begin{align*}
x & = \sqrt{e} \\
x & = e^{2} 
\end{align*}$$


