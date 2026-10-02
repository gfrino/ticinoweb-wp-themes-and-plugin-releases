### Fixed
- **Ordine e icone delle categorie nell'app non corrispondevano a mobile-admin** quando una categoria veniva rinominata in WooCommerce (es. "Pizze Classiche Normali" → "Pizze Normali", slug invariato). La riga in mobile-admin restava col nome vecchio, l'app (che abbina per nome) trovava invece una voce "traduzione automatica" nascosta con icona e posizione vecchie, e mostrava le pizze in fondo con l'icona a linea.
- Nuova `ARD_heal_renamed_category_icons()`: se il nome di una riga non esiste più ma il suo slug corrisponde a una categoria attuale, la riga passa al nome attuale mantenendo icona e posizione (sostituisce solo voci auto_i18n, mai righe reali). Applicata all'apertura della pagina Icone (salva e sincronizza con l'app se cambia qualcosa), nella sincronizzazione verso le Cloud Functions e nell'endpoint REST `/mobile-admin/v1/category-icons`.

### Added
- Ogni voce sincronizzata porta il `term_id` WooCommerce della categoria (per abbinare per ID nelle prossime versioni dell'app).
- Badge "⚠️ Categoria non trovata" sulle righe che non corrispondono a nessuna categoria con prodotti (nell'app non compaiono, si possono eliminare).

