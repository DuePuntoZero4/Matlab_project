# Blocchi condizionali

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
- `load <nome_fi
