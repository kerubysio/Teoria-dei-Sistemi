Materia: [[Teoria dei Sistemi dinamici]]

Negli esercizi in cui devi verificare che un certo T sia un tempo di campionamento congruo per un'approssimazione a dati campionati, ci sono due possibili strade da seguire a seconda della situazione in cui ci troviamo.
Per prima cosa, analizza la fdt e trova i poli. Ci sono due casi:

- poli distanti almeno una decade l'uno dall'altro $\rightarrow$ approssimazione a polo dominante
- poli ravvicinati $\rightarrow$ studio del diagramma di Bode dei moduli
  
## Poli distanti almeno una decade

In questo caso posso approssimare la fdt per poli dominanti, ossia considero solo il polo che ha la parte reale in modulo più piccola, ossia il più vicino all'asse immaginario.
A questo punto, applico la seguente formula:
$$Sia \,\, \tau = \frac{1}{T_{p}}, \,\, \alpha \in [5;10] \,\, e \,\,t_{\alpha_{1}\%} = 4,6\tau$$
Allora avremo che:

$$\frac{t_{\alpha1\%}}{10\alpha} \leq T_{c} \leq \frac{t_{\alpha1\%}}{\alpha}$$
Dopodichè scriviamo la isu con le matrici a fine paragrafo.

## Poli ravvicinati

Nel caso di poli ravvicinati, traccio il diagramma di Bode dei moduli, dopodichè individuo la frequenza in questo modo:
- la frequenza dopo la quale il grafico si trova sempre in una fascia di più o meno tre decibel attorno al valore che il grafico dei moduli assume in 1
- la frequenza dopo la quale il grafico si trova sempre al di fuori di tale fascia di valori
Una volta individuata tale omega, applico questa formula:
$$\alpha \omega_{3} \leq \frac{2\pi}{T_{c}} \leq 10\alpha\omega_{3}$$

## Rappresentazione ISU del sistema a dati campionati

Per rappresentare tale sistema in forma ISU, basta applicare le seguenti formule:
$$\begin{align} A_{D} &= e^{At} = \mathcal{L}^{-1}[(sI-A)^{-1}]  \\ B_{D} &= A^{-1}(A_{D}-I)B  \\ C_{D} &= C  \\ D_{D} &= D \end{align}$$

$$
\begin{align*}
A_{D} &= e^{At} = \mathcal{L}^{-1}\big[(sI-A)^{-1}\big] \\ 
B_{D} &= A^{-1}(A_{D}-I)B \\ 
C_{D} &= C \\ 
D_{D} &= D
\end{align*}
$$
