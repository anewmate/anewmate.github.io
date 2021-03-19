# DISEQUAZIONE ESP E LOG

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 5:

> Risolvi la seguente disequazione applicando il metodo necessario

$$2^x < \frac{7^{x+1}}{2}$$

## Soluzione: 

Avendo esponenziali con basi diverse, escludo in metodo di sostituzione (introducendo un'incognita ausiliaria). L'obiettivo è quindi quello di arrivare utilizzare le proprietà delle potenze e arrivare a una forma del tipo $$a^x \gtrless b$$ con $$a>0$$. 

$$\begin{align*}
2^x & < \frac{7^{x+1}}{2} \\
2^x & < \frac{7^{x} \cdot 7^1}{2} \\
\frac{1}{7^x} \cdot 2^x & < \frac{7^{x} \cdot 7}{2} \cdot \frac{1}{7^x} \\
\frac{2^x}{7^x} & < \frac{7}{2} \\
\left(\frac{2}{7}\right)^x & < \left(\frac{2}{7}\right)^{-1} \\
& \downarrow \\
\text{base minore di uno:} & \; \; \text{inverto il verso} \\
x & > -1
\end{align*}$$

Nota: posso tranquillamente dividere destra e sinistra per $$7^x$$ senza preoccuparmi del segno (e quindi del verso della disuguaglianza) perchè **gli esponenziali sono sempre strettamente positivi**. 

