# Progetti-Python

Svolgimento di progetti di programmazione classica tramite il linguaggio di programmazzione Python.
Di seguito le specifiche dei progetti. Il primo ed il terzo progetto sono stati commentati, mentre per il secondo è presente solo il codice.

# Progetto 1°

Il dataset formula1_data.csv contiene i risultati del mondiale di Formula 1 della Stagione 2008.

Esso contiene 180 righe e le seguenti 5 colonne:

Driver: Nome del Pilota  
Team: Costruttore per il quale il pilota gareggia  
Race: Città dove si è svolto il Gran Premio  
Country: Paese dove si è svolto il Gran Premio  
Position: Numero compreso tra 0 e 8 che rappresentano l’ordine di arrivo del pilota nella singola gara (0 significa che il pilota non è arrivato tra i primi 8).  
Al termine di un gran premio, vengono assegnati i punti ai piloti in base all’ordine di arrivo: 10 al vincitore, 8 al secondo, 6 al terzo, e poi a scalare di 1 punto fino all’ottavo.


Implementa un insieme di funzioni per analizzare i risultati del Campionato Mondiale di Formula 1 utilizzando i dati nel file csv a tua disposizione

In particolare dovrai implementare le seguenti funzioni:

Una funzione che riceve in input il nome di un pilota e restituisce una lista contenente il totale dei punti del pilota, il numero di vittorie (quante volte il pilota è arrivato primo) e il numero dei podi (quante volte il pilota è salito sul podio).  
Una funzione che non riceve alcun parametro in ingresso e deve restituire un dizionario formato da coppie chiave valore, dove la chiave è una stringa che contiene il nome del pilota, mentre il valore associato alla chiave è un intero che rappresenta il totale dei punti che il pilota ha conseguito alla fine del campionato mondiale.
Salva poi la classifica in un file di testo di tipo txt con il seguente formato:

Drivers Standings 2008 Formula 1  
NomePilota1: PunteggioTotale  
NomePilota2: PunteggioTotale…  
Una funzione che non riceve alcun parametro in ingresso e deve restituire un dizionario formato da coppie chiave valore, dove la chiave è una stringa che contiene il nome del costruttore, mentre il valore associato alla chiave è un intero che rappresenta il totale dei punti che il costruttore ha conseguito alla fine del campionato mondiale.  
I punti conseguiti da un costruttore sono la somma dei punti che i piloti che corrono per il costruttore hanno conseguito durante l’anno.Per fare ciò, utilizza i dati salvati sul file creato precedentemente



# Progetto 2°

Questo progetto consiste nel realizzare un software per la gestione di un negozio di prodotti 
vegani. Il software deve avere le seguenti funzionalità:

• Registrare nuovi prodotti, con nome, quantità, prezzo di vendita e prezzo di acquisto.  
• Elencare tutti i prodotti presenti.  
• Registrare le vendite effettuate.  
• Mostrare i profitti lordi e netti.  
• Mostrare un menu di aiuto con tutti i comandi disponibili.

Il software è testuale, quindi utilizzabile da riga di comando.

NOTE

• Cerca di scrivere del buon codice organizzandolo le varie funzionalità in apposite 
funzioni.  
• Prima di scrivere il codice, pensa a quali sono le migliori strutture dati da utilizzare: liste, 
tuple, dizionari, o combinazioni di esse come liste di dizionari.  
• Il programma deve essere persistente, cioè le informazioni inserite dall'utente devono 
essere mantenute tra diverse esecuzioni del programma, per fare questo puoi utilizzare 
un file di testo scegliendo tu che tipo di codifica utilizzare per le informazioni.  
• Assicurati che gli input inseriti dall'utente siano validi, ad esempio che i numeri siano 
effettivamente numeri, gestisci i casi non validi con eccezioni e messagi di errore.  
• Durante un acquisto, verifica che i prodotti acquistati siano effettivamente presenti nel 
magazzino, nel caso negativo mostra all'utente un messaggio di errore.  
• Durante l'aggiunta in magazzino, verifica se il prodotto da aggiungere è già presente 
magazzino, nel caso positivo aggiungi la quantità a quella già presente in magazzino, in 
questo caso non serve specificare di nuovo il prezzo di acquisto e di vendita, altrimenti 
registralo come un nuovo prodotto.  
• Il profitto lordo è il totale delle vendite, cioè tutto ciò che i clienti hanno pagato, il profitto
netto invece è pari al profitto lordo meno il costo di acquisto per i prodotti.

ESEMPIO DI INTERAZIONE CON IL PROGRAMMA

Inserisci un comando:  
• aiuto:  
I comandi disponibili sono i seguenti:  
• aggiungi: aggiungi un prodotto al magazzino  
• elenca: elenca i prodotto in magazzino  
• vendita: registra una vendita effettuata  
• profitti: mostra i profitti totali  
• aiuto: mostra i possibili comandi  
• chiudi: esci dal programma  

Inserisci un comando:  
aggiungi  
Nome del prodotto: latte di soia  
Quantità: 20  
Prezzo di acquisto: 0.80  
Prezzo di vendita: 1.40  
AGGIUNTO: 20 X latte di soia

Inserisci un comando:  
aggiungi  
Nome del prodotto: **tofu* *  
Quantità: 10  
Prezzo di acquisto: 2.20  
Prezzo di vendita: 4.19  
AGGIUNTO: 10 X tofu  

Inserisci un comando: 
aggiungi  
Nome del prodotto: seitan  
Quantità: 5  
Prezzo di acquisto: 3  
Prezzo di vendita: 5.49  
AGGIUNTO: 5 X seitan  

Inserisci un comando:  
elenca  
PRODOTTO QUANTITA' PREZZO  
latte di soia 20 €1.4  
tofu 10 €4.19  
seitan 5 €5.49  

Inserisci un comando:  
vendita  
Nome del prodotto: latte di soia  
Quantità: 5  

Aggiungere un altro prodotto ? (si/no): si  
Nome del prodotto: tofu  
Quantità: 2  

Aggiungere un altro prodotto? (si/no): no  
VENDITA REGISTRATA  
• 5 X latte di soia: €1.40  
• 2 X tofu: €4.19  
Totale: €15.38  

Inserisci un comando:  
elenca  
PRODOTTO QUANTITA' PREZZO  
latte di soia 15 €1.4  
tofu 8 €4.19  
seitan 5 €5.49  

Inserisci un comando:  
vendita  
Nome del prodotto: seitan  
Quantità: 5  

Aggiungere un altro prodotto ? (si/no): no  
VENDITA REGISTRATA  
• 5 X seitan: €5.49  
Totale: €27.45  

Inserisci un comando:  
elenca  
PRODOTTO QUANTITA' PREZZO  
latte di soia 15 €1.4 tofu 8 €4.19  

Inserisci un comando: profitti  
Profitto: lordo=€42.83 netto=€19.43  

Inserisci un comando: storna  
Comando non valido I comandi disponibili sono i seguenti:  
• aggiungi: aggiungi un prodotto al magazzino  
• elenca: elenca i prodotto in magazzino  
• vendita: registra una vendita effettuata  
• profitti: mostra i profitti totali  
• aiuto: mostra i possibili comandi  
• chiudi: esci dal programma  

Inserisci un comando: chiudi Bye bye

# Progetto 3°

La neonata IASS (International Alliance for Safe Skies) ti ha incaricato di svolgere un'accurata analisi di tutti gli incidenti aerei che si sono verificati dal 1919 al 2023.
A tale scopo ti mette a disposizione un set di dati in cui sono registrati quasi 25.000  incidenti con le seguenti informazioni

date: data dell'incidente  
type: tipo del velivolo  
registration: codice di registrazione del velivolo  
operator: operatore del velivolo  
fatalities: numero di morti  
location: luogo dell'incidente  
country: nazione dell'incidente  
cat: categoria dell'incidente come descritto dal ASN

Utilizza i dati per portare alla luce, anche tramite grafici e visualizzazioni, utili insight.

ESEMPI DI INSIGHT  
Questi sono esempi di domande alla quale puoi trovare risposta tramite i dati, non limitarti a queste ma svolgi un’analisi approfondita ponendoti ulteriori domande che pensi possano fornire insight utili  
In quale nazione si sono verificati più incidenti?  
Gli incidenti avvengono più di frequente durante determinati giorni della settimana?  
Quali sono gli operatori più sicuri?  
Quale tipo di velivolo ha causato più morti?  
Come si sono evoluti gli incidenti dopo l'11 Settembre?  
