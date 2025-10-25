Materia: [[Teoria dei Sistemi dinamici]]
# $G_i$ dentro ai blocchi
Controlla il numero di n ingressi e di m uscite. La fdt sarà una matrice con n righe ed m colonne, del tipo:

$$
W(s) =\begin{pmatrix} w_{00} && \dots && w_{0m} \\
\vdots && \vdots && \vdots \\ w_{n0} && \dots && w_{nm}  \\ \\
\end{pmatrix}
$$ 

Possiamo calcolare ogni componente della W(s) tramite il teorema della sovrapposizione degli effetti, ossia considerando di volta in volta un solo ingresso come attivo e spegnendo gli altri due.
Spesso ti può convenire di scrivere direttamente le singole $W_{i}$ senza passare prima per la Y(s), basta che guardi lo schema a blocchi e sostituisci a mente paralleli, serie e retroazioni.

## Attento

![Schema a blocchi](../Immagini/Schemi%20a%20blocchi.png)

Nota che quando spegni il primo ingresso e lasci solo il secondo attivo, se c'è un nodo come quello dell'immagine, devi mettere un segno meno davanti alla fdt del nodo precedente ad esso.
Inoltre, nello schema della figura nota come lei considera la parte sopra come fdt unitaria. Per capirne il senso ti basta provare a ridisegnare questo schema mettendo l'ingresso a sinistra come si fa di solito.