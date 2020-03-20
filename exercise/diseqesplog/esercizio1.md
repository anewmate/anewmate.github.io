# DISEQUAZIONI ESPONENZIALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Risolvi la seguente disequazione

$$\left( \frac{4}{5} \right)^2 \left(\frac{5}{4} \right)^x \leq \sqrt[x+2]{\frac{5}{4}}$$

## Soluzione: 

Come prima cosa ricordiamo le proprietà delle potenze:

$$\begin{align*}
A^n \cdot A^m & = A^{n+m} \\
A^n : A^m = \frac{A^n}{A^m} & = A^{n-m} \\
A^n \cdot B^n & = (A \cdot B)^n \\
A^n : B^n = \frac{A^n}{B^n} & = \left( \frac{A}{B}\right)^n \\
(A^n)^m & = A^{n \cdot m}
\end{align*}$$

Come seconda cosa notiamo subito che abbiamo un radicale, ossia un termine con radice. Dobbiamo quindi mettere le condizioni di esistenza su quel termine. Visto che l'incognita sta a indice della radice, dobbiamo imporre che esso sia positivo e naturale. In altre parole, le condizioni di esistenza (C.E.) sono

$$x+2 > 0$$

$$x+2 \in \mathbb{N}$$

La seconda condizione di traduce semplicemente restringendo le $$x$$ all'insieme dei numeri interi $$\mathbb{Z}$$ invece che considerare $$x$$ nell'insieme $$\mathbb{R}$$.

Visto che a destra della disuguaglianza abbiamo come base $$\frac{5}{4}$$, vediamo di trasformare tutto in questa base anche a sinistra. In particolare ci basta riscrivere la potenza con base $$\frac{4}{5}$$ come 

$$\left(\frac{4}{5}\right)^2 = \left(\left(\frac{5}{4}\right)^{-1}\right)^2 = \left(\frac{5}{4}\right)^{-2}$$ 

Inoltre ricordando che

$$\sqrt[n]{x^m} = x^{\frac{m}{n}}$$

si ha 

$$\sqrt[x+2]{\frac{5}{4}} = \left(\frac{5}{4}\right)^{\frac{1}{x+2}}$$

Quindi la disuguaglianza diventa 

$$\left(\frac{5}{4}\right)^{-2} \left(\frac{5}{4} \right)^x \leq \left(\frac{5}{4}\right)^{\frac{1}{x+2}}$$

e per la prima proprietà delle potenze

$$\left(\frac{5}{4} \right)^{x-2} \leq \left(\frac{5}{4}\right)^{\frac{1}{x+2}}$$

Poichè le potenze hanno **base maggiore di 1**, dalla disequazione precedente otteniamo una disequazione equivalente fra gli esponenti **lasciando lo stesso verso**:

$$x-2 \leq \frac{1}{x+2}$$

Siamo quindi passati a una disequazione fratta: portiamo tutto a sinistra e facciamo denominatore comune.

$$\begin{align*}
x-2 & \leq \frac{1}{x+2} \\
x-2 -\frac{1}{x+2} & \leq 0 \\
\frac{x(x+2)-2(x+2)-1}{x+2} & \leq 0 \\
\frac{x^2+2x-2x-4-1}{x+2} & \leq 0 \\
\frac{x^2-5}{x+2} & \leq 0
\end{align*}$$

Passiamo quindi allo studio di numeratore e denominatore singolarmente.

### STUDIO NUMERATORE 
Studio quando 

$$x^2-5 \geq 0$$

Ottengo

$$\begin{align*}
x^2 - 5 & \geq 0 \\
x^2 & \geq 5 \\
& \downarrow \\
\text{equazione} & \; \; \; \text{associata:} \\
x^2 & = 5 \\
x & = \pm \sqrt{5} \\
\text{avevo} \geq & \Rightarrow \text{intervalli esterni} \\
& \downarrow \\
x \leq -\sqrt{5} & \cup x \geq \sqrt{5} 
\end{align*}$$

### STUDIO DENOMINATORE

Studio quando

$$x +2 > 0$$

ossia si ha direttamente 

$$x > -2$$

### STUDIO FRAZIONE

Vado quindi a costruire il castello dei segni: nella prima riga scrivo quando il numeratore è positivo mettendo una + negli intervalli trovati ai passi precedenti. Nella seconda riga faccio la stessa cosa con il denominatore. Infine, nella terza riga moltiplico i segni delle due righe precedenti e vado a selezionare gli intervalli in cui ho il segno - dato che volevo andare a vedere quando la frazione è negativa. 

$$\begin{tikzpicture}
\draw (-3,0) -- (3,0);
\draw (-2,3) -- (-2,-0.2);
\draw (-1,3) -- (-1,-0.2);
\draw (2,3) -- (2,-0.2);
\node at (-2,-0.5) {$-\sqrt{5}$};
\node at (-1,-0.5) {$-2$};
\node at (2,-0.5) {$\sqrt{5}$};
\draw (-3,2) -- (3,2);
\draw (-3,1) -- (3,1);
%Numeratore
\node at (-5,2.5) {Numeratore:};
\node at (-2.5,2.5) {$+$};
\node at (-1.5,2.5) {$-$};
\node at (0.5,2.5) {$-$};
\node at (2.5,2.5) {$+$};
\draw [fill = black](-2,2.5) circle (0.07cm);
\draw [fill = black](2,2.5) circle (0.07cm);
%Denominatore
\node at (-5,1.5) {Denominatore:};
\node at (-2.5,1.5) {$-$};
\node at (-1.5,1.5) {$-$};
\node at (0.5,1.5) {$+$};
\node at (2.5,1.5) {$+$};
\draw(-1,1.5) circle (0.07cm);
%Frazione
\node at (-5,0.5) {Frazione:};
\node at (-2.5,0.5) {$-$};
\node at (-1.5,0.5) {$+$};
\node at (0.5,0.5) {$-$};
\node at (2.5,0.5) {$+$};
\draw [fill = black](-2,0.5) circle (0.07cm);
\draw [fill = black](2,0.5) circle (0.07cm);
\draw(-1,0.5) circle (0.07cm);
\end{tikzpicture}$$

La frazione è negativa quindi negli intervalli 

$$x \leq -\sqrt{5} \vee -2 < x \leq \sqrt{5}$$

Devo però ricordami ora che tutto il problema aveva delle C.E., e in particolare queste consistevano in $$x \in \mathbb{Z}$$ e $$x > -2$$. Tenendo conto di queste restrizioni, devo quindi escludere l'intervallo $$x \leq -\sqrt{5}$$ e la soluzione finale è 

$$-2 < x \leq \sqrt{5}, x \in \mathbb{Z}$$