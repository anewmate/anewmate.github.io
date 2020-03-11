# DERIVATE

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Calcola la derivata della seguente funzione
$$y = x^3(4-x^2)^2$$

## Soluzione: 

Come prima cosa notiamo che la funzione è data dal prodotto di due funzioni: $$x^3$$ e $$(4-x^2)^2$$. Ricordiamo la regola per la derivata di un prodotto

> Date due funzioni $$f(x)$$ e $$g(x)$$, la derivata (che io indico con il simbolo $$D$$ oppure $$'$$ ) del prodotto è data da

$$D(f(x)\cdot g(x)) = D(f(x))\cdot g(x) + f(x) \cdot D(g(x))$$

Il primo step è quindi

$$D(y) = y' = D(x^3)\cdot (4-x^2)^2 + x^3 \cdot D((4-x^2)^2)$$

Calcolo singolarmente le derivate in questione.

La prima derivata da calcolare è $$D(x^3)$$. Questa è una delle derivate "immediate" per cui esiste una formula diretta per calcolarle. Ricordiamo qual è.

> La derivata di $$x^n$$ con $$n \in \mathbb{R}$$ è 

$$D(x^n) = n \cdot x^{n-1}$$

Nel nostro caso $$n=3$$, quindi 

$$D(x^3) = 3x^2$$

La seconda derivata da calcolare è $$D((4-x^2)^2)$$. Questa è una derivata composta: la funzione più "esterna" è l'elevamento al quadrato, mentre quella più interna è $$4-x^2$$. Ricordiamo anche qui la formula.

> La derivata della composizione di due funzioni $$f(x)$$ e $$g(x)$$ è data da 

$$D(f(g(x))) = f^{'}(g(x)) \cdot g^{'}(x)$$

Nel nostro caso $$f(x) = x^2$$ mentre $$g(x) = 4-x^2$$. Infatti, con queste definizioni, la composizione è

$$f(g(x)) = (4-x^2)^2$$

***

MEMO: Ricordiamo un attimo come funziona la composizione di funzioni. $$f(g(x))$$ significa che devo calcolare $$f$$ non in $$x$$ ma in $$g(x)$$, ossia al posto della $$x$$ nella definizione di $$f$$ devo sostituire la definizione di $$g(x)$$. Nell'esempio precedente $$f(x) = x^2$$ significa che $$f$$ calcolata in $$x$$ è uguale a $$x$$ al quadrato. Se al posto di $$x$$ metto $$g(x)$$ risulta: $$f$$ calcolata in $$g(x)$$ è uguale a $$g(x)$$ al quadrato, ossia $$f(g(x)) = (g(x))^2$$. Se $$g(x) = 4-x^2$$, avrò quindi 

$$f(g(x)) = (4-x^2)^2$$

***
Per applicare la formula della derivata composta dobbiamo quindi calcolare la derivata di $$f$$ (e poi calcolarla in $$g(x)$$) e la derivata di $$g$$. 

Dato che $$f(x) = x^2$$, la derivata è come la prima che abbiamo calcolato:

$$D(f(x)) = f^{'}(x) = D(x^2) = 2x$$

Calcoliamola subito in $$g(x)$$: 

$$f^{'}(g(x)) = 2(g(x)) = 2(4-x^2)$$

Per la derivata di $$g$$ invece dobbiamo usare la formula per la somma/differenza di funzioni, dato che $$g$$ è definita come la differenza fra $$4$$ e $$x^2$$.

> La derivata di una somma/differenza è la somma/differenza delle derivate.

$$D(A(x)\pm B(x)) = D(A(x)) \pm D(B(x))$$

Nel nostro caso, 

$$D(g(x)) = D(4-x^2 ) = D(4) - D(x^2)$$

Ricordandosi che la derivata delle costanti è sempre zero, si ha 

$$D(4) - D(x^2) = 0 - 2x = -2x$$

La derivata composta è quindi

$$D(f(g(x))) = 2(4-x^2)\cdot(-2x)$$

Ora basta solo mettere di nuovo assieme tutti i pezzi:

$$\begin{align*}
D(y) & = y' \\
& = D(x^3)\cdot (4-x^2)^2 + x^3 \cdot D((4-x^2)^2) \\
& = 3x^2 \cdot (4-x^2)^2 + x^3 \cdot 2(4-x^2)(-2x) \\
& = 3x^2(4-x^2)^2 - 4x^4(4-x^2)
\end{align*}$$

Ufficialmente la derivata è finita qui. Ora si tratta solo di rendere un po' più ordinata quell'espressione. Raccogliamo a fattor comune $$x^2(4-x^2)$$ e otteniamo

$$\begin{align*}
y^{'} & = x^2(4-x^2) \cdot (3(4-x^2)-4x^2) \\
& = x^2(4-x^2) \cdot (12-3x^2-4x^2) \\
& = x^2(4-x^2)(12-7x^2)
\end{align*}$$
