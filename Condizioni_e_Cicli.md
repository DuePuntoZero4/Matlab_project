# Blocchi condizionali
A volte può risultare necessario, sia in script che in funzioni, fare scelte diverse in base al valore delle variabili a disposizione; per questo motivo, l'utilizzo dei blocchi condizionali è fondamentale.
## Sintassi
```matlab
if (condizione1)
  %istruzioni  
elseif (condizione2)
  %istruzioni
else                  %caso base
  %istruzioni
end
```
L'editor dà automaticamente l'indentazione, nonostante non risulti essenziale. Come per le funzioini, l'utilizzo della parola chiave `end` indica il termine dell'istruzione di ciclo.
## Operatori logici
Le condizioni, sia per cicli che per i blocchi condizionali, hanno valore booleano, e sono quindi modificabili con l'utilizzo degli operatori logici:
- `&` → AND: restituisce vero (1) se entrambi i valori comparati sono veri; può essere utilizzato anche per vettori ed array *se e solo se* sono della stessa grandezza.
- `|` → OR: restituisce vero (1) se almeno uno tra i valori comparati è vero; può essere utilizzato anche per vettori ed array *se e solo se* sono della stessa grandezza.
- `~` → NOT: prende ogni elemento della matrice e ne inverte il valore logico.
- `xor(..., ...)` → XOR: compara elemento per elemento le due matrici e ne restituisce una terza avente in *i,j*-esima posizione un 1 se solo uno tra gli elementi *i,j*-esimi delle due matrici è uno zero; questo perché, come per altri linguaggi, 0 corrisponde al falso booleano, mentre ≠0 viene considerato vero.
# Cicli
## Ciclo for
```matlab
for variabile = vettore
  %istruzioni
end
```
Analizziamo la sintassi:
- `variabile` è una variabile temporanea (definita prima del ciclo) che assume il valore successivo del vettore ad ogni iterazione.
- `vettore` è da dove prendiamo i valori che la nostra variabile temporanea assumerà; una volta finiti i valori, il ciclo terminerà automaticamente.
- `end` indica la fine del blocco di istruzioni da ripetere.
## Ciclo while
```matlab
while (condizione)
  %istruzioni
end
```
Analizziamo la sintassi:
- `condizione` è un'espressione logica che ci permette di rimanere nel ciclo finché è vera.
- `end` indica la fine del blocco di istruzioni da ripetere.
