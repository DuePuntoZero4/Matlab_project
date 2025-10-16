# Comandi
Questo file presenta un elenco dei comandi che abbiamo visto / vedremo a lezione.
## Comandi ereditati da Shell (bash)
- `pwd` → *Print Working Directory*: stampa in output (nella Command Window) la cartella di lavoro corrente come una stringa.
- `ls` → *List Directory Contents*: elenca (sempre nella Command Window) i file e le sottocartelle della directory corrente; se viene aggiunto un percorso di una cartella come argomento, elenca i contenuti di quella cartella.
- `mkdir` → *Make Directory*: crea una nuova cartella all'interno della cartella corrente, con nome la stringa specificata nell'argomento.
- `cd` → *Change Directory*: questo comando può essere utilizzato in due modi:
  - senza argomento, ritorni alla cartella madre.
  - con argomento, entri in una sottocartella della cartella corrente.
- `delete`: cancella il file specificato dall'argomento.
## Comandi base
**ATTENZIONE**: la scrittura `<...>` indica lo spazio dove va aggiunto l'argomento del comando / funzione, quindi i simboli maggiore e minore non fanno parte del comando e vanno omessi.
- `clc`: svuota la Command Window di tutti i contenuti, ma senza eliminare le variabili definite o i loro valori.
- `whos <...>`: può essere usata in due modi:
  - senza argomento, mostra tutte le variabili del workspace, il loro tipo, la loro dimensione e lo spazio che ognuna occupa in memoria.
  - con argomento (il nome di una variabile), funziona come la precedente, ma solo per la variabile specificata.
- `clear <...>`: può essere usata in due modi:
  - senza argomento, cancella tutte le variabili dal workspace.
  - con argomento (il nome di una variabile), funziona come la precedente, ma solo per la variabile specificata.
- `close <...>`: può essere usata in tre modi:
  - con argomento `all`, chiude tutte le finestre grafiche attualmente aperte.
  - con argomento il nome di una finestra, chiude la finestra grafica corrispondente.
  - senza argomento, chiude la finestra corrente.
- `help <...>`: mostra un riassunto della documentazione di una funzione o un comando.
- `%`: inizia un commento valido dal simbolo di percentuale sino al fine riga.
- `save <nome_file.mat> <...>`: salva il workspace in un file *nome_file.mat* che verrà aggiunto alla directory corrente; possono essere aggiunti i nomi di variabili come argomento per fare un salvataggio selettivo dei dati.
- `load <nome_file.mat>`: carica nel workspace le variabili contenute nel file.
# Operazioni ed operatori
In generale, MatLab è una calcolatrice scientifica sotto steroidi; di conseguenza, valgono le normali regole di calcolo usati da altri linguaggi di programmazione.
Un'operazione in matlab può essere definita con `;` finale o senza. Nel primo caso, il risultato non verrà mostrato nella Command Window, mentre nel secondo comparirà associato alla variabile predefinita *ans*.
Le operazioni di base di MatLab sono 6:
- addizione `+`
- sottrazione `-`
- moltiplicazione `*`
- divisione `/`
- potenza `^`
- assegnazione `=`
## Operazioni su vettori
- `v(1)`: stampa nella Command Window il valore salvato nella prima cella di v.
  - `v(end)` stampa invece sempre l'ultimo valore.
  - `v(index)` permette di scorrere l'array in base al valore assunto da index stesso.
- `v+w`: somma membro a membro due vettori *se e solo se* sono della stessa lunghezza.
- `v*2`: moltiplica ogni membro del vettore per uno scalare.
- `v*w'`: prodotto scalare tra due vettori (dove w subisce una operazione di casting); restituisce la somma dell'*i*-esimo termine di v moltiplicato con l'*i*-esimo termine di w per tutti i valori dei due vettori.
- `v.*w`: salva in ans un array avente la stessa dimensione di v e w con valori il prodotto membro a membro dei precedenti (*se e solo se* sono della stessa lunghezza).
## Operazioni su matrici
- `A(1,3)`: stampa nella Command Window il valore individuato dalla prima riga e terza colonna di A.
- 
