Milestone 1
Replica della grafica con la possibilità di avere messaggi scritti dall’utente (verdi) e dall’interlocutore (bianco) assegnando due classi CSS diverse
Visualizzazione dinamica della lista contatti: tramite la direttiva v-for, visualizzare nome e immagine di ogni contatto
Milestone 2
Visualizzazione dinamica dei messaggi: tramite la direttiva v-for, visualizzare tutti i messaggi relativi al contatto attivo all’interno del pannello della conversazione
Click sul contatto mostra la conversazione del contatto cliccato


Milestone 3
Aggiunta di un messaggio: l’utente scrive un testo nella parte bassa e digitando “enter” il testo viene aggiunto al thread sopra, come messaggio verde
Risposta dall’interlocutore: ad ogni inserimento di un messaggio, l’utente riceverà un “ok” come risposta, che apparirà dopo 1 secondo.
Milestone 4
Ricerca utenti: scrivendo qualcosa nell’input a sinistra, vengono visualizzati solo i contatti il cui nome contiene le lettere inserite (es, Marco, Matteo Martina -> Scrivo “mar” rimangono solo Marco e Martina)
Milestone 5 - opzionale
Cancella messaggio: cliccando sul messaggio appare un menu a tendina che permette di cancellare il messaggio selezionato

Visualizzazione ora e ultimo messaggio inviato/ricevuto nella lista dei contatti 

Consigli utili:
Si possono trascurare le scrollbar verticali, sia nel pannello dei messaggi, che nella lista dei contatti
I pulsanti e le icone possono non funzionare (a parte l’invio del messaggio)
Per gestire le date, può essere utile la libreria Luxon
La struttura dell’array dei contatti potrebbe avere questa forma:



SCOMPOSIZIONE

Milestone1:
Creo una sezione in absolute per l'app.
Divido l'app in due contenuti tra la lista chat e la chat aperta.
Imposto il CSS per ogni parte e per le signole conversazioni.
Creo un v-for per mostrare ogni contatto


Milestone2:
Creo un v-for per mostrare i messaggi nella chat
Creo una funzione per mostrare la chat del contatto selezionato

Milestone3:
Creo una funzione che si attiva quando l'utente preme invio nell'input di testo.
La funzione Crea una nuova variabile con le propretà uguali a quelle esistenti che avrò come testo il contenuto dell'input.
Pusho la variabile nell'array dei messaggi del singolo contatto.
Imposto un timeout che si attiva subito dopo, facendo la stessa cosa del messaggio inviato ma con stato del messaggio diverso.

Mileston4:
Creo una funzione che tramite un indexOf di tutti i contatti confronta l'input nella barra di ricerca.
Se index è maggiore di 0 (ovvero se è presente ) il v-show lo mostra, in caso contrario lo nasconde.

Milestone5:
Creo una funzione che al click elimina il messaggio selezionato.
Aggiungo il menù a tendina nei messaggi da mostrare solo al click 