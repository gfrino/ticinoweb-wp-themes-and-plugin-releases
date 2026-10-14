
- pannello ticinoWEB CMS → Servizi: Titolo, Descrizione e Immagine Servizio tornano modificabili; al salvataggio vengono scritti nella pagina del servizio (Titolo, Riassunto, Immagine in evidenza), che resta l’unica sorgente;
- ogni servizio nel CMS ha il campo “Immagini aggiuntive (carosello)” con Libreria media, riordino e rimozione, sincronizzato con lo stesso campo dell’editor della pagina;
- sincronizzazione protetta da capability `edit_post` e limitata alle pagine servizio;
- test aggiornati (`test-services-page-sync.php`, `test-services-page-sync-admin.js`).

