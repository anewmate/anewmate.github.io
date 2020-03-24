# LIMITI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Data la seguente funzione, individua i suoi punti di discontinuità e la relativa specie.

$$y = \frac{|x|}{x}\cdot 2^{\frac{1}{x-1}}$$

## Soluzione:

Come prima cosa stabiliamo le condizioni di esistenza (C.E.) di questa funzione. Poichè abbiamo due frazioni, $$\frac{|x|}{x}$$ e $$\frac{1}{x-1}$$, dobbiamo imporre che esse esistano: dobbiamo cioè escludere che il denominatore si annulli. Quindi 

$$\begin{align*}
\text{C.E.:} & \;  \begin{cases}
x \neq 0 \\
x-1 \neq 0
\end{cases} \\
\text{C.E.:} & \;  \begin{cases} 
x \neq 0 \\
x \neq 1
\end{cases}
\end{align*}$$

Abbiamo quindi due punti di discontinuità: $$x=0$$ e $$x=1$$. 

Per poterli classificare dobbiamo andare a calcolare limite destro e sinistro della funzione in quei punti. Prima di procedere, ricordiamo un attimo la definizione di valore assoluto: 

$$|x| = \begin{cases}
x & \text{se} \; x \geq 0 \\
-x & \text{se} \; x < 0
\end{cases}$$

Partiamo con i limiti a zero. 

$$\begin{align*}
\lim_{x\rightarrow 0^+} \frac{|x|}{x}\cdot 2^{\frac{1}{x-1}}
\end{align*}$$

Vediamo subito che l'esponenziale non ha problemi e $$2^{\frac{1}{x-1}} \rightarrow 2^{-1} = \frac{1}{2}$$. Il problema ce l'abbiamo in $$\frac{|x|}{x}$$ che diventa un $$\frac{0}{0}$$. Notiamo però una cosa: se noi riscriviamo la funzione inserendo la definizione di valore assoluto, otteniamo

$$\begin{align*}
y & = \frac{|x|}{x}\cdot 2^{\frac{1}{x-1}} \\
& = \begin{cases}
\frac{x}{x} \cdot 2^{\frac{1}{x-1}} & \text{se} \; x \geq 0 \\
\frac{-x}{x} \cdot 2^{\frac{1}{x-1}} & \text{se} \; x < 0
\end{cases} \\
& = \begin{cases}
  2^{\frac{1}{x-1}} & \text{se} \; x \geq 0 \\
-2^{\frac{1}{x-1}} & \text{se} \; x < 0
\end{cases}
\end{align*}$$

Con questa riscrittura vediamo subito che quando facciamo il limite per $$x$$ che tende a $$0^+$$ siamo nel primo caso della funzione, mentre quando $$x$$ tende a $$0^-$$ siamo nel secondo caso. Quindi 

$$\begin{align*}
\lim_{x\rightarrow 0^+} \frac{|x|}{x}\cdot 2^{\frac{1}{x-1}} & = \lim_{x\rightarrow 0^+} 2^{\frac{1}{x-1}} \\
& = 2^{-1} \\
& = \frac{1}{2}
\end{align*}$$

$$\begin{align*}
\lim_{x\rightarrow 0^-} \frac{|x|}{x}\cdot 2^{\frac{1}{x-1}} & = \lim_{x\rightarrow 0^-} -2^{\frac{1}{x-1}} \\
& = -2^{-1} \\
& = -\frac{1}{2}
\end{align*}$$

Il punto $$x=0$$ è quindi un punto di discontinuità di prima specie, o di salto, poichè limite destro e sinistro sono entrambi finiti e diversi fra loro. 

Passiamo ora a $$x=1$$.

$$\begin{align*}
\lim_{x\rightarrow 1^+} \frac{|x|}{x}\cdot 2^{\frac{1}{x-1}} & = \lim_{x\rightarrow 1^+} 2^{\frac{1}{x-1}} \\
& = "2^{\frac{1}{0^+}}" \\
& = "2^{+\infty}" \\
& = + \infty 
\end{align*}$$

$$\begin{align*}
\lim_{x\rightarrow 1^-} \frac{|x|}{x}\cdot 2^{\frac{1}{x-1}} & = \lim_{x\rightarrow 1^-} 2^{\frac{1}{x-1}} \\
& = "2^{\frac{1}{0^-}}" \\
& = "2^{-\infty}" \\
& = 0
\end{align*}$$

Il punto $$x=1$$ è quindi un punto di discontinuità di seconda specie poichè uno dei due limiti (quello destro) è infinito. 