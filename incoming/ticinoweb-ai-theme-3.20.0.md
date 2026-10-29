- **Contatti: seconda sede, dati fiscali e mappa**: nuovi campi in ticinoWEB CMS → Contatti (etichetta dell'indirizzo, seconda sede con etichetta, dati fiscali, link alla mappa), esposti da `ticinoweb_get_contact_info()` insieme a `phone_display`. Tutti facoltativi: i siti che non li compilano non cambiano.
- **Form**: nuovi filtri `ticinoweb_form_errors` (controlli extra del child, es. consenso privacy) e `ticinoweb_form_success_message` (testo di conferma del child).
- **Servizi**: un child che gestisce i servizi con un proprio tipo di contenuto può fornirli con il filtro `ticinoweb_services_external` (usato da `ticinoweb_get_services()` e dagli shortcode) e segnalarlo con `ticinoweb_services_managed_notice`: la tab «Servizi Principali» mostra il rimando invece dell'elenco vuoto.
  - Motivo: il child capoferrisagl duplicava modulo, contatti e servizi del parent; ora li usa e li estende.

