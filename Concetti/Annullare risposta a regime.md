Materia: [[Teoria dei Sistemi dinamici]]

---

## Nella pratica

Quando fai un esercizio del genere poni il modulo della fdt pari a 0, poi imponi che le soluzioni trovate abbiano parte reale nulla e, se ci sono parametri, verifica che si trovino nel range in cui il sistema è asintoticamente stabile.

# Zeri immaginari puri e risposta a regime nulla

Quando un sistema lineare e tempo-invariante è stabile e riceve in ingresso una sinusoide  
$$u(t) = \sin(\omega t)$$  
a regime la risposta  y(t)  ha la **stessa frequenza**  $\omega$ , ma un certo **guadagno** e **fase**.  
Se si vuole che la **risposta a regime sia nulla**, per quell'ingresso sinusoidale, la funzione di trasferimento deve soddisfare:

$$ |G(j\omega)|sen(\omega t + \angle{G(j\omega)} ) = 0 \Leftrightarrow |G(j\omega)| = 0 $$

Questo può accadere solo se il sistema ha uno zero in  $s = j\omega$, cioè uno **zero immaginario puro**.  

Per cui se un ingresso ha una frequenza pari alla parte immaginaria dello zero, quella componente viene completamente **eliminata** in uscita.

---

### Perché serve che lo zero sia immaginario puro?

Nel piano complesso $$s = \sigma + j\omega$$
- $\sigma$  (parte reale): determina la crescita o il decadimento esponenziale;
- $\omega$  (parte immaginaria): rappresenta le oscillazioni sinusoidali.

Uno zero **immaginario puro** si trova *esattamente sull'asse immaginario*.  Solo in questo caso il valore della funzione di trasferimento sulla risposta in frequenza,  diventa realmente **zero**.

## In sintesi

**IN SINTESI**: un ingresso sinusoidale introduce nel sistema una frequenza $\omega$, per annullarla è necessario che G(s) si annulli per la stessa frequenza omega (per il teorema della frequenza armonica). Affinchè questo accada, è necessario che ci sia quindi uno zero in $\omega$. Se lo zero ha anche una parte reale, cioè è del tipo $z = \sigma + j\omega$, lo zero si trova sfasato rispetto ad omega, e non in omega.



