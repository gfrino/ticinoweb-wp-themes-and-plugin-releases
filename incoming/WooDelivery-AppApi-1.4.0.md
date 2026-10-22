### Added
- **Foto e orario dei punti di ritiro**, mostrati nell'app. I due campi compaiono nella pagina *Pickup Location* di CodeRockz, sotto i campi esistenti, con anteprima dal vivo di come appariranno nell'app, e si salvano con lo stesso pulsante *Save Changes* (nessuna pagina separata).
- L'endpoint `/wp-json/getPickupLocations/allLocations` restituisce `time_slot`, `image_id` e `image_url` per ogni punto.
- Se un punto viene rinominato, foto e orario lo seguono; se viene eliminato, i suoi dati extra vengono rimossi.
- Aggiornamenti automatici dal repo delle release ticinoWEB (header `Update URI`, `includes/tw-release-updater.php`), icona e scheda «Dettagli versione».
- Traduzioni IT/EN (`languages/`).

### Security
- Salvataggio solo con nonce di CodeRockz e permesso `manage_woocommerce` / `manage_options`; l'immagine deve essere un allegato di tipo immagine.

