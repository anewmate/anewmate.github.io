# DISEQUAZIONE FRATTE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Risolvi la seguente disequazione fratta

$$\frac{2x^2+3x+5}{x^2-x+3} < -1$$

## Soluzione: 

Come prima cosa, avendo delle frazioni con l'incognita a denominatore, poniamo le condizioni di esistenza (C.E.): in questo caso dobbiamo imporre che la frazione esista, quindi che il suo denominatore sia diverso da zero.

$$\begin{align*}
\text{C.E.:} \; x^2-x+3 \neq 0 
\end{align*}$$

Risoluzione:

$$\begin{align*}
x^2-x+3 & = 0 \\
x_{1/2} & = \frac{-b\pm\sqrt{b^2-4ac}}{2a} \\
& = \frac{+1\pm \sqrt{1-12}}{2} \\
& = \frac{1 \pm \sqrt{\textcolor{red}{-11}}}{2}
\end{align*}$$

Attenzione: abbiamo ottenuto che il $$\textcolor{red}{\Delta} = - 11$$ è negativo. Ciò significa che l'equazione che volevamo risolvere non ha soluzione, ossia non esistono valori di $$x$$ che annullano il denominatore. In altre parole, qualunque valore di $$x$$ io inserisca in $$x^2-x+3$$ ottengo sempre un numero diverso da zero. Quindi non ho condizioni di esistenza:

$$\begin{align*}
\text{C.E.:} \; x^2-x+3 \neq 0 \rightarrow \forall \; x \in \mathbb{R} 
\end{align*}$$

Per poter poi risolvere la disequazione fratta, dobbiamo arrivare ad avere una forma del tipo 

$$\frac{A(x)}{B(x)} \gtrless 0$$

ossia un'unica frazione a sinistra e zero a destra. Andiamo quindi a sommare i termini a sinistra 

$$\begin{align*}
\frac{2x^2+3x+5}{x^2-x+3}+1 & < 0 \\
\frac{2x^2+3x+5+x^2-x+3}{x^2-x+3} & < 0 \\
\frac{3x^2+2x+8}{x^2-x+3} & < 0 
\end{align*}$$

Ci stiamo quindi chiedendo quando quella frazione è negativa: per poter rispondere a questa domanda, dobbiamo andare a studiare il segno del numeratore e del denominatore separatamente e poi, alla fine, moltiplicare i segni. Indipendentemente dal verso della disuguaglianza, vado quindi a vedere quando numeratore e denominatore sono positivi. 

<h3>Studio del numeratore</h3>

Inizio chiedendomi quando il numeratore è positivo:

$$ 3x^2+2x+8 > 0 $$

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
3x^2+2x+8 & > 0 \\
& \downarrow \\
\text{equazione} & \; \text{associata:} \\
3x^2+2x+8 & = 0 \\
x_{1/2} & = \frac{-b\pm \sqrt{b^2-4ac}}{2a} \\
& = \frac{-2 \pm \sqrt{4-4(3)(8)}}{2(3)} \\
& = \frac{-2 \pm \sqrt{-92}}{2} \\
\end{align*}$$

Abbiamo quindi trovato che il delta è negativo: l'equazione associata non ha mai soluzioni, ma noi volevamo risolvere la disequazione. Cosa possiamo dire su quella? 

<hr>

**Memo**: Ricordiamo la regola in generale che ci dice. Se ho

1. espressione del tipo $$ax^2+bx+c \gtrless 0$$
1. $$\textbf{a}>0$$
1. delta negativo: $$\Delta < 0$$

Allora $$ax^2+bx+c > 0$$ ha soluzione $$\forall \; x \in \mathbb{R}$$, mentre $$ax^2+bx+c < 0$$ ha soluzione $$\nexists \; x \in \mathbb{R}$$. A parole, se $$a > 0$$ e delta è negativo, l'espressione $$ax^2+bx+c$$ è sempre positiva: quindi la disuguaglianza con il maggiore è sempre verificata mentre non lo è mai quella con il minore.   

<hr>

Nel nostro caso $$a = 3$$ e vogliamo $$3x^2+2x+8 > 0$$: la disuguaglianza quindi è sempre verificata (soluzione: $$\forall \; x \in \mathbb{R}$$). Ciò significa quindi che il nostro numeratore è sempre positivo. 


<h3>Studio del denominatore</h3>

Mi chiedo ora quando il denominatore è positivo:

$$\begin{align*}
x^2-x+3 & > 0 
\end{align*}$$

Andando a studiare l'equazione associata (che avevamo fatto prima per determinare le C.E.), anche qui troviamo un delta negativo: $$a = 1$$ e vogliamo $$x^2-x+3 > 0$$, disequazione sempre verificata con lo stesso ragionamento fatto per il numeratore. Abbiamo quindi trovato che anche il denominatore è sempre positivo. 

<h3>Studio della frazione</h3>

Ora che abbiamo studiato numeratore e denominatore, possiamo mettere tutto insieme e studiare il segno della frazione. Andiamo a costruire il "castello dei segni": 

$$
\begin{tikzpicture}
\draw (0,0) -- (2,0);
\node at (-2,0.5) {\small Frazione:};
\node at (-2,1.5) {\small Denominatore:};
\node at (-2,2.5) {\small Numeratore:};
\draw (0,1) -- (2,1);
\draw (0,2) -- (2,2);
\node at (1,2.5) {$+$};
\node at (1,1.5) {$+$};
\node at (1,0.5) {$+$};
\end{tikzpicture}
$$

Inerisco in ogni riga i risultati ottenuti in precedenza: metto una $$+$$ negli intervalli dove il numeratore è positivo e una $$-$$ nel resto. Stessa cosa per il denominatore: in generale, con i pallini vuoti indico il fatto che gli estremi sono esclusi. Nell'ultima riga, quella chiamata Frazione, si moltiplicano fra loro i segni delle due righe precedenti; è inoltre in questa riga che leggo il risultato finale. 

Dal momento che sia numeratore che denominatore sono sempre positivi, avrò un segno $$+$$ su tutta la riga del numeratore e su tutta la riga del denominatore.

Il mio obiettivo era quello di scoprire quando la frazione è negativa: la soluzione sarà quindi data da tutti gli intervalli in cui ho un segno $$-$$ nella riga Frazione: nel nostro caso non abbiamo segni $$-$$ nella riga frazione, quindi possiamo concludere che la frazione non è mai negativa. La disequazione quindi non ha soluzione

$$\nexists \; x \in \mathbb{R}$$

In generale, l'ultimo step consisterebbe nel confrontare la soluzione trovata con le C.E., che però in questo caso non abbiamo. 




