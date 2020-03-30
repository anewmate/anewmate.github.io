# INTEGRALI

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 3:

> Calcola il seguente integrale

$$\int \frac{\cos(3x)}{2\sqrt{\sin(3x)}}dx$$

## Soluzione: 

Come prima cosa noto che l'integrale è indefinito. Come seconda cosa, vedo che a numeratore c'è un coseno mentre a denominatore c'è la radice di un seno, entrambi con lo stesso argomento $$3x$$. Ricordandosi che la derivata del seno è il coseno, ci si accende la lampadina che potremmo essere di fronte all'integrale di una funzione composta. 

Ricordiamo un attimo come funzionano le derivate composte. Indico con $$D$$ o $$'$$ il simbolo di derivata. 

$$D(f(g(x))) = f^{'}(g(x))\cdot g^{'}(x)$$

In parole semplici, prima devo identificare $$f(x)$$ e $$g(x)$$ tali che $$f$$ calcolata in $$g(x)$$ sia uguale alla funzione di cui voglio calcolare la derivata. Dopodichè calcolo $$f^{'}(x)$$ e $$g^{'}(x)$$ e infine calcolo la derivata di $$f$$ in $$g(x)$$. 

Perchè sto parlando di derivate quando dobbiamo calcolare un integrale? Ricordo che calcolare un integrale significa trovare quella funzione la cui derivata coincide con l'argomento dell'integrale. In altre parole, l'integrale di una funzione è un'altra funzione tale che, se la derivo, ottengo la funzione di cui volevo calcolare l'integrale. 

Nel nostro caso, proviamo a calcolare la derivata di $$\sqrt{\sin(3x)}$$. Perchè esattamente questa funzione visto che nell'integrale abbiamo $$\frac{1}{\sqrt{\sin(3x)}}$$?

Perchè, sapendo bene le derivate, so che $$D(\sqrt{x}) = \frac{1}{2\sqrt{x}}$$, e se al posto di $$x$$ metto $$\sin(3x)$$ ottengo qualcosa di molto simile a quello che abbiamo noi. 

Quindi, per calcolare la derivata di $$\sqrt{\sin(3x)}$$ dobbiamo applicare la formula di derivata di una funzione composta. 

In particolare abbiamo 

$$f(x) = \sqrt{x}$$

$$g(x) = \sin(3x)$$

Infatti, $$f(g(x))$$ ossia $$f$$ calcolata in $$g(x)$$ invece che in $$x$$, è

$$f(g(x)) = \sqrt{\sin(3x)}$$

(in parole semplici dove c'è $$x$$ nella definizione di $$f$$ dobbiamo mettere $$g(x)$$). 

Ora che abbiamo individuato $$f$$ e $$g$$ calcoliamo le loro derivate.

$$D(f(x)) = \frac{1}{2\sqrt{x}}$$

$$D(g(x)) = \cos(3x) \cdot 3$$

Nota: anche derivare $$g$$ significa utilizzare la formula di derivata composta. 

Ultima cosa da calcolare è $$f^{'}(g(x))$$:

$$f^{'}(g(x)) = \frac{1}{2\sqrt{\sin(3x)}}$$

Mettendo insieme tutti i pezzi ho quindi 

$$\begin{align*}
D(\sqrt{\sin(3x)}) & = \frac{1}{2\sqrt{\sin(3x)}} \cdot 3\cos(3x) \\
& = 3 \cdot \frac{\cos(3x)}{2\sqrt{\sin(3x)}}
\end{align*}$$

Vediamo quindi che non abbiamo ottenuto esattamente l'argomento del nostro integrale, ma quasi: manca solo quel $$3$$ che moltiplica tutto. 

Visto che le costanti si possono gestire facilmente con gli integrali, procedo in questo modo: 

$$\begin{align*}
\int \frac{\cos(3x)}{2\sqrt{\sin(3x)}}dx & = \int \frac{1}{3} \cdot 3 \cdot \frac{\cos(3x)}{2\sqrt{\sin(3x)}}dx \\
& = \frac{1}{3} \int 3 \cdot \frac{\cos(3x)}{2\sqrt{\sin(3x)}}dx \\
& = \frac{1}{3} \int D(\sqrt{\sin(3x)})dx \\
& = \frac{1}{3}\sqrt{\sin(3x)} +c
\end{align*}$$

A parole: visto che mi serve l'argomento dell'integrale moltiplicato per $$3$$, lo moltiplico (e divido, altrimenti non ottengo qualcosa di equivalente) per $$3$$. Così facendo ottengo come argomento dell'integrale la derivata che ho appena calcolato. Per definizione di integrale infine, l'integrale di una derivata è l'argomento della derivata. Ricordo sempre di aggiungere la costante alla fine in quanto l'integrale è indefinito. 

Quindi,

$$\int \frac{\cos(3x)}{2\sqrt{\sin(3x)}}dx = \frac{1}{3}\sqrt{\sin(3x)} +c$$






