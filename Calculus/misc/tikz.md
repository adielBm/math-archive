```
\documentclass[tikz, border={10pt 10pt 10pt 10pt}]{standalone}
\usetikzlibrary{arrows,decorations.markings}
\usetikzlibrary{arrows.meta}% CVS
\begin{document}

\tikz[label position=below, inner sep=+0pt, outer sep=+0pt, every label/.style={font=},
  label distance=+2pt, nodes={font=\bfseries}]
  \draw (+0pt,+0pt) -- node[pos=.2,label=$a_1$] {[}
node[pos=.4,label=$a_2$] {[}
node[pos=0.6,label=$\dots$] {}
node[pos=0.8,label=$a_n$] {[}
node[pos=1.0,label=$\dots$] {}
node[pos=1.2,label=$L$] {|}
node[pos=1.4,label=$\dots$] {}
node[pos=1.6,label=$b_n$] {]} 
node[pos=1.8,label=$\dots$] {}
node[pos=2.0,label=$b_2$] {]} 
++(right:+90pt)
\end{document}
```