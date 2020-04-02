# EQUAZIONI DIFFERENZIALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Determina la soluzione particolare della seguente equazione differenziale, verificante la condizione
posta a fianco.

$$y^{'}+2xy = \frac{x}{y} \qquad y(0) = 1$$

## Soluzione:

Come prima cosa notiamo che l'equazione non è lineare in quanto c'è un termine $$y$$ a denominatore. Isoliamo la derivata:

$$y^{'} = \frac{x}{y} - 2xy$$

L'equazione non è neanche del tipo $$y^{'} = f(x)$$ in quanto a destra dell'uguale compaiono anche termini in $$y$$. 

Questa è un'equazione a variabili separabili: infatti,

$$\begin{align*}
y^{'} & = \frac{x}{y} - 2xy \\
& = -x\left(-\frac{1}{y}+2y\right) \\
& = -x \left(\frac{-1+2y^2}{y}\right) \\
& = \underbrace{-x }_{\text{funzione in x}}\cdot \underbrace{\left(\frac{2y^2-1}{y}\right)}_{\text{funzione in y}}
\end{align*}$$

Siamo quindi di fronte a un'equazione differenziale del tipo 

$$y^{'} = g(x)\cdot h(y)$$

dove, nel nostro caso, $$g(x) = -x$$ e $$h(y) = \frac{2y^2-1}{y}$$.

Per risolverla si applica il metodo della separazione delle variabili.

Piccola parentesi per capire come funziona questo metodo:

Sappiamo che scrivere $$y$$ o scrivere $$f(x)$$ è lo stesso: modi diversi per scrivere la stessa identica cosa. Analogamente, ci sono vari modi per indicare la derivata: i più comuni sono $$'$$ oppure $$D$$. Un terzo modo è 

$$\frac{d(\text{cosa voglio derivare})}{d(\text{variabile rispetto a cui voglio fare la derivata})}$$

Per esempio, se voglio derivare la nostra funzione $$f(x)$$ rispetto alla variabile $$x$$ (tradotto: la derivata che facciamo sempre) posso scrivere equivalentemente

$$\frac{d f(x)}{dx}, D(f(x)), f^{'}(x)$$

E visto che scrivere $$f(x)$$ è come scrivere $$y$$ ho 

$$\frac{dy}{dx}, D(y), y^{'}$$

Ora, se invece di $$y^{'}$$ scrivo $$\frac{dy}{dx}$$ e lo tratto come se fosse una frazione, ottengo

$$\begin{align*}
y^{'} & = g(x)h(y) \\
\frac{dy}{dx} & = g(x)h(y)
\end{align*}$$

Moltiplico destra e sinistra per $$\frac{dx}{h(y)}$$:

$$\begin{align*}
\frac{dy}{dx} \cdot \frac{dx}{h(y)} & = g(x)h(y) \cdot \frac{dx}{h(y)} \\
\frac{dy}{h(y)} & = g(x)dx
\end{align*}$$

Integro destra e sinistra: 

$$\begin{align*}
\int \frac{dy}{h(y)} & = \int g(x)dx
\end{align*}$$

e calcolo infine e due integrali separatamente. 

Applichiamo questo metodo al nostro caso. 

$$\begin{align*}
\frac{dy}{dx} & = -x\left(\frac{2y^2-1}{y}\right) \\
\frac{dy}{dx} \cdot \frac{dx}{\frac{2y^2-1}{y}}& = -x\left(\frac{2y^2-1}{y}\right) \cdot \frac{dx}{\frac{2y^2-1}{y}} \\
\frac{dy}{\frac{2y^2-1}{y}} & = -xdx \\
\frac{y}{2y^2-1}dy & = -xdx \\
\int \frac{y}{2y^2-1}dy & = \int -xdx
\end{align*}$$

Risolviamo ora i due integrali separatamente. Quello di destra è immediato e si ottiene

$$\int -xdx = -\int xdx = -\frac{x^2}{2} +c$$

Per quello di sinistra invece notiamo che a numeratore della frazione abbiamo quasi esattamente la derivata del denominatore: la derivata del denominatore sarebbe $$4y$$ e invece noi abbiamo $$y$$. Posso però moltiplicare e dividere per $$4$$ al fine di ottenere quello che voglio:

$$\begin{align*}
\int \frac{y}{2y^2-1} dy & = \int \frac{1}{4} \cdot 4 \cdot \frac{y}{2y^2-1}dy \\
& = \frac{1}{4} \int \frac{4y}{2y^2-1}dy \\
& = \frac{1}{4} \int \frac{D(2y^2-1)}{2y^2-1}dy \\
& = \frac{1}{4} \ln\left(|2y^2-1|\right)
\end{align*}$$

***
Memo: 

$$\int \frac{f^{'}(x)}{f(x)}dx = \ln(|f(x)|)+c$$

Nel nostro caso la variabile è $$y$$ invece che $$x$$, $$f(y) = 2y^2-1 \Rightarrow f^{'}(y) = 4y$$.
***

Ora che abbiamo calcolato i due integrali, abbiamo 

$$\begin{align*}
\int \frac{y}{2y^2-1}dy & = \int -xdx \\
\frac{1}{4} \ln\left(|2y^2-1|\right) & = -\frac{x^2}{2}+c \\
4 \cdot \frac{1}{4} \ln\left(|2y^2-1|\right) & = 4 \cdot \left(-\frac{x^2}{2}+c\right) \\
\ln\left(|2y^2-1|\right) & = -2x^2+4c \\
e^{\ln\left(|2y^2-1|\right)} & = e^{-2x^2+4c} \\
|2y^2-1| & = e^{-2x^2+4c}
\end{align*}$$

Notiamo che, per definizione di valore assoluto,

$$|2y^2-1| = \begin{cases}
2y^2-1 & \text{se} \; 2y^2-1 \geq 0 \\
-2y^2+1 & \text{se} \; 2y^2-1 < 0
\end{cases}$$

Risolvendo $$2y^2-1 \geq 0$$ si ottiene 

$$\begin{align*}
2y^2-1 & \geq 0 \\
2y^2 & \geq 1 \\
y^2 & \geq \frac{1}{2} \\
& \downarrow \\
\text{equazione} & \; \text{associata} \\
y^2 & = \frac{1}{2} \\
y & = \pm \frac{1}{\sqrt{2}} \\
& \downarrow \\
\text{avevo} \geq & \Rightarrow \text{intervalli esterni} \\
y \leq - \frac{1}{\sqrt{2}} \; \; & \cup \; \; y \geq \frac{1}{\sqrt{2}}
\end{align*}$$

e quindi 

$$|2y^2-1| = \begin{cases}
2y^2-1 & \text{se} \; y \leq - \frac{1}{\sqrt{2}} \; \cup \; y \geq \frac{1}{\sqrt{2}} \\
-2y^2+1 & \text{se} \; -\frac{1}{\sqrt{2}} < y < \frac{1}{\sqrt{2}}
\end{cases}$$

Dal momento che $$y(0) = 1$$ (ossia $$y=1$$ in $$x=0$$), devo utilizzare il primo caso del valore assoluto: esso vale infatti quando $$y \leq - \frac{1}{\sqrt{2}} \;\cup \; y \geq \frac{1}{\sqrt{2}}$$. Avendo io $$y=1 > \frac{1}{\sqrt{2}}$$, ricado in questo caso. 

Quindi

$$\begin{align*}
|2y^2-1| & = e^{-2x^2+4c} \\
2y^2-1 & = e^{-2x^2+4c} \\
2y^2 & = e^{-2x^2+4c}+1 \\
y^2 & = \frac{e^{-2x^2+4c}+1}{2} \\
y & = \pm \sqrt{\frac{e^{-2x^2+4c}+1}{2}}
\end{align*}$$

Anche qui faccio un ragionamento analogo a prima: poichè ho $$y(0) = 1 > 0$$, ciò significa che $$y$$ deve essere positiva. Devo quindi considerare

$$y = + \sqrt{\frac{e^{-2x^2+4c}+1}{2}}$$

Vado ora ad imporre la condizione $$y(0) = 1$$ al fine di trovare $$c$$. Calcolo quindi la funzione in $$x=0$$:

$$\begin{align*}
y(0) & =  \sqrt{\frac{e^{-2(0)^2+4c}+1}{2}} \\
& = \sqrt{\frac{e^{4c}+1}{2}}
\end{align*}$$

La condizione mi dice che questo deve essere uguale a 1:

$$\begin{align*}
\sqrt{\frac{e^{4c}+1}{2}} & = 1 \\
\left(\sqrt{\frac{e^{4c}+1}{2}}\right)^2 & = (1)^2 \\
\frac{e^{4c}+1}{2} & = 1 \\
2 \cdot \frac{e^{4c}+1}{2} & = 2 \cdot 1 \\
e^{4c}+1 & = 2 \\
e^{4c} & = 2-1 \\
e^{4c} & = 1 \\
\ln\left(e^{4c}\right) & = \ln(1) \\
4c & = 0 \\
\frac{4c}{4} & = \frac{0}{4} \\
c & = 0
\end{align*}$$

La soluzione particolare è quindi data da

$$y = \sqrt{\frac{e^{-2x^2}+1}{2}}$$



