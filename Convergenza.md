# Convergenza
Con convergenza intendiamo la proprietà di una qualche funzione o successione di avere un limite finito di qualche tipo quando il parametro da cui dipende tende verso un valore specifico o un infinito.

Parleremo di convergenza per limiti, successioni, serie e funzioni.
## Successioni
In matematica, una successione è una funzione $`a_n:\mathbb{N}→\mathbb{R}`$ che associa ad ogni $`n`$ un valore $`a_n`$.

In *MatLab*, una successione si rappresenta come un vettore.
```matlab
n=1:10;               % creiamo un vettore di indici
a=1./n;               % inizializziamo una successione con formula a_n=1/n
```
Ricordiamo che il punto indica un'operazione elemento per elemento sul vettore di indici.

Se una successione è definita ricorsivamente, possiamo utilizzare un ciclo for o while.
## Limiti
In matematica, un limite descrive il comportamento di funzioni e successioni quando il parametro da cui dipendono si avvicina ad un certo valore, sia esso finito o infinito.

In *MatLab*, un limite può essere calcolato in due modi:
- Simbolicamente: utilizziamo i comandi `syms` e `limit(...)` per calcolare il limite esatto, come se non fossimo limitati dalla precisione della macchina.
- Numericamente: attraverso approssimazioni, arriviamo a valori molto vicini a quelli reali.

Noi utilizzeremo il secondo metodo, sfruttando le successioni per calcolare i limiti, ma per completezza, meglio aggiungere un esempio con il calcolo simbolico.
```matlab
syms x                 % creiamo una variabile simbolica che rappresenta un simbolo matematico
f = (x^2 - 4)/(x - 2); % definiamo la funzione su cui calcolare il limite
limit(f, x, 2)         % calcoliamo il limite matematico di una funzione con parametri simbolici
```
Alla funzione limit passiamo la funzione $`f`$, la variabile rispetto alla quale calcoliamo il limite e il punto a cui tende quella variabile.
## Serie
In matematica, una serie è la somma dei termini di una successione. Siccome possiamo dover rappresentare sia serie finite che infinite.

Anche le serie numeriche verranno trattate attraverso le successioni.
