
- Software store: ogni plugin WordPress pubblicato nel repo delle release diventa da solo un prodotto WooCommerce (virtuale, scaricabile, venduto singolarmente, licenza perpetua, prezzo predefinito 199 CHF) e si aggiorna a ogni nuova versione (file, versione, novità, immagini). I temi sono ignorati; prezzo e testi scelti a mano non vengono mai sovrascritti. Perché: il negozio deve restare allineato alle release senza lavoro a mano. Impostazioni in WooCommerce → Software Store, comandi `wp tw-store sync|list|link`. Codice in `inc/software-store/` (nessun plugin).
- Nuovo template «ticinoWEB — Wordpress Software» (`page-wordpress-software.php`): catalogo dei plugin in vendita.

