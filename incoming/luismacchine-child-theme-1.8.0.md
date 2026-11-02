
- Aggiunto nella lista “Tutti i Veicoli” il comando amministrativo “Sincronizza con tutti.ch”, protetto da permessi e nonce e con risultato mostrato nella stessa schermata.
- Collegato il motore di sincronizzazione già predisposto alle pagine pubbliche del profilo Luismacchine e dei relativi annunci, senza autenticazione né accesso a endpoint privati.
- Importati soltanto inventari completi: ID, categoria, titolo, descrizione, prezzo, dati tecnici e immagini; in caso di risposta incompleta o formato cambiato non viene modificato alcun prodotto.
- Mantenute classificazione Veicoli/Ricambi, deduplicazione, riconciliazione con i prodotti esistenti, copia locale delle immagini e protezione dalla rimozione accidentale.
- Aggiunta una cache settimanale per le schede invariate, così i controlli successivi richiedono una sola lettura del profilo e scaricano nuovamente solo gli annunci cambiati.

