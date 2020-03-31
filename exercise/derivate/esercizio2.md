# DERIVATE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Calcola la derivata della seguente funzione nel punto $$c$$ indicato a fianco, applicando la definizione di derivata

$$f(x) = \frac{x^2-1}{2-x} \qquad c = 1$$

## Soluzione:

Come prima cosa ricordiamo la definizione di derivata. Data una funzione $$y = f(x)$$ si chiama derivata della funzione $$f$$ nel punto $$c$$ il limite, se esiste ed è finito, per $$h$$ che tende a zero, del rapporto incrementale relativo a $$c$$: si indica con $$f^{'}(c)$$ e vale 

$$f^{'}(c) = \lim_{h \rightarrow 0} \underbrace{\frac{f(c+h)-f(c)}{h}}_{\text{rapporto incrementale}}$$

Applicando questa definizione al nostro caso, otteniamo che la derivata di $$f$$ in $$c=1$$ è 

$$\begin{align*}
f^{'}(1) & = \lim_{h\rightarrow 0} \frac{f(1+h)-f(1)}{h}
\end{align*}$$

Calcoliamo separatamente $$f(1+h)$$ e $$f(1)$$.

$$\begin{align*}
f(1) & = \frac{(1)^2-1}{2-(1)} \\
& = \frac{1-1}{1} = 0 \\
f(1+h) & = \frac{(1+h)^2-1}{2-(1+h)} \\
& = \frac{1+h^2+2h-1}{2-1-h} \\
& = \frac{h^2+2h}{1-h}
\end{align*}$$

Quindi

$$\begin{align*}
f^{'}(1) & = \lim_{h\rightarrow 0} \frac{f(1+h)-f(1)}{h} \\
& = \lim_{h\rightarrow 0} \frac{\frac{h^2+2h}{1-h}-0}{h} \\
& = \lim_{h\rightarrow 0} \frac{\frac{h^2+2h}{1-h}}{h} \\ 
& = \lim_{h\rightarrow 0} \frac{h^2+2h}{1-h} \cdot \frac{1}{h} \\
& = \lim_{h\rightarrow 0} \frac{h^2+2h}{h(1-h)} \\
& = \lim_{h\rightarrow 0} \frac{h(h+2)}{h(1-h)} \\
& = \lim_{h\rightarrow 0} \frac{h+2}{1-h} \\
& = 2
\end{align*}$$





