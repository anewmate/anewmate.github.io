# CALCOLO COMBINATORIO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 2:

> Determina in quanti modi diversi possiamo distribuire otto tavolette di cioccolato a cinque bambini. 

## Soluzione:

Come prima cosa ricordiamo la differenza fra disposizioni, permutazioni e combinazioni. 

Le **disposizioni** semplici di $$n$$ elementi distinti di classe $$k$$ (con $$k\leq n$$) sono tutti i possibili gruppi che si possono formare con $$k$$ elementi, presi fra gli $$n$$, tali che ogni gruppo è diverso dagli altri per gli elementi contenuti o per il loro ordine. 

Le **permutazioni** semplici di $$n$$ elementi distinti sono tutti i gruppi formati dagli $$n$$ elementi che differiscono per il loro ordine. 

Le **combinazioni** semplici di $$n$$ elementi distinti di classe $$k$$ (con $$k \leq n$$) sono tutti i possibili gruppi che si possono formare con $$k$$ elementi, presi fra gli $$n$$, e tali che ogni gruppo è diverso dagli altri per almeno un elemento contenuto. 

Nel nostro caso abbiamo $$n=5$$ bambini e $$k=8$$ tavolette. Visto che l'ordine con cui i bambini si presentano **non** è importante, siamo nell'ambito delle combinazioni, e non disposizioni (dove invece l'ordine è importante). Tradotto: non importa se prima do una tavoletta al bambino numero 2 e poi una tavoletta al bambino numero 4, ma è importante quante ne ho date a testa. In particolare, abbiamo combinazioni con ripetizione che, ricordiamo, si calcolano come

$$\begin{align*}
C_{n,k}^{'} & = \binom{n+k-1}{k} \\
& = \frac{(n+k-1)\cdot (n+k-2) \cdot \dots \cdot (n+1) \cdot n}{k!}
\end{align*}$$

Nel nostro caso quindi

$$\begin{align*}
C_{5,8}^{'} & = \binom{12}{8} \\
& = \frac{12\cdot 11 \cdot 10 \cdot 9 \cdot 8 \cdot 6 \cdot 5}{8!} \\
& = \frac{12\cdot 11 \cdot 10 \cdot 9 \cdot 8 \cdot 6 \cdot 5}{8\cdot 7 \cdot 6 \cdot 5 \cdot 4 \cdot 3 \cdot 2} \\
& = 11\cdot 5 \cdot 9 \\
& = 495
\end{align*}$$

Possiamo quindi distribuire otto tavolette di cioccolato a cinque bambini in $$495$$ modi diversi.



