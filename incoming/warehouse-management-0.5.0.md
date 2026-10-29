
### Added
- Aggiornamenti dal repo pubblico delle release ticinoWEB (Update URI, `includes/tw-release-updater.php`, installazione del mu-plugin «ticinoWEB Release Updater»), icona e scheda «Dettagli versione».
- La gestione dei lotti scalati dagli ordini è ora nel plugin (`inc/order-lots.php`): prima stava nel tema lagalpi-child (ex Code Snippets #7). Riquadro dell'ordine «Lotti scalati» con tabella di WordPress e testi in italiano.
- Traduzioni: text domain unico `warehouse-management`, file `languages/warehouse-management.pot`.

### Fixed
- **Prodotti semplici scalati due volte**: sulla stessa transizione «In lavorazione» giravano due riduzioni dei lotti (l'hook `whm_reduce_stock_on_order_processing` del plugin e quello del tema). Ora ce n'è una sola, e un ordine che torna più volte «In lavorazione» viene scalato una volta sola (meta `_whm_lots_reduced_*`).
- Il ramo delle variazioni di `whm_reduce_stock_on_order_processing` non faceva nulla (variabile sbagliata): rimosso insieme all'hook, le variazioni restano gestite da `inc/order-lots.php`.
- Pulsante «Aggiungi lotto» delle variazioni: usava `$`, che nel backend non è definito, e un `alert()`. Ora usa jQuery e al quinto lotto il pulsante sparisce.
- Avvisi PHP per parametri mancanti nell'elenco prodotti e ordini.
- Menu dei mesi nel filtro «più/meno venduti»: il mese scelto restava selezionato solo in inglese.

### Changed
- **Report Excel su richiesta**: prima veniva rigenerato a ogni apertura dell'elenco prodotti filtrato (una query su tutti i prodotti più la scrittura del file). Ora l'elenco ricorda solo il filtro; il file si crea al clic su «Scarica Excel», per utente, e si cancella dopo il download.
- Elenco prodotti del filtro ordini caricato con una query più leggera.
- Testi del backend in italiano: filtri magazzino, colonne «Ordini» ed «Esporta», sezione «Lotti di magazzino», email dei lotti in scadenza.
- Libreria PhpSpreadsheet aggiornata (vedi `lib/composer.json`) e verificata con `composer audit`.

### Removed
- `readme.txt` e `templates/`, avanzi del plugin «Blank» da cui era partito lo sviluppo, non usati.

