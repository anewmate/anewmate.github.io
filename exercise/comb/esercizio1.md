# CALCOLO COMBINATORIO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 1:

> Determina in quanti modi possono disporsi in fila tre gettoni rossi e quattro gialli se il primo gettone deve essere giallo.

## Soluzione:

Come prima cosa ricordiamo la differenza fra disposizioni, permutazioni e combinazioni. 

Le **disposizioni** semplici di $$n$$ elementi distinti di classe $$k$$ (con $$k\leq n$$) sono tutti i possibili gruppi che si possono formare con $$k$$ elementi, presi fra gli $$n$$, tali che ogni gruppo è diverso dagli altri per gli elementi contenuti o per il loro ordine. 

Le **permutazioni** semplici di $$n$$ elementi distinti sono tutti i gruppi formati dagli $$n$$ elementi che differiscono per il loro ordine. 

Le **combinazioni** semplici di $$n$$ elementi distinti di classe $$k$$ (con $$k \leq n$$) sono tutti i possibili gruppi che si possono formare con $$k$$ elementi, presi fra gli $$n$$, e tali che ogni gruppo è diverso dagli altri per almeno un elemento contenuto. 

Nel nostro caso ci stanno sostanzialmente chiedendo come si possono mettere in fila 7 gettoni. Siamo quindi nel caso delle permutazioni. 

Essendo però i 7 gettoni divisi in 3 rossi e 4 gialli, siamo nello specifico nel caso di permutazioni con ripetizione. La regola ci dice che le permutazioni di $$n$$ elementi di cui $$h,k$$ ripetuti sono 

$$P_n^{(h,k)} = \frac{n!}{h!\cdot k!}$$

dove con "!" indico il simbolo del fattoriale.

Poichè ci dicono che il primo gettone deve essere fissato giallo, nel nostro caso $$n = 6$$ (7 meno quello fissato), $$h = 3$$ (gettoni rossi) e $$k = 3$$ (gettoni gialli, 4 meno uno fissato). Quindi i gettoni possono disporsi in fila in 

$$\begin{align*}
P_6^{(3,3)} & = \frac{6!}{3! \cdot 3!} \\
& = \frac{6\cdot 5 \cdot 4 \cdot 3!}{3! \cdot 3 \cdot 2} \\
& = \frac{6\cdot 5 \cdot 4}{3 \cdot 2} \\
& = 2 \cdot 5 \cdot 2 \\
& = 20
\end{align*}$$

modi.

