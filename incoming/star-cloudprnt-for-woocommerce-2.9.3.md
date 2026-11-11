
### Fixed
- Multisite: l'impostazione «ModSecurity Bypass» era salvata sito per sito, ma il file `cloudprnt/.htaccess` è unico per tutta la rete. Bastava un sito con il bypass disattivato (per esempio un sito migrato da un altro server) perché il plugin cancellasse il file a ogni caricamento di pagina: tutte le stampanti CloudPRNT del server ricevevano HTTP 403 e smettevano di stampare (successo l'11.11.2026 su ticinoweb01 dalle 14:37 alle 18:08). Ora l'impostazione vale per tutta la rete, la può cambiare solo l'amministratore di rete (con una conferma prima di spegnerla) e i vecchi valori dei singoli siti vengono ignorati.
- Se il bypass è attivo e il file `.htaccess` manca (copia o migrazione del sito che salta i file nascosti), il plugin lo ricrea da solo; se non riesce a scriverlo lo segnala nelle impostazioni e riprova al massimo una volta all'ora.
- Il messaggio di esito del pulsante viene mostrato come testo, non come HTML.

