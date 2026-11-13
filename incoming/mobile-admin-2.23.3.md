### Fixed
- Completata la protezione della 2.23.2 (risposte REST mai servite dalla cache di pagina) dopo una review del codice:
  - un indirizzo scritto con maiuscole diverse (per esempio `/wp-json/Mobile-Admin/v1/config`) arrivava comunque alla rotta, perché WordPress non distingue maiuscole e minuscole, ma non veniva riconosciuto come «del plugin» e poteva finire in cache: ora il confronto non dipende dalle maiuscole;
  - una regola «Force Cache URIs» di LiteSpeed Cache che comprende `/wp-json/` aveva la precedenza sul plugin: ora il plugin usa anche il blocco forte di LiteSpeed Cache (dalla 7.9.2) e la costante `DONOTCACHEPAGE`;
  - una risposta 403 per autenticazione non valida (per esempio un `X-WP-Nonce` errato) veniva decisa da WordPress prima del controllo del plugin e poteva essere messa in cache: ora il plugin lo dice a LiteSpeed Cache anche all'uscita.
- Precisazione sulla 2.23.2: senza LiteSpeed Cache cambia solo che le risposte portano gli header «no-cache» standard.

