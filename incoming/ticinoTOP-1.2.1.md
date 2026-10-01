
### Correzioni
- Scanner AI: "Pubblica in Aziende" rispondeva "Risultato della scansione scaduto" subito dopo l'anteprima. Il risultato era salvato in un transient, che con un object cache esterno vive solo in cache e può sparire tra due richieste. Ora è salvato nel database (user meta dell'utente), resta disponibile 24 ore e viene eliminato dopo la pubblicazione.

