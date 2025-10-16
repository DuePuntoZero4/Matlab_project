# MatLab_project
## Introduzione a MatLab
Il nome *MatLab* è un abbreviazione per la dicitura "MATrix LABoratory"; il software è pensato per calcoli matriciali e vettoriali di elevata complessità, anche con numeri definiti in floating point a doppia precisione.
Ogni cosa in MatLab è rappresentata come una matrice, anche una variabile singola, ed ogni valore occupa 8 byte.
## Aree di lavoro
La finestra di lavoro offerta da MatLab è suddivisa in 4 aree principali:
- **Command Window**: assomiglia alla finestra di un terminale, dove potremo scrivere comandi diretti.
- **Workspace**: in quest'area il calcolatore mostra il nome e il valore di tutte le variabili salvate in memoria.
- **Folder**: è un'area di navigazione, che mostra la nostra cartella corrente e i file in essa contenuti.
- **Script Editor**: è un'area dove possiamo scrivere codice, eseguibile poi da MatLab. Gli script vengono salvati con estensione *.m*.
## Linee guida sintattiche
- Una **variabile** è definibile come una sequenza di lettere e numeri (e il carattere underscore). Deve iniziare con una lettera e se possibile avere un nome esplicativo.
## Oggetti di Lavoro
**ATTENZIONE**: come detto in precedenza, tutti gli oggetti di lavoro utilizzati da MatLab sono interpretati come matrici *m × n*, ed ogni valore che compone la matrice è definito su 8 byte. Si può capire facilmente che l'obiettivo del linguaggio sia la precisione, a discapito dell'ottimizzazione.
- **Variabili**: una variabile si definisce assegnando un valore reale ad un nome scelto per la variabile. Così facendo, la variabile appena creata verrà salvata automaticamente nel workspace.
  - `a=15`
- **Vettori**: un vettore riga è dichiarato attraverso le parentesi quadrate, che racchiudono i valori che lo compongono separati da uno spazio (o una virgola). È possibile definire un vettore attraverso la dicitura *inizio - passo - fine*, o anche *inizio - fine* se il passo è unitario.
Per creare un vettore colonna, infine, dovremmo utilizzare i punti e virgola al posto degli spazi.
  - `row=[1 2 3]` oppure `row=[1, 2, 3]`
  - `column=[1; 2; 3]`
- **Matrici**: % continua qui
## Comandi
Questo file presenta un elenco dei comandi che abbiamo visto / vedremo a lezione.
### Comandi ereditati da Shell (bash)
- `pwd` → *Print Working Directory*: stampa in output (nella Command Window) la cartella di lavoro corrente come una stringa.
- `ls` → *List Directory Contents*: elenca (sempre nella Command Window) i file e le sottocartelle della directory corrente; se viene aggiunto un percorso di una cartella come argomento, elenca i contenuti di quella cartella.
- `mkdir` → *Make Directory*: crea una nuova cartella all'interno della cartella corrente, con nome la stringa specificata nell'argomento.
- `cd` → *Change Directory*: questo comando può essere utilizzato in due modi:
  - senza argomento, ritorni alla cartella madre.
  - con argomento, entri in una sottocartella della cartella corrente.
- `delete`: cancella il file specificato dall'argomento.
### Comandi base
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
### Operazioni ed operatori
In generale, MatLab è una calcolatrice scientifica sotto steroidi; di conseguenza, valgono le normali regole di calcolo usati da altri linguaggi di programmazione.
Un'operazione in matlab può essere definita con `;` finale o senza. Nel primo caso, il risultato non verrà mostrato nella Command Window, mentre nel secondo comparirà associato alla variabile predefinita *ans*.
Le operazioni di base di MatLab sono 6:
- addizione `+`
- sottrazione `-`
- moltiplicazione `*`
- divisione `/`
- potenza `^`
- assegnazione `=`
