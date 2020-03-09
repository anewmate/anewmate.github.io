# CIRCONFERENZA

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Scrivi le equazioni delle rette tangenti alla circonferenza di equazione $$x^2+y^2-2x-3 = 0$$ condotte dal punto $$P(-1;3)$$.

## Soluzione: 

Come prima cosa disegniamo la circonferenza e il punto, giusto per visualizzare gli elementi del problema.

Ricordiamo le formule per trovare il centro e il raggio.

> Data l'equazione $$x^2+y^2+ax+by+c=0$$, il centro $$C(x_C,y_C)$$ ha coordinate

$$x_C = -\frac{a}{2}, \qquad y_C = - \frac{b}{2}$$

>mentre il raggio è 

$$r = \sqrt{\left(-\frac{a}{2}\right)^2 + \left(-\frac{b}{2}\right)^2 -c}$$

Nel nostro caso l'equazione è $$x^2+y^2-2x-3=0$$, quindi abbiamo $$a=-2,b=0,c=-3$$. Il centro ha quindi coordinate $$C(1,0)$$ e raggio $$r=\sqrt{1+3} = 2$$.

$$\begin{tikzpicture}
\draw[->] (-2,0) -- (4,0);
\draw[->] (0,-3) -- (0,4);
\draw (1,0) circle (2cm);
\draw[fill=black] (-1,3) circle (0.05cm);
\draw[fill=black] (1,0) circle (0.05cm);
\node at (1,0.5) {C};
\node at (-1,3.5) {P};
\end{tikzpicture}$$

Nota: già graficamente possiamo vedere che una tangente sarà la retta $$x=-1$$, ma troviamola seguendo il procedimento standard. 

Per trovare le tangenti utilizziamo quello che solitamente si chiama Metodo 2, ossia imponiamo che la distanza fra il centro e le rette passanti per $$P$$ sia uguale al raggio.

Il fascio di rette passante per $$P$$ è dato da: $$y-y_P = m(x-x_P)$$, ossia nel nostro caso $$y-3 = m(x+1)$$.

Memo: i fasci di rette NON includono le rette verticali, ossia quelle parallele all'asse $$y$$.

Memo: dato un punto $$P(x_P;y_P)$$ e una retta $$ax+by+c = 0$$, la distanza del punto dalla retta è definita come 

$$d = \frac{|a\cdot x_P + b \cdot y_P + c|}{\sqrt{a^2+b^2}}$$

Riscrivo quindi il fascio di rette come $$mx-y+m+3 = 0$$ e pongo la distanza fra questo e il centro $$C(1,0)$$ uguale a $$2$$ (il raggio):

$$2 = \frac{|m\cdot 1 -1 \cdot 0 + m+3|}{\sqrt{m^2+1}}$$

Moltiplico destra e sinistra per la radice e ottengo

$$2\sqrt{m^2+1} = |2m+3|$$

Elevo al quadrato sia a destra che a sinistra e ottengo 

$$4(m^2+1) = 4m^2+9+12m$$

Moltiplico a sinistra, porto tutti i termini in $$m$$ a sinistra e tutti quelli senza a destra

$$4m^2 - 4m^2 - 12m = +9-4$$ 

$$-12m = +5$$

Divido destra e sinistra per $$-12$$ in modo da isolare la $$m$$:

$$m = -\frac{5}{12}$$

Otteniamo un solo valore di $$m$$ a cui corrisponde la retta di equazione 

$$y-3 = -\frac{5}{12}(x+1)$$

$$y = -\frac{5}{12}x -\frac{5}{12}+3$$

$$y = -\frac{5}{12}x +\frac{31}{12}$$

Il punto $$P$$ è esterno alla circonferenza, quindi le tangenti devono essere due. Avendo determinato, mediante l'equazione del fascio, una sola retta, l'altra tangente deve essere parallela all'asse $$y$$.  Poichè $$P$$ ha ascissa $$-1$$, l'altra tangente ha equazione

$$x=-1$$

$$\begin{tikzpicture}
\draw[->] (-2,0) -- (4,0);
\draw[->] (0,-2.5) -- (0,4);
\draw (1,0) circle (2cm);
\draw[fill=black] (-1,3) circle (0.05cm);
\draw[fill=black] (1,0) circle (0.05cm);
\node at (1,0.5) {C};
\node at (-1,3.5) {P};
\draw[red] (-1,3) -- (-1,-2.5);
\draw[red] (-1,3) -- (4,11/12);
\node[red] at (-1,-3) {$x=-1$};
\node[red] at (4.5,0.5) {$y = -\frac{5}{12}x +\frac{31}{12}$};
\end{tikzpicture}$$

<!--ossia mettiamo a sistema la circonferenza con il fascio di rette passante per $$P$$ e poi poniamo $$\Delta = 0$$.
Il fascio di rette passante per $$P$$ è dato da: $$y-3 = m(x+1)$$
Lo metto a sistema con la circonferenza:
$$\begin{align*}
&\begin{cases}
y-3 = mx +m \\
x^2+y^2-2x-3=0
\end{cases}
\end{align*}$$
Isolo $$y$$ e lo sostituisco nella seconda equazione:
$$
&\begin{cases}
y = mx +m +3\\
x^2+(mx +m +3)^2-2x-3=0
\end{cases}
\end{align*}$$
Considero ora solo l'equazione $$x^2+(mx +m +3)^2-2x-3=0$$
$$\begin{align*}
& x^2+(mx +m +3)^2-2x-3=0 \\
& x^2 +m^2x^2+m^2x+3mx+m^2x+m^2+3m+3mx+3m+9-2x-3 = 0 \\
& (1+m^2)x^2 + (m^2+3m+m^2-2)x +m^2+3m+3m+9-3 = 0 \\
& \underbrace{(1+m^2)}_{a}x^2 +\underbrace{(2m^2+3m-2)}_{b}x+\underbrace{m^2+6m+6}_{c}=0
\end{align*}$$
Abbiamo quindi un'equazione di secondo grado in cui dobbiamo imporre il delta uguale a zero. Ricordiamo che $$\Delta = b^2-4ac$$.
$$\begin{align*}
\Delta & = (2m^2+3m-2)^2-4(1+m^2)(m^2+6m+6) \\
& = 4m^4+6m^3-4m^2+6m^3+9m^2-6m-4m^2-6m+4-4(m^2+6m+6+m^4+6m^3+6m^2) \\
& = 4m^4+12m^3+m^2-12m+4 -4m^2-24m-24-4m^4-24m^3-24m^2 \\
& = -12m^3-27m^2-36m-24
\end{align*}$$
Porre $$\Delta = 0$$ significa risolvere $$-12m^3-27m^2-36m-24 = 0$$.
$$\begin{align*}
-12m^3-27m^2-36m-24 & = 0 \\
-3(4m^3+9m^2+12m+8)& = 0 \\
4m^3+9m^2+12m+8 & = 0
\end{align*}$$-->