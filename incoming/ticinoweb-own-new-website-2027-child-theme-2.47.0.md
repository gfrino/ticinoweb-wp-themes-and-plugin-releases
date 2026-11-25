
- Software store, **licenze dei plugin venduti**: a ordine completato il sito chiede a Odoo (GestaClient su ticinoweb.online,
  menu Plugin WordPress) la chiave di licenza di ogni plugin dell'ordine. La chiave compare nell'email «Ordine completato»,
  nel dettaglio dell'ordine in Il mio account e nell'ordine in bacheca. Se Odoo non risponde il pagamento non si blocca:
  nuovi tentativi automatici per due giorni e, quando la chiave arriva, il cliente la riceve per email con una nota
  dell'ordine. Rimborso o annullamento dell'ordine: le licenze vengono spente in Odoo.
- WooCommerce → Software Store: nuova sezione «Licenze» con lo stato del collegamento, il campo per il segreto condiviso
  con Odoo (oppure la costante `TWSS_LICENSE_SECRET` in wp-config) e il pulsante «Prova il collegamento».
  WP-CLI: `wp tw-store license <ordine>` (chiavi mancanti di un ordine, mandate al cliente) e `wp tw-store license-test`.
- Scheda dei plugin: «Licenza perpetua per un sito: si paga una volta sola, nessun canone annuale. Per i siti ospitati
  da ticinoWEB il plugin è già incluso.» Perché: i siti sui nostri server usano i plugin senza licenza.

