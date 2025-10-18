Materia: [[Teoria dei Sistemi dinamici]]

# Forma canonica di Kalman

Scrivi lo spazio di raggiungibilità prendendo le colonne linearmente indipendenti di R: 

$$X_{R} = <\begin{bmatrix} col_{1} && col_{2} && \dots && col_{i}  \end{bmatrix}>$$

Allo stesso modo costruiamo anche lo spazio di osservabilità prendendo le colonne linearmente indipendenti di O, come segue:

$$X_{O} = <\begin{bmatrix} col_{1} && col_{2} && \dots && col_{i}  \end{bmatrix}>$$

A questo punto si calcolano gli spazi non raggiungibili e non osservabili, calcola i nulli di R e di O in questo modo, ricordandoti di fare le TRASPOSTE:

$$R^T \underline{z} = \begin{pmatrix}r_{11} && \dots && r_{1r} \\ \vdots && \dots && \vdots \\ r_{r1} && \dots && r_{rr} \end{pmatrix}^T \begin{pmatrix}z_{1} \\ \vdots \\ z_{r}\end{pmatrix} = \underline{0}$$

Le soluzioni di questa equazione ci restituiranno lo spazio non raggiungibile, ossia $X_{NR}$.

In modo analogo calcoliamo lo spazio non osservabile, come segue:

$$O^T \underline{z} = \begin{pmatrix}o_{11} && \dots && o_{1o} \\ \vdots && \dots && \vdots \\ o_{o1} && \dots && o_{oo} \end{pmatrix}^T \begin{pmatrix}z_{1} \\ \vdots \\ z_{r}\end{pmatrix} = \underline{0}$$

Le soluzioni di questa equazione ci restituiranno lo spazio di non osservabilità, ossia $X_{NO}$.

