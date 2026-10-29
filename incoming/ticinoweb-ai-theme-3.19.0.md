
- **Tabelle elenco, colonne ridimensionabili**: in tutte le tabelle del backend (articoli, pagine, prodotti, ordini, utenti, tipi di contenuto...) si trascina il bordo destro di un'intestazione per allargare o stringere la colonna; doppio clic sul bordo per tornare alla larghezza automatica. Le larghezze restano salvate per ogni schermata nel browser di chi le imposta (nuovo `assets/js/admin-columns.js`, disattivabile con il filtro `ticinoweb_admin_resizable_columns`). Solo da 783 px in su.
- **Intestazioni che si sovrapponevano**: il testo delle intestazioni ora va a capo dentro la propria colonna anche quando un plugin forza `nowrap` (es. "Visualizzazioni: 30 giorni" di Jetpack sopra "Traduzioni").
  - Motivo: poter gestire la larghezza delle colonne ed evitare testi sovrapposti.

