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
- Una **variabile** è definibile come una sequenza di lettere e numeri (e il carattere underscore). Deve iniziare con una lettera (minuscola) e se possibile avere un nome esplicativo.
- Un **vettore** dovrebbe avere come nome una singola lettera minuscola (se possibile), oppure utilizzare un nome più lungo ma esplicativo; possiamo distinguere se si tratta di riga o colonna utilizzando `_r` e `_c` come suffissi.
- Una **matrice** dovrebbe avere come nome una singola lettera maiuscola.
## Oggetti di Lavoro
**ATTENZIONE**: come detto in precedenza, tutti gli oggetti di lavoro utilizzati da MatLab sono interpretati come matrici *m × n*, ed ogni valore che compone la matrice è definito su 8 byte. 

Si può capire facilmente che l'obiettivo del linguaggio sia la precisione, a discapito dell'ottimizzazione.
- **Variabili**: una variabile si definisce assegnando un valore reale ad un nome scelto per la variabile. Così facendo, la variabile appena creata verrà salvata automaticamente nel workspace.
  - `a=15`
- **Vettori**: un vettore riga è dichiarato attraverso le parentesi quadrate, che racchiudono i valori che lo compongono separati da uno spazio (o una virgola). È possibile definire un vettore attraverso la dicitura *inizio - passo - fine*, o anche *inizio - fine* se il passo è unitario.
Per creare un vettore colonna, infine, dovremmo utilizzare i punti e virgola al posto degli spazi.
  - `row=[1 2 3]` oppure `row=[1, 2, 3]`
  - `column=[1; 2; 3]`
- **Matrici**: le matrici possono essere dichiarati come un vettore colonna di vettori riga oppure cadenzando le colonne con i punto e virgola e le righe con spazio (o virgola).
  -  `matrix=[[1 2 3]; [4 5 6]; [7 8 9]]` oppure `matrix=[1 2 3; 4 5 6; 7 8 9]`
