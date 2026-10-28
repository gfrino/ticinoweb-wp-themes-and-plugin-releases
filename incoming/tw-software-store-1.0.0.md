### Added
- Ogni plugin WordPress pubblicato nel repo delle release diventa un prodotto WooCommerce (virtuale, scaricabile, venduto singolarmente, licenza perpetua, prezzo predefinito 199 CHF) e si aggiorna a ogni nuova versione: file, versione, novità, immagini. Perché: oggi chi vuole un nostro plugin deve chiedercelo; il negozio deve restare allineato alle release senza lavoro a mano.
- I temi sono riconosciuti dallo zip e ignorati; i plugin su misura si escludono per slug o con `"shop": false` in details.json.
- Prezzo, testi e immagini scelti a mano non vengono mai sovrascritti (`wp tw-store link <slug> <id>` collega un prodotto esistente).
- Pagina WooCommerce → Software Store, comandi `wp tw-store sync|list|link`, controllo orario e ping firmato per l'aggiornamento immediato dal workflow GitHub.
