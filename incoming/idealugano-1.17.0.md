- Gli amministratori possono caricare file SVG nella libreria media (serve ai loghi: un PNG di marchio a schermo grande si vede sgranato). WordPress li blocca perché un SVG può contenere codice eseguibile, quindi nessun file entra com'è arrivato: `inc/svg-upload.php` lo riscrive tenendo solo gli elementi e gli attributi che disegnano, e scarta DOCTYPE, `<script>`, gestori di eventi, riferimenti esterni e `javascript:` nel CSS. Un SVG che non è XML valido viene rifiutato con un messaggio chiaro invece di finire rotto in pagina.
- Il permesso è `manage_options`: gli editor, che pure usano la pagina Marchi, non possono caricare SVG.
- La libreria media ora mostra le miniature degli SVG con le misure giuste, lette dagli attributi o dal viewBox.

