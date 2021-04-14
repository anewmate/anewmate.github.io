# DISEQUAZIONE FRATTE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Risolvi la seguente disequazione fratta

$$\frac{2x}{2x+2} + \frac{3x-2}{x^2+2x+1} + \frac{2-x}{(x+1)^2} + \frac{1}{x+1} \geq 0$$

## Soluzione: 

Come prima cosa, avendo delle frazioni con l'incognita a denominatore, poniamo le condizioni di esistenza (C.E.): in questo caso dobbiamo imporre che tutte le frazioni esistano, quindi che ogni denominatore sia diverso da zero.

$$\begin{align*}
\text{C.E.:} \; \begin{cases}
2x+2 \neq 0 \\
x^2+2x+1 \neq 0 \\
(x+1)^2 \neq 0 \\
x+1 \neq 0 
\end{cases}
\end{align*}$$

Risoluzione di ogni singola condizione:

$$\begin{align*}
\text{1.} \qquad 2x+2 & = 0 \\
2x & = -2 \\
\frac{2x}{2} & = \frac{-2}{2} \\
x & = -1 \\
\text{2.} \qquad x^2+2x+1 & = 0 \\
(x+1)^2 & = 0 \\
x + 1 & = 0 \\
x & = -1 \\
\text{3.} \qquad (x+1)^2 & = 0 \\
x+1 & = 0 \\
x & = -1 \\
\text{4.} \qquad x+1 & = 0 \\
x & = -1 
\end{align*}$$

Abbiamo quindi trovato un solo valore che annulla i denominatori: $$x = -1$$. Le condizioni di esistenza sono quindi 

$$\begin{align*}
\text{C.E.:} \; x \neq -1 
\end{align*}$$

Per poter poi risolvere la disequazione fratta, dobbiamo arrivare ad avere una forma del tipo 

$$\frac{A(x)}{B(x)} \gtrless 0$$

ossia un'unica frazione a sinistra e zero a destra. Andiamo quindi a sommare i termini a sinistra 

$$\begin{align*}
\frac{2x}{2x+2} + \frac{3x-2}{x^2+2x+1} + \frac{2-x}{(x+1)^2} + \frac{1}{x+1} & \geq 0 \\
\frac{2x}{2(x+1)} + \frac{3x-2}{(x+1)^2} + \frac{2-x}{(x+1)^2} + \frac{1}{x+1} & \geq 0 \\
\frac{2x\cdot (x+1) + (3x-2)\cdot (2) + (2-x) \cdot (2) + (1) \cdot (2(x+1))}{2(x+1)^2} & \geq 0 \\
\frac{2x^2+2x+6x-4+4-2x+2x+2}{2(x+1)^2} & \geq 0 \\
\frac{2x^2+8x+2}{2(x+1)^2} & \geq 0 
\end{align*}$$

Ci stiamo quindi chiedendo quando quella frazione è positiva: per poter rispondere a questa domanda, dobbiamo andare a studiare il segno del numeratore e del denominatore separatamente e poi, alla fine, moltiplicare i segni. Indipendentemente dal verso della disuguaglianza, vado quindi a vedere quando numeratore e denominatore sono positivi. 

<h3>Studio del numeratore</h3>

Inizio chiedendomi quando il numeratore è positivo: siccome mi sto chiedendo quando la frazione è $$\geq$$ di zero (c'è anche l'uguale), mantengo l'uguale anche nello studio del numeratore. 

$$ 2x^2+8x+2 \geq 0 $$

Visto che tutti i coefficienti sono multipli di due, raccolgo un 2 e divido tutto per 2:

$$\begin{align*}
2x^2+8x+2 & \geq 0 \\
2(x^2+4x+1) & \geq 0 \\
\frac{2(x^2+4x+1)}{2} & \geq \frac{0}{2} \\
x^2+4x+1 & \geq 0 
\end{align*}$$

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
x^2+4x+1 & \; \textcolor{red}{\geq} \; 0 \\
& \downarrow \\
\text{equazione} & \; \text{associata:} \\
x^2+4x+1 & = 0 \\
x_{1/2} & = \frac{-b\pm \sqrt{b^2-4ac}}{2a} \\
& = \frac{-4 \pm \sqrt{16-4(1)(1)}}{2(1)} \\
& = \frac{-4 \pm \sqrt{12}}{2} \\
& = \frac{-4 \pm \sqrt{4 \cdot 3}}{2} \\
& = \frac{-4 \pm 2\sqrt{3}}{2} \\
& = \frac{2(-2 \pm \sqrt{3})}{2} \\
& = -2 \pm \sqrt{3} \\
\text{poichè avevo} \; \textcolor{red}{\geq} & \rightarrow \text{intervalli esterni:} \\
x \leq -2-\sqrt{3} & \; \; \vee \; \; x \geq -2+\sqrt{3}
\end{align*}$$

Abbiamo quindi trovato che il numeratore è positivo quando $$x \leq -2-\sqrt{3}$$ e quando $$x \geq -2+\sqrt{3}$$. 

<h3>Studio del denominatore</h3>

Mi chiedo ora quando il denominatore è positivo: sebbene ci stessimo chiedendo quando la frazione è $$\geq$$ di zero (c'è anche l'uguale), nel denominatore l'uguaglianza non si mantiene mai dal momento che i denominatori non possono essere uguali a zero. 

$$\begin{align*}
2(x+1)^2 & > 0 
\end{align*}$$

Anche qui divido tutto per due:

$$\begin{align*}
2(x+1)^2 & > 0 \\
\frac{2(x+1)^2}{2} & > \frac{0}{2} \\
(x+1)^2 & > 0 
\end{align*}$$

Ricordando che i quadrati sono sempre maggiori o uguali a zero, la disuguaglianza è sempre verificata tranne quando si annulla l'argomento del quadrato. Ossia 

$$(x+1)^2 > 0 \rightarrow x + 1 \neq 0$$

La soluzione di $$(x+1)^2 > 0$$ è quindi $$x \neq -1$$. Abbiamo trovato che il denominatore è sempre positivo tranne per $$x=-1$$ (dove la frazione non esiste). 

<hr>

MEMO: Siccome so che di solito queste disequazioni sono sempre un casino, ricordo qui le soluzioni in generale: 

1. $$(*(x))^2 \geq 0 \rightarrow \forall \; x \in \mathbb{R}$$
1. $$(*(x))^2 > 0 \rightarrow  *(x) \neq 0 $$
1. $$(*(x))^2 \leq 0 \rightarrow *(x) = 0 $$ 
1. $$(*(x))^2 < 0 \rightarrow \nexists \; x \in \mathbb{R}$$ 

dove $$*(x)$$ è qualsiasi cosa scritta in funzione di $$x$$. Esempi:

$$(x-7)^2 \leq 0$$ appartiene al caso 3. e ha soluzione $$x-7 = 0$$;

$$(3x+1)^2 > 0$$ appartiene al caso 2. e ha soluzione $$3x+1 \neq 0$$. 

<hr>

<h3>Studio della frazione</h3>

Ora che abbiamo studiato numeratore e denominatore, possiamo mettere tutto insieme e studiare il segno della frazione. Andiamo a costruire il "castello dei segni": 

$$
\begin{tikzpicture}
\draw (0,0) -- (5,0);
\draw (1,-0.2) -- (1,3);
\draw (2.5,-0.2) -- (2.5,3);
\draw (4,-0.2) -- (4,3);
\node at (1,-0.5) {\small $-2-\sqrt{3}$};
\node at (2.5,-0.5) {\small $-1$};
\node at (4,-0.5) {\small $-2+\sqrt{3}$};
\node at (-2,0.5) {\small Frazione:};
\node at (-2,1.5) {\small Denominatore:};
\node at (-2,2.5) {\small Numeratore:};
\draw (0,1) -- (5,1);
\draw (0,2) -- (5,2);
\node at (0.5,2.5) {$+$};
\node at (1.75,2.5) {$-$};
\node at (3.25,2.5) {$-$};
\node at (4.5,2.5) {$+$};
\draw[fill = black] (1,2.5) circle (0.07);
\draw[fill = black] (4,2.5) circle (0.07);
\node at (0.5,1.5) {$+$};
\node at (1.75,1.5) {$+$};
\node at (3.25,1.5) {$+$};
\node at (4.5,1.5) {$+$};
\draw (2.5,1.5) circle (0.07);
\node at (0.5,0.5) {$+$};
\node at (1.75,0.5) {$-$};
\node at (3.25,0.5) {$-$};
\node at (4.5,0.5) {$+$};
\draw[fill = black] (1,0.5) circle (0.07);
\draw[fill = black] (4,0.5) circle (0.07);
\draw (2.5,0.5) circle (0.07);
\end{tikzpicture}
$$

Inerisco in ogni riga i risultati ottenuti in precedenza: metto una $$+$$ negli intervalli dove il numeratore è positivo e una $$-$$ nel resto. Stessa cosa per il denominatore: in generale, con i pallini pieni indico il fatto che gli estremi sono inclusi. Nell'ultima riga, quella chiamata Frazione, si moltiplicano fra loro i segni delle due righe precedenti; è inoltre in questa riga che leggo il risultato finale. 

Il mio obiettivo era quello di scoprire quando la frazione è positiva: la soluzione sarà quindi data da tutti gli intervalli in cui ho un segno $$+$$ nella riga Frazione: nel nostro caso $$x \leq -2-\sqrt{3} \; \vee \; x \geq -2+\sqrt{3}$$. 

ATTENZIONE: l'esercizio non è finito qui. L'ultimo step consiste nel confrontare la soluzione trovata con le C.E.: se nelle condizioni di esistenza ho dei valori che sono inclusi nella soluzione che ho trovato, devo andare ad escluderli dalla soluzione. 

Non è però il nostro caso: le C.E. ci dicevano $$x \neq -1$$, ma $$-1$$ non è incluso nella soluzione che abbiamo trovato, che è quindi la soluzione finale: 

$$x \leq -2-\sqrt{3} \; \vee \; x \geq -2+\sqrt{3}$$

<hr> 

Esempio di cosa intendo con confrontare la soluzione finale con le C.E..

Supponiamo che le C.E. siano $$x \neq \pm 1$$. 

Faccio tutto lo studio della frazione e nella riga Frazione leggo che il mio risultato è $$x \leq -2 \vee x \geq 0$$. In questo caso questa *non* è la mia soluzione finale: infatti c'è $$x = 1$$ che devo escludere per C.E.. 

Graficamente: 

$$
\begin{tikzpicture}
\draw (-3,0) -- (2,0);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (0,-0.2) -- (0,0.2);
\draw (1,-0.2) -- (1,0.2);
\node at (-2,-0.5) {-2};
\node at (-1,-0.5) {-1};
\node at (0,-0.5) {0};
\node at (1,-0.5) {1};
\draw[red] (-2,0.5) -- (-3,0.5);
\draw[red] (0,0.5) -- (2,0.5);
\draw[fill = red] (-2,0.5) circle (0.05);
\draw[fill = red] (0,0.5) circle (0.05);
\draw[fill = white] (-1,0.5) circle (0.05);
\draw[fill = white] (1,0.5) circle (0.05);
\draw[->] (-1,1) -- (-1,0.7);
\node at  (-1,1.2) {\small C.E.};
\draw[->] (1,1) -- (1,0.7);
\node at  (1,1.2) {\small C.E.};
\node[red] at (3,0.5) {soluzione};
\end{tikzpicture}
$$

La mia soluzione finale è quindi 

$$x \leq -2 \; \vee \; 0 \leq x < 1 \; \vee \; x > 1$$

o, equivalentemente,

$$x \leq -2 \; \vee \; x \geq 0,\;  x \neq 1$$




