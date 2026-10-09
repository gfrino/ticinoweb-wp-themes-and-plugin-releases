
- Reso traducibile l’intero configuratore EBITDA: i testi dell’interfaccia non sono più scritti nel JavaScript ma arrivano da PHP (`deltoraConfiguratorConfig.strings`) passando da `ticinoweb_frontend_text()`, così tW Translate Plus li traduce come il resto del sito.
- Tradotti anche le voci del percorso guidato, nomi e descrizioni dei settori (le parole chiave del classificatore restano in italiano), i messaggi della ricerca Zefix e dell’invio, l’email del risultato con il link ai contatti nella lingua del visitatore.
- Aggiunto un test che blocca testi italiani scritti direttamente nello script e tiene allineato l’elenco dei testi tra JavaScript e PHP.

