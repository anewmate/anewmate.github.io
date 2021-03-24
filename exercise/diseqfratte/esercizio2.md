# DISEQUAZIONE FRATTE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Risolvi la seguente disequazione fratta

$$-\frac{2}{x-3}-x < 0$$

## Soluzione: 

Come prima cosa, avendo delle frazioni con l'incognita a denominatore, poniamo le condizioni di esistenza (C.E.): in questo caso dobbiamo imporre che la frazione esista, quindi che il suo denominatore sia diverso da zero.

$$\begin{align*}
\text{C.E.:} \; x-3 \neq 0 \rightarrow x \neq 3
\end{align*}$$

Per poter poi risolvere la disequazione fratta, dobbiamo arrivare ad avere una forma del tipo 

$$\frac{A(x)}{B(x)} \gtrless 0$$

ossia un'unica frazione a sinistra e zero a destra. Andiamo quindi a sommare i termini a sinistra 

$$\begin{align*}
-\frac{2}{x-3}-x & < 0 \\
\frac{-2-x(x-3)}{x-3} & < 0 \\
\frac{-2-x^2+3x}{x-3} & < 0 \\
\frac{-x^2+3x-2}{x-3} & < 0
\end{align*}$$

Ci stiamo quindi chiedendo quando quella frazione è negativa: per poter rispondere a questa domanda, dobbiamo andare a studiare il segno del numeratore e del denominatore separatamente e poi, alla fine, moltiplicare i segni. Indipendentemente dal verso della disuguaglianza, vado quindi a vedere quando numeratore e denominatore sono positivi. 

<h3>Studio del numeratore</h3>

Inizio chiedendomi quando il numeratore è positivo:

$$ -x^2+3x-2 > 0 $$

Abbiamo ottenuto quindi una disequazione di secondo grado.

<hr>

**Memo**: Ricordiamo la regola in generale che ci dice. Se ho

1. espressione del tipo $$ax^2+bx+c \gtrless 0$$
1. $$\textbf{a}>0$$
1. delta positivo: $$\Delta > 0$$
1. $$x_1,x_2$$ soluzioni dell'equazione associata con $$x_2 < x_1$$

Allora $$ax^2+bx+c > 0$$ ha soluzione $$x < x_2 \cup x > x_1$$, mentre $$ax^2+bx+c < 0$$ ha soluzione $$x_2 < x < x_1$$. A parole, se voglio l'espressione positiva devo prendere l'unione degli intervalli esterni ai due valori che ottengo nell'equazione associata. Se invece voglio l'espressione negativa, devo prendere l'intervallo interno. In entrambi i casi, escludo o includo i punti estremi se la disuguaglianza è stretta oppure no.  

<hr>

Quindi 

$$\begin{align*}
-x^2+3x-2 & > 0 \\
(-1) \cdot (-x^2+3x-2) & > 0 \cdot (-1) \\
x^2-3x+2 \; & \textcolor{red}{<} \; 0 \\
& \downarrow \\
\text{equazione} & \; \text{associata:} \\
x^2-3x+2 & = 0 \\
x_{1/2} & = \frac{-b\pm \sqrt{b^2-4ac}}{2a} \\
& = \frac{-(-3) \pm \sqrt{9-4(1)(2)}}{2(1)} \\
& = \frac{3 \pm 1}{2} \\
& = \begin{cases}
2 \\
1
\end{cases}
& \downarrow \\
\text{poichè avevo} \; \textcolor{red}{<} & \rightarrow \text{intervallo interno:} \\
1 < \; &  \; x  \; < 2
\end{align*}$$

Abbiamo quindi trovato che il numeratore è positivo quando $$1 < x < 2$$. 

<h3>Studio del denominatore</h3>

Mi chiedo ora quando il denominatore è positivo:

$$\begin{align*}
x-3 & > 0 \\
x & > 3
\end{align*}$$

<h3>Studio della frazione</h3>

Ora che abbiamo studiato numeratore e denominatore, possiamo mettere tutto insieme e studiare il segno della frazione. Andiamo a costruire il "castello dei segni": 

$$
\begin{tikzpicture}
\draw (0,0) -- (4,0);
\draw (1,2.7) -- (1,-0.2);
\draw (2,2.7) -- (2,-0.2);
\draw (3,2.7) -- (3,-0.2);
\node at (1,-0.5) {$1$};
\node at (2,-0.5) {$2$};
\node at (3,-0.5) {$3$};
\node at (-2,0.5) {\small Frazione:};
\node at (-3,1.5) {\small Denominatore: $x > 3$};
\node at (-3,2.5) {\small Numeratore: $1<x<2$};
\draw (0,1) -- (4,1);
\draw (0,2) -- (4,2);
\node at (1.5,2.5) {$+$};
\node at (0.5,2.5) {$-$};
\node at (2.5,2.5) {$-$};
\node at (3.5,2.5) {$-$};
\node at (1.5,1.5) {$-$};
\node at (0.5,1.5) {$-$};
\node at (2.5,1.5) {$-$};
\node at (3.5,1.5) {$+$};
\node at (1.5,0.5) {$-$};
\node at (0.5,0.5) {$+$};
\node at (2.5,0.5) {$+$};
\node at (3.5,0.5) {$-$};
\node at (1,2.5) {o};
\node at (2,2.5) {o};
\node at (3,1.5) {o};
\node at (1,0.5) {o};
\node at (2,0.5) {o};
\node at (3,0.5) {o};
\end{tikzpicture}
$$

Inerisco in ogni riga i risultati ottenuti in precedenza: metto una $$+$$ negli intervalli dove il numeratore è positivo e una $$-$$ nel resto. Stessa cosa per il denominatore: in generale, con i pallini vuoti indico il fatto che gli estremi sono esclusi. Nell'ultima riga, quella chiamata Frazione, si moltiplicano fra loro i segni delle due righe precedenti; è inoltre in questa riga che leggo il risultato finale. 

Il mio obiettivo era quello di scoprire quando la frazione è negativa: la soluzione sarà quindi data da tutti gli intervalli in cui ho un segno $$-$$ nella riga Frazione:

$$1 < x < 2 \; \vee \; x > 3$$

L'ultimo step consiste nel confrontare la soluzione trovata con le C.E.:

$$\begin{align*}
\begin{cases}
x \neq 3 \\
1 < x < 2 \vee x > 3
\end{cases}
\end{align*}$$

La soluzione finale è quindi 

$$1 < x < 2 \; \vee \; x > 3$$

