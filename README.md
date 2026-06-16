# ai-ghostwriter-dante
rogetto RNN/LSTM per generazione testo in stile Divina Commedia
# AI Ghostwriter - Dante

Progetto realizzato per il modulo di Machine Learning sulle reti ricorrenti.

## Descrizione

L'obiettivo del progetto era modificare un generatore di testo inizialmente addestrato sul dataset Tiny Shakespeare per farlo lavorare sulla Divina Commedia di Dante Alighieri.

Il modello è stato addestrato a livello di carattere e utilizzato per generare nuovi testi ispirati allo stile dantesco.

## Modifiche effettuate

* Sostituito il dataset Shakespeare con il testo della Divina Commedia.
* Download del testo tramite la libreria requests.
* Gestione della codifica UTF-8 per gli accenti italiani.
* Creazione del nuovo vocabolario dei caratteri.
* Riduzione della lunghezza delle sequenze da 250 a 80 caratteri.
* Addestramento del modello sul nuovo dataset.
* Test della generazione con diverse temperature.

## Risultati

Numero di caratteri unici:

* Shakespeare: 65
* Dante: 69

Sono stati effettuati test con tre valori di temperatura:

* 0.2 → testo più stabile ma ripetitivo
* 1.0 → miglior equilibrio tra coerenza e creatività
* 2.0 → testo molto più casuale e spesso poco comprensibile

## Conclusioni

La temperatura 1.0 ha prodotto i risultati migliori.

Il modello è riuscito a generare testi che ricordano in parte la struttura e il linguaggio del corpus utilizzato, pur mantenendo alcuni errori e parole inventate tipici dei modelli di generazione a livello di carattere.

## Strumenti utilizzati

* Python
* TensorFlow / Keras
* GRU
* NumPy
* Requests
* Jupyter Notebook
* GitHub
