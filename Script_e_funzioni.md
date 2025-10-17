# Script
Uno script è un semplice file di testo contenente una serie di istruzioni da eseguire riga per riga; In Matlab uno script deve avere estensione `.m`.

Uno script condivide le variabili del workspace, ma soprattutto è statico, ovvero non ha input o logica parametrica per cambiare comportamento, eseguendo sempre la stessa sequenza di comandi nello stesso modo.
# Funzioni
Per MatLab, ogni funzione dev'essere salvata su un file diverso (sempre però con estensione `.m`). A differenza degli script, le funzioni:
- ricevono input
- elaborano dati
- restituiscono un output

**ATTENZIONE**: il nome della funzione dev'essere lo stesso del nome del file che la contiene (esclusa l'estensione).
## Sintassi di una funzione
```matlab
function [out1, out2, ...] = nome_funzione (in1, in2, ...)
  %corpo della funzione
end
```
Analizziamo la sintassi:
- La parola chiave `function` (riga 1) indica a MatLab che il file contiene una funzione piùttosto che uno script.
- Gli argomenti di `function` indicano i valori restituiti dalla funzione all'istanza chiamante.
- `nome_funzione` indica il nome della funzione del file, che ricordiamo deve corrispondere al nome del file stesso.
- Gli argomenti di `nome_funzione` indicano i valori ricevuti dall'istanza chiamante.
- `end` indica la chiusura della funzione.
## Funzioni anonime (chiamate inline in precedenza)
È possibile definire funzioni "rapide" senza dover creare un nuovo file per ognuna; queste funzioni prendono il nome di anonime proprio perché non hanno un nome proprio, ma vengono create assegnandole ad una variabile.
```matlab
f = @(arg) espressione
```
- `f` sarà il nome della "funzione" (ovvero della variabile a cui l'assegneremo).
- `arg` è lo spazio dedicato agli argomenti della funzione.
- `espressione` è l'istruzione che la nostra funzione eseguirà; le funzioni anonime possono contenere un'istruzione sola.
