### Added
- **Gestione App → Menù combinati** (solo sito principale del brand): pagina per le due nuove pagine dell'app. «Crea Menù» propone, quando nel carrello c'è una poké senza bibite né dessert, le offerte Pokè + Acqua, Pokè + Dessert e Pokè + Acqua + Dessert con il supplemento impostato qui (ognuna si può spegnere); «Aggiungi una bibita» compare se il cliente salta il menù. Acque, dessert e bibite si scelgono per nome da un elenco con foto e ricerca, valgono per tutte le sedi e ogni sede mostra solo quelli che vende e ha disponibili. Anteprima dal vivo di come appare nell'app.
- REST `GET mobile-admin/v1/combo-menu?site=<sede>`: configurazione con i prodotti della sede (id, prezzo, foto) e le categorie che servono all'app per riconoscere poké, bibite e dessert nel carrello.

### Why
- Little Inka vuole proporre il menù combinato in app prima del pagamento, con prezzi e prodotti gestibili senza aggiornare l'app.

