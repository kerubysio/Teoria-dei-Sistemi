## Zeri immaginari puri e risposta a regime nulla

Quando un sistema lineare e tempo-invariante è stabile e riceve in ingresso una sinusoide  
$$ u(t) = \sin(\omega t) $$  
a regime la risposta  y(t)  ha la **stessa frequenza**  $\omega$ , ma un certo **guadagno** e **fase**.  
Se si vuole che la **risposta a regime sia nulla**, per quell'ingresso sinusoidale, la funzione di trasferimento deve soddisfare:

$$ |G(j\omega)|sen(\omega t + \angle{G(j\omega)} ) = 0 \Leftrightarrow |G(j\omega)| = 0 $$

Questo può accadere solo se il sistema ha uno zero in  $s = j\omega$, cioè uno **zero immaginario puro**.  

Per cui se un ingresso ha una frequenza pari alla parte immaginaria dello zero, quella componente viene completamente **eliminata** in uscita.

---

### Perché serve che lo zero sia immaginario puro?

Nel piano complesso $$ s = \sigma + j\omega $$
- $\sigma$  (parte reale): determina la crescita o il decadimento esponenziale;
- $\omega$  (parte immaginaria): rappresenta le oscillazioni sinusoidali.

Uno zero **immaginario puro** si trova *esattamente sull'asse immaginario*.  Solo in questo caso il valore della funzione di trasferimento sulla risposta in frequenza,  diventa realmente **zero**.

**IN SINTESI**: un ingresso sinusoidale introduce nel sistema una frequenza $\omega$, per annullarla è necessario che G(s) si annulli per la stessa frequenza omega (per il teorema della frequenza armonica). Affinchè questo accada, è necessario che ci sia quindi uno zero in $\omega$. Se lo zero ha anche una parte reale, cioè è del tipo $z = \sigma + j\omega$, lo zero si trova sfasato rispetto ad omega, e non in omega.

---

### Sintesi

- **Zeri in $$ \pm j\omega $$ → $$ G(j\omega)=0 $$ → la sinusoide di frequenza $$ \omega $$ viene totalmente annullata.**  
- **Zeri con parte reale negativa → $$ G(j\omega) \neq 0 $$ → attenuano, ma non annullano.**  
- **Zeri con parte reale positiva → destabilizzano o amplificano.**

---

### Applicazione al problema visto

Nel sistema dato, gli zeri sono:

$$
z_{1,2} = \frac{-k \pm \sqrt{k^2 + 8hk}}{2}.
$$

Per avere zeri immaginari puri serve che la **parte reale sia nulla**, quindi $$ k = 0 $$.  
Ma la stabilità richiede $$ h < 0 \ \wedge \ k < 0 $$.  
Se $$ k = 0 $$ la stabilità viene meno e gli zeri si riducono a $$ z = 0 $$ (niente parte immaginaria).

**Conclusione:** non è possibile scegliere valori di $$ h $$ e $$ k $$ tali da avere:
- sistema stabile **e**
- zeri in $$ \pm j\omega $$.

Quindi **il sistema non può mai annullare a regime una sinusoide in ingresso**.

