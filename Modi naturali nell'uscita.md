Materia: [[Teoria dei Sistemi dinamici]]

Se il sistema è stabile, ti basta calcolare separatamente risposta libera e risposta forzata, sommarle e poi porre a zero i termini che non ci interessano. La formula da applicare è:

$$
y(t) = y_{l}(t) + y_{f}(t)
$$
Con:

$$
\begin{align}
y_{l}(t) &= Ce^{At}x(0) = C\mathcal{L}^{-1}[(sI-A)^{-1}] \\
y_{f}(t) &= \mathcal{L}^{-1}[G(s)U(s)]
\end{align}
$$
