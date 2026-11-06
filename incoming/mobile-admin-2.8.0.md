### Added
- **Pagina Gestione App → Chiavi API app** (solo sul sito principale del brand, come Metodi di Pagamento): una riga per sede con stato (✅ Attiva con ultimo uso, ⚠️ Mancante, ❌ Cancellata in WooCommerce), pulsanti «Genera chiave» / «Rigenera» e «Genera tutte le chiavi mancanti». La chiave WooCommerce in lettura/scrittura viene creata direttamente nella tabella della sede: nessuno deve più copiare chiavi a mano.
- Avviso rosso in bacheca sul sito principale finché una sede è senza chiave funzionante (da lì l'app non può ricevere ordini).
- Endpoint `GET /wp-json/mobile-admin/v1/app-keys` per le Cloud Functions, protetto dall'header `X-App-Keys-Secret` (segreto in `wp-config.php` come `ARD_APP_KEYS_SECRET` o generato automaticamente nell'opzione di rete `ard_app_keys_secret`, visibile nella pagina con «Mostra» / «Copia»). Risposta mai in cache (LiteSpeed/CDN).

### Why
- Il 6 novembre 2026 le chiavi WooCommerce delle sedi Little Inka, salvate in due campi ACF del sito principale e servite in chiaro-cifrato da un endpoint pubblico, sono state cestinate «perché inutilizzate»: tutti gli ordini dall'app sono falliti per una giornata. Con questa versione le chiavi non sono più modificabili per sbaglio da una schermata di modifica, lo stato è visibile e la rigenerazione è un clic.

