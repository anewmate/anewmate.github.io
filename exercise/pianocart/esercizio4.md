# PIANO CARTESIANO

<!--Upmath extremely simplifies this task by using Markdown and LaTeX. It converts the Markdown syntax extended with LaTeX equations support into HTML code you can publish anywhere on the web.-->

<!--![Paper written in LaTeX](/i/latex.jpg)-->

## 

Esercizio 4:

> Stabilisci se il triangolo $$ABC$$ di vertici $$A(-5;6), B(-1;4), C(4;-1)$$ è isoscele. 

## Soluzione: 

Come prima cosa mi disegno i tre punti in un sistema di riferimento cartesiano: non è richiesto dall'esercizio, ma sono sempre dell'idea che visualizzare aiuta. 

$$\begin{tikzpicture}
\draw[->] (-6,0) -- (5,0);
\draw [->] (0,-2) -- (0,7);
\draw (1,-0.2) -- (1,0.2);
\draw (2,-0.2) -- (2,0.2);
\draw (3,-0.2) -- (3,0.2);
\draw (4,-0.2) -- (4,0.2);
\draw (-1,-0.2) -- (-1,0.2);
\draw (-2,-0.2) -- (-2,0.2);
\draw (-3,-0.2) -- (-3,0.2);
\draw (-4,-0.2) -- (-4,0.2);
\draw (-5,-0.2) -- (-5,0.2);
\draw (-0.2,1) -- (0.2,1);
\draw (-0.2,2) -- (0.2,2);
\draw (-0.2,3) -- (0.2,3);
\draw (-0.2,4) -- (0.2,4);
\draw (-0.2,5) -- (0.2,5);
\draw (-0.2,6) -- (0.2,6);
\draw (-0.2,-1) -- (0.2,-1);
\node at (5.5,0) {$x$};
\node at (0,7.5) {$y$};
\draw[fill=red] (-5,6) circle (0.07cm);
\draw[fill=red] (-1,4) circle (0.07cm);
\draw[fill=red] (4,-1) circle (0.07cm);
\draw (-5,6) -- (-1,4);
\draw (-5,6) -- (4,-1);
\draw (-1,4) -- (4,-1);
\node[red] at (-5,6.5) {$A$};
\node[red] at (-1,4.5) {$B$};
\node[red] at (4,-1.5) {$C$};
\end{tikzpicture}$$

Per stabilire se il triangolo è isoscele devo verificare se ha due lati della stessa lunghezza. 

**Memo**: si definisce triangolo isoscele un triangolo che possiede due lati congruenti.

Devo quindi calcolare la lunghezza dei segmenti $$\overline{AB}, \overline{AC}, \overline{BC}$$. Per fare ciò, devo ricordarmi come si calcola la distanza fra due punti nel piano cartesiano. 

La distanza fra due punti $$A(x_A;y_A)$$ e $$B(x_B;y_B)$$ è data da 

$$\overline{AB} = \sqrt{(x_B-x_A)^2+(y_B-y_A)^2}$$

Nel nostro caso quindi 

$$\begin{align*}
\overline{AB} & = \sqrt{(-1-(-5))^2+(4-(6))^2} \\
& = \sqrt{4^2+(-2)^2} \\
& = \sqrt{16+4} \\
& = \sqrt{20} \\
\overline{AC} & = \sqrt{(4-(-5))^2+(-1-(6))^2} \\
& = \sqrt{9^2+(-7)^2} \\
& = \sqrt{81+49} \\
& = \sqrt{130} \\
\overline{BC} & = \sqrt{(4-(-1))^2+(-1-(4))^2} \\
& = \sqrt{5^2+(-5)^2} \\
& = \sqrt{25+25} \\
& = \sqrt{50}
\end{align*}$$

I tre lati del triangolo hanno tutti lunghezze differenti, quindi possiamo concludere che il triangolo NON è isoscele.


 