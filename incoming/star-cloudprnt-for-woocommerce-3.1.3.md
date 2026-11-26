
### Fixed
- **Ordini dei partner sullo scontrino.** Un ordine da consegnare a un partner (ufficio, scuola…) usciva come «<< Ritiro in sede» se fatto dal sito (il checkout lo registra come ritiro in un «punto di ritiro», con la data di ritiro) e con il solo titolo della spedizione se fatto dall'app Little Inka; il nome del partner non compariva mai. Ora stampa «>> Consegna al partner» con il nome del partner sotto (meta `pickup_location` del checkout o `stud_office_address` dell'app) e non stampa più il QR verso l'indirizzo di casa del cliente.

