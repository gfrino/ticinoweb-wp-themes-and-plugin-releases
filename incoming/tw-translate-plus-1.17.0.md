- **feat(migrazione)**: import da WPML (scheda «Migrazione WPML» e `wp twtr wpml-import`): contenuti, prodotti e varianti, modelli Elementor, voci di menu, categorie e attributi, media, stringhe; nessuna traduzione rifatta dal motore (`origin=wpml`, bloccate). Resoconto con le note da controllare, import ripetibile e annullabile.
- **feat(url)**: indirizzi tradotti per lingua (`Twtr_Slugs`, mappa per segmento: pagine anche annidate, prodotti, base prodotto, categorie) senza rewrite rule; 301 dallo slug originale a quello tradotto; redirect 301 per vecchi indirizzi senza pagina (solo su 404).
- **feat(elementor)**: i link interni delle pagine (Elementor, editor) puntano alla lingua corrente (selettori lingua esclusi); il contenuto grezzo delle pagine costruite con Elementor non viene più messo in coda (lo traduce il livello pagina: niente costi inutili).
- **feat(ajax)**: le richieste AJAX (moduli, carrello, risposte di plugin) partite da una pagina tradotta usano la lingua di quella pagina (Referer dello stesso sito).
- **feat(wpml)**: finché WPML è attivo tW Translate resta in attesa sul sito pubblico (avviso in admin con il link alla migrazione).


