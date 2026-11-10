
### Added
- Shortcode `[make_your_own_poke categoria="crea-la-tua-poke" per_pagina="4" orderby="price" ordine="ASC"]`: il configuratore funziona in qualsiasi tema, senza Elementor. Il markup sta in `brtw_render_configurator($args)` (`src/configurator.php`), usato anche dal widget.
- Pagina Impostazioni → «Make your own Pokè»: scelta per nome delle categorie «misura» e tabella dei gruppi di ingredienti con il numero di inclusi letto dalla descrizione, il prezzo dell'extra e la colonna «Forza a» per le eccezioni (es. TOPPING = 1, come faceva il codice in produzione). Opzione `brtw_settings` (`categorie`, `inclusi`).
- Funzioni per tema e plugin: `brtw_included_count($gruppo, $prodotto)` (secondo numero della descrizione, eccezioni dall'opzione, filtro `brtw_included_count`), `brtw_configurator_categories()` (filtro `brtw_configurator_categories`), `brtw_product_addon_groups($prodotto)`, `brtw_included_label()`, `brtw_render_configurator()`.
- Il cambio di misura non ricarica più la pagina: il render stampa i gruppi di add-on di ogni misura (un blocco `data-product` per prodotto) e lo script mostra quello scelto; le scelte già fatte passano alla nuova misura quando l'ingrediente esiste.
- Aggiunta al carrello con l'endpoint standard `wc-ajax=add_to_cart` di WooCommerce e i campi `addon-<prodotto>-<gruppo>` di Product Add-ons: frammenti del carrello aggiornati, avviso «Aggiunto al carrello» con link, oppure redirect se WooCommerce è impostato così. Senza JavaScript il modulo si invia al permalink del prodotto.
- Avviso in bacheca se WooCommerce o Product Add-ons mancano; header `Requires Plugins: woocommerce, woocommerce-product-addons`.

### Changed
- Prezzo lato server rifatto (`src/helper.php`): riconosce i prodotti del configuratore dalle categorie configurate (non più dagli slug WPML scritti nel codice); confronta i gruppi con il `field_name` che Product Add-ons salva nel carrello (`<id prodotto>-<id gruppo>`), non per posizione; sconta i primi N ingredienti di ogni gruppo nell'ordine in cui il cliente li ha scelti (anche con prezzo «per quantità»); ricalcola il prezzo da zero a ogni passaggio, quindi non si somma; non fa nulla se il carrello non ha prodotti del configuratore.
- Il modulo invia gli ingredienti nell'ordine di scelta e il plugin riordina `cart_item['addons']` di conseguenza (`woocommerce_add_cart_item_data`).
- Il widget Elementor si carica solo se Elementor è attivo (`did_action('elementor/loaded')`), chiama `brtw_render_configurator()` e regola i colori con le variabili `--brtw-*`; corretti `order_by` → `orderby` e `ase` → `ASC`; testi in italiano.
- JavaScript riscritto senza jQuery e senza `console.log`: totale a video con la stessa regola del server (inclusi gratis, poi extra), contatore «N di 2 incluse», limiti minimo e massimo del gruppo, validazione della Base obbligatoria prima dell'invio.
- CSS neutro e leggero: struttura, stati e variabili `--brtw-*` con default che il tema sovrascrive; tolti i colori imposti (#26a9ac, #CB6672…) e il riquadro fisso del totale; su telefono il riepilogo è sticky in basso.
- CSS e JS si accodano solo dove c'è lo shortcode, il widget o la funzione di render, con `BRTW_VERSION` (mai `time()`).

### Removed
- Endpoint `admin-ajax` `wc_brtw_product_addons_cart` (restituiva solo l'URL del carrello), `brtw_print`, `printbr`, `?print-dev`, `extract()` e i `print_r` nel render.
- File mai inclusi: `src/woocommerce/class-brtw-product-addons-cart.php`, il doppione `src/elementor/class.brtw.elementor.php`, la cartella `templates/addons/`.

### Security
- Tutto l'output del configuratore è escapato; l'input dello shortcode e delle impostazioni è sanitizzato; la pagina impostazioni usa Settings API con capability `manage_options`.

