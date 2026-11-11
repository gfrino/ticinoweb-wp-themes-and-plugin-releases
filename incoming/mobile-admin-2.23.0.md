### Added
- REST `GET /wp-json/mobile/v1/products/id_translator` (ID dei prodotti nella lingua scelta), letto dalle Cloud Functions dell'app per i prodotti preferiti in inglese, tedesco e francese. Prima stava nello snippet «Mobile - Products Custom Endpoints» di Code Snippets su ogni sede: ora è nel plugin con gli stessi parametri e la stessa risposta. Con WPML usa le sue traduzioni; con tW Translate Plus (o senza plugin di traduzione) un prodotto ha lo stesso ID in tutte le lingue. Lo snippet si può togliere.

### Removed
- La rotta `mobile/v1/products/search` dello stesso snippet non è stata portata: nessuno la usa (né l'app né le Cloud Functions) e rispondeva con un errore 500 da quando WPML è spento.

