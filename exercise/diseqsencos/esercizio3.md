# DISEQUAZIONI CON SENO E COSENO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Risolvi la seguente disequazione in $$[0,2\pi]$$

$$\frac{2\sin^2(x)-1}{\cos(x)} \leq 0$$

## Soluzione:

Come prima cosa vediamo che la disequazione, oltre a contenere seni e coseni, è più in generale una **disequazione fratta** dal momento che l'incognita $$x$$ compare anche a denominatore oltre che a numeratore. 

Come si risolvono le disequazioni fratte? Dopo essere arrivati a una forma del tipo $$\frac{A(x)}{B(x)} \gtrless 0$$ (ossia la nostra disequazione) si procede con lo studio del segno di numeratore, denominatore e alla fine della frazione. 

### Studio del numeratore

Andiamo a studiare quando il numeratore è positivo:

$$\begin{align*}
2\sin^2(x) - 1 & \geq 0 \\
2\sin^2(x) & \geq 1 \\
\frac{2\sin^2(x)}{2} & \geq \frac{1}{2} \\
\sin^2(x) & \geq \frac{1}{2}
\end{align*}$$

Se pensiamo a $$\sin(x)$$ come a un'unica variabile, siamo sostanzialmente di fronte a una disequazione di secondo grado tipo $$t^2 \geq \frac{1}{2}$$. Risolviamo quindi l'equazione associata:

$$\sin^2(x) = \frac{1}{2} \rightarrow \sin(x) = \pm \frac{1}{\sqrt{2}}$$

Poichè avevamo $$\geq$$, prendo gli intervalli esterni:

$$\sin(x) \leq -\frac{1}{\sqrt{2}} \; \; \vee \; \; \sin(x) \geq \frac{1}{\sqrt{2}}$$

Quali sono gli angoli che hanno seno uguale a $$\pm\frac{1}{\sqrt{2}}$$? 

$$\sin(x) = \frac{1}{\sqrt{2}} \rightarrow x = \frac{\pi}{4} \vee x = \frac{3}{4}\pi$$

$$\sin(x) = -\frac{1}{\sqrt{2}} \rightarrow x = \frac{5}{4}\pi \vee x = \frac{7}{4}\pi$$

Attenzione: nell'ultima equazione non scrivo $$x = -\frac{3}{4}\pi \vee x = -\frac{\pi}{4}$$ (che sarebbe stato giusto) in quanto mi viene richiesto di risolvere l'equazione in $$[0,2\pi]$$.  

Poichè il seno si legge sull'asse delle $$y$$, devo prendere tutti quegli angoli che sono compresi fra gli estremi che ho trovato (in rosso nel grafico di seguito), ossia che hanno seno maggiore di $$\frac{1}{\sqrt{2}}$$ e minore di $$-\frac{1}{\sqrt{2}}$$.

$$\begin{tikzpicture}
\draw [->] (-2,0) -- (2,0);
\draw [->] (0,-2) -- (0,2);
\draw (0,0) circle (1cm);
\node at (1.2,-0.2) {\tiny 1};
\node at (-1.2,-0.2) {\tiny -1};
\node at (0.2,1.2) {\tiny 1};
\node at (0.2,-1.2) {\tiny -1};
\node at (1.7,0.3) {\tiny $\textcolor{green}{\frac{1}{\sqrt{2}}}$};
\node at (-1.9,-0.4) {\tiny $\textcolor{green}{-\frac{1}{\sqrt{2}}}$};
\draw [green] (0,0.70710678118) -- (0,0);
\draw [green] (0,-0.70710678118) -- (0,0);
\draw [->,green] (1.4,0.3) -- (0.2,0.3);
\draw [->,green] (-1.4,-0.4) -- (-0.2,-0.4);
\draw [red] (0,0.70710678118) -- (0,1);
\draw [red] (0,-0.70710678118) -- (0,-1);
\draw [dashed] (-0.70710678118,0.70710678118) -- (0.70710678118,0.70710678118);
\draw [dashed] (-0.70710678118,-0.70710678118) -- (0.70710678118,-0.70710678118);
\draw [ultra thin] (0,0) -- (0.70710678118,0.70710678118);
\draw [ultra thin] (0,0) -- (-0.70710678118,0.70710678118);
\draw [ultra thin] (0,0) -- (-0.70710678118,-0.70710678118);
\draw [ultra thin] (0,0) -- (0.70710678118,-0.70710678118);
\draw[fill=red] (0.70710678118,0.70710678118) circle (0.05cm);
\draw[fill=red] (0.70710678118,-0.70710678118) circle (0.05cm);
\draw[fill=red] (-0.70710678118,0.70710678118) circle (0.05cm);
\draw[fill=red] (-0.70710678118,-0.70710678118) circle (0.05cm);
%\draw[red] (0,0) arc (-45:-135:1);
\draw [red,domain=-135:-45] plot ({cos(\x)}, {sin(\x)});
\draw [red,domain=45:135] plot ({cos(\x)}, {sin(\x)});
\node [red] at (1,0.707) {\tiny $\frac{\pi}{4}$};
\node [red] at (-1.2,0.707) {\tiny $\frac{3}{4}\pi$};
\node [red] at (1.1,-0.707) {\tiny $\frac{7}{4}\pi$};
\node [red] at (-1.2,-0.74) {\tiny $\frac{5}{4}\pi$};
\end{tikzpicture}$$

Abbiamo quindi trovato che il numeratore è positivo per 

$$\frac{\pi}{4} \leq x \leq \frac{3}{4}\pi \; \;  \vee \; \; \frac{5}{4}\pi \leq x \leq \frac{7}{4}\pi$$

### Studio del denominatore

Fortunatamente il denominatore è facile in quanto sappiamo che il coseno è positivo nel primo e quarto quadrante: 

$$\cos(x) > 0 \rightarrow -\frac{\pi}{2} < x < \frac{\pi}{2}$$

Attenzione: poichè mi viene chiesto di risolvere l'equazione in $$[0,2\pi]$$, devo riscrivere la soluzione come 

$$-\frac{\pi}{2} < x < \frac{\pi}{2} \; \text{equivale a} \; \; \;  0 \leq x < \frac{\pi}{2} \vee \frac{3}{2}\pi < x \leq 2\pi$$

### Studio della frazione

Ora che sappiamo quando il numeratore e il denominatore sono positivi, posso mettere tutto insieme nel "castello dei segni" e vedere quando la frazione è positiva e negativa. 

Metto in una riga il segno del numeratore: con $$+$$ indico dove il numeratore è positivo. Stessa cosa per il denominatore in una riga successiva. Indico con i pallini pieni gli estremi che sono inclusi, con i pallini vuoti quelli esclusi. 

$$
\begin{tikzpicture}
\draw (0,0) -- (3.5,0);
\draw (0,2.7) -- (0,-0.2);
\draw (0.5,2.7) -- (0.5,-0.2);
\draw (1,2.7) -- (1,-0.2);
\draw (1.5,2.7) -- (1.5,-0.2);
\draw (2,2.7) -- (2,-0.2);
\draw (2.5,2.7) -- (2.5,-0.2);
\draw (3,2.7) -- (3,-0.2);
\draw (3.5,2.7) -- (3.5,-0.2);
\node at (0,-0.5) {\small $0$};
\node at (0.5,-0.5) {\small $\frac{\pi}{4}$};
\node at (1,-0.5) {\small $\frac{\pi}{2}$};
\node at (1.5,-0.5) {\small $\frac{3\pi}{4}$};
\node at (2,-0.5) {\small $\frac{5\pi}{4}$};
\node at (2.5,-0.5) {\small $\frac{3\pi}{2}$};
\node at (3,-0.5) {\small $\frac{7\pi}{4}$};
\node at (3.5,-0.5) {\small $2\pi$};
\node at (-2,0.5) {\small Frazione:};
\node at (-3,1.5) {\small Den: $0 \leq x < \frac{\pi}{2} \vee \frac{3}{2}\pi < x \leq 2\pi$};
\node at (-3,2.5) {\small Num: $\frac{\pi}{4} \leq x \leq \frac{3}{4}\pi  \vee \frac{5}{4}\pi \leq x \leq \frac{7}{4}\pi$};
\draw (0,1) -- (4,1);
\draw (0,2) -- (4,2);
\node at (0.25,2.5) {\small $-$};
\node at (0.75,2.5) {\small $+$};
\node at (1.25,2.5) {\small $+$};
\node at (1.75,2.5) {\small $-$};
\node at (2.25,2.5) {\small $+$};
\node at (2.75,2.5) {\small $+$};
\node at (3.25,2.5) {\small $-$};
\node at (0.25,1.5) {\small $+$};
\node at (0.75,1.5) {\small $+$};
\node at (1.25,1.5) {\small $-$};
\node at (1.75,1.5) {\small $-$};
\node at (2.25,1.5) {\small $-$};
\node at (2.75,1.5) {\small $+$};
\node at (3.25,1.5) {\small $+$};
\node at (0.25,0.5) {\small $-$};
\node at (0.75,0.5) {\small $+$};
\node at (1.25,0.5) {\small $-$};
\node at (1.75,0.5) {\small $+$};
\node at (2.25,0.5) {\small $-$};
\node at (2.75,0.5) {\small $+$};
\node at (3.25,0.5) {\small $-$};
\draw[fill=black] (0.5,2.5) circle (0.06cm);
\draw[fill=black] (1.5,2.5) circle (0.06cm);
\draw[fill=black] (2,2.5) circle (0.06cm);
\draw[fill=black] (3,2.5) circle (0.06cm);
\draw[fill=black] (0,1.5) circle (0.06cm);
\draw (1,1.5) circle (0.06cm);
\draw (2.5,1.5) circle (0.06cm);
\draw[fill=black] (3.5,1.5) circle (0.06cm);
\draw[fill=black] (0.5,0.5) circle (0.06cm);
\draw[fill=black] (1.5,0.5) circle (0.06cm);
\draw[fill=black] (2,0.5) circle (0.06cm);
\draw[fill=black] (3,0.5) circle (0.06cm);
\draw[fill=black] (0,0.5) circle (0.06cm);
\draw (1,0.5) circle (0.06cm);
\draw (2.5,0.5) circle (0.06cm);
\draw[fill=black] (3.5,0.5) circle (0.06cm);
\end{tikzpicture}
$$

Nella riga frazione, prendo gli intervalli con $$+$$ o con $$-$$? Dipende da cosa sto risolvendo. Nel nostro caso volevamo trovare quando la frazione è negativa ($$\leq 0$$) quindi prendo gli intervalli con il segno $$-$$. 

La soluzione è quindi 

$$0 \leq x \leq \frac{\pi}{4} \; \vee \; \frac{\pi}{2} < x \leq \frac{3}{4}\pi \; \vee \; \frac{5}{4}\pi \leq x < \frac{3}{2}\pi \; \vee \; \frac{7}{4}\pi \leq x \leq 2\pi$$



