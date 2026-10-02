### Added
- **Icone Categorie: drag & drop dalla libreria alle categorie.** Si trascina un'icona su una riga: la riga si evidenzia, l'icona viene assegnata come SVG (e sostituisce un eventuale "equivalente"), l'anteprima si aggiorna.
- **Clicca e assegna** per trackpad, tablet e touch: clic sull'icona, poi clic sulla categoria. `Esc` annulla. Le icone sono raggiungibili da tastiera (Tab + Invio).
- **Ricerca** nella libreria icone (filtra per nome e nasconde i gruppi vuoti).
- **Barra "Modifiche non salvate"** in basso con il pulsante Salva, mostrata dopo un'assegnazione, un riordino o una modifica nella tabella.

### Security
- Salvataggio: i valori di tipo SVG passano da `esc_url_raw()` oltre che da `sanitize_text_field()`.

### Note
- Il riordino delle righe (⠿) continua a funzionare: i due trascinamenti sono distinti.

