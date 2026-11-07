### Added
- **Rimborsi Datatrans dalla pagina dell'ordine WooCommerce.** Per gli ordini pagati nell'app (TWINT, carta, Apple Pay, Google Pay) il pannello «Rimborsa» di WooCommerce mostra il pulsante «Rimborsa X CHF tramite Datatrans»: l'importo si sceglie come sempre dagli articoli, il rimborso parte su Datatrans attraverso le Cloud Functions dell'app (le credenziali Datatrans non sono nel sito) e WooCommerce lo registra con una nota. Gli ordini delle versioni precedenti dell'app vanno ancora rimborsati dal Webadmin, e la pagina lo dice.
- **Riconciliazione oraria degli storni fatti nel Webadmin Datatrans**: Datatrans non avvisa il sito quando uno storno viene fatto da lì, quindi ogni ora ogni sede controlla gli ordini Datatrans degli ultimi 30 giorni e registra in WooCommerce (con nota «Stornato da Datatrans (Webadmin)») gli importi stornati che mancano.
- Campo «Indirizzo delle Cloud Functions» in Gestione App → Chiavi API app (sito principale), usato dai rimborsi e dalla riconciliazione.

### Why
- Finora i rimborsi dell'app si facevano solo nel Webadmin Datatrans e WooCommerce non ne sapeva nulla: contabilità e stato ordine restavano sbagliati.

