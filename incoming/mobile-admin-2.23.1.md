### Fixed
- Il plugin non carica più `build/main.css` su tutte le pagine di wp-admin. Era il CSS della vecchia interfaccia React (ritirata nella 2.4.1) e conteneva un reset globale: `* { box-sizing: border-box; padding: 0 }`, `p { margin: 0 }`, `body { font-family: Roboto }` e `.show { opacity: 1 !important }`. Su ogni sito con Mobile Admin alterava il back office: il logo tondo della voce «ticinoWEB CMS» risultava schiacciato (22×16 invece di 22×22) e i paragrafi di avvisi e impostazioni non avevano spazio tra loro.

### Removed
- La cartella `build/` (`main.css`, `index.html`), la funzione `ADR_showContent()` (non collegata a nessun menu) e la variabile JS globale `fetch_url` stampata su ogni pagina admin: servivano solo alla vecchia interfaccia React.

