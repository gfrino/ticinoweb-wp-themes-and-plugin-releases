
- **Esportazione automatica su ImmoGalaxy** (Immobili → Immogalaxy): ogni notte, tra le 00:01 e le 01:29, un file XML `AAAAMMGG.<gestionale>.xml` con gli immobili nuovi o modificati (UPDATE) e quelli tolti dalla vendita o archiviati (DELETE); il sabato, se attivo, invio completo di tutti gli immobili. Invio via FTP (anche FTPS), resoconto per email dopo ogni invio, registro degli ultimi invii, pulsanti per scaricare l'XML di prova (completo o solo novità) e per inviare subito. Spento finché non lo si attiva e non si inseriscono codice agenzia, gestionale e accessi.
- Nuovi campi nell'immobile: NAP, Cantone e «Pubblica su ImmoGalaxy» (Sì/No). Gli immobili senza NAP, località, categoria riconosciuta o almeno una foto non partono e compaiono nell'elenco «da completare».
- Codice stabile verso ImmoGalaxy per ogni immobile (`_idea_export_id`): per gli immobili del vecchio sito è lo stesso codice usato allora, così non nascono doppioni; per i nuovi si assegna in automatico.

