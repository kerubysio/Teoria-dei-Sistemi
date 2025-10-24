Materia: [[Teoria dei Sistemi dinamici]]
# Calcolo della risposta forzata
Quando calcoli la risposta forzata, a volte dopo aver fatto i fratti semplici ti potresti trovare in una situazione del tipo:

$$y(k) = Z^{-1}\left[\frac{A}{z-p_{i} } + \frac{B}{z-p_{j}}\right]$$

È facile notare che dopo aver risolto i fratti, avremo al numeratore due costanti. Per calcolare la Z antitrasformata però, ci servirebbe una z al numeratore di entrambi i fattori. Per farla comparire in un modo che ci semplifichi la vita, procediamo in questo modo:
* Nella funzione di partenza, prima dei fratti, moltiplichiamo e dividiamo per z
* Adesso, calcoliamo i fratti semplici senza però considerare la z al numeratore, in questo modo l'equazione di sopra diventa:  $y(k) = Z^{-1}\left[(\frac{A}{z-p_{i}} + \frac{B}{z-p_{j}} + \frac{C}{z})z \right]$
* A questo punto, quando calcoliamo A, B e C, li sostituiamo e moltiplichiamo per la z esterna