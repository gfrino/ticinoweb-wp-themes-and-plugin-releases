### Added
- Prima versione. Quattro metodi di pagamento WooCommerce su un solo account Datatrans: **TWINT**, **Carta di credito o debito** (circuiti a scelta), **Apple Pay** (solo Safari) e **Google Pay**, ognuno attivabile e rinominabile da WooCommerce → Impostazioni → Pagamenti. Funziona con il checkout classico e con quello a blocchi.
- Pagina **WooCommerce → Datatrans**: modalità Live o Test (sandbox) con credenziali separate, chiave di firma del webhook (HMAC‑SHA256), addebito immediato, log dettagliato, pulsante «Verifica le credenziali», stato dei metodi e indirizzo del webhook.
- Pagamento sulla pagina sicura di Datatrans (Redirect, API v2): l'ordine viene segnato pagato solo dopo una verifica dello stato sull'API Datatrans, sia all'arrivo del webhook sia al ritorno del cliente. Annullamento e errore riportano al pagamento dell'ordine con un messaggio chiaro, senza addebiti.
- **Rimborsi dalla pagina dell'ordine**, totali o parziali, con controllo preventivo dell'importo ancora rimborsabile su Datatrans.
- Riquadro Datatrans nella pagina dell'ordine (transazione, metodo, carta mascherata, ambiente di test).
- Testi in inglese con traduzione italiana; nomi e testi personalizzati dei metodi registrati per WPML e tW Translate Plus.

### Why
- Little Inka accetta già TWINT, carte, Apple Pay e Google Pay nell'app tramite Datatrans: il sito web deve offrire gli stessi metodi con lo stesso contratto, senza un secondo fornitore di pagamenti.
