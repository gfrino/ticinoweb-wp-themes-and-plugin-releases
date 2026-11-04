
- Header che scende con la pagina, come su tenconi.ch: resta fisso in alto; in cima è com'era
  (trasparente sopra lo sfondo azzurro della homepage), appena si scorre diventa bianco con un'ombra
  sottile e più basso, con il logo più piccolo. Su tutte le pagine e anche sul telefono.
- Nuovo `assets/js/header.js` (IntersectionObserver su un sensore in cima alla pagina, nessun ascoltatore
  su scroll). Il corpo riserva lo spazio dell'header, quindi il cambio d'altezza non sposta la pagina.

