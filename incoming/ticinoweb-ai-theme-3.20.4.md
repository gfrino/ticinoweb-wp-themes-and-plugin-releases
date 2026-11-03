- **WooCommerce 11.2**: i tab delle Impostazioni (Generale, Prodotti, Spedizione, Pagamenti, ...) tornano visibili.
  - Motivo: il tema dava `top: 44px` all'intestazione di WooCommerce pensandola fissa; da WooCommerce 11.2 è `position: relative`, quindi scendeva di 44px e copriva la riga dei tab.

