
- Aggiunta nel menu ticinoWEB CMS una pagina “Integrazione Zefix” con stato operativo, configurazione per-sito e istruzioni per la messa online.
- Mantenute le costanti server come fonte prioritaria, con un fallback amministrabile dal backend quando il provider di hosting non consente di configurarle.
- Protetti salvataggio e verifica del collegamento con capability e nonce; la password salvata non viene mai ristampata in chiaro e le opzioni non sono caricate automaticamente.
- Aggiunto un controllo manuale della connessione Zefix con esito sicuro, senza mostrare credenziali o dettagli interni.
- Sostituito sul solo sito Deltora il banner cookie generico con un consenso aderente ai trattamenti realmente presenti: memorie necessarie e Google Maps facoltativo.
- Rimossi dal pannello pubblico i consensi inutilizzati per analytics e marketing e disattivati, sul solo sito Deltora, sia il loader Analytics sia il contatore visite ereditati dal parent.
- Bloccato il caricamento dell’iframe Google Maps fino al consenso, con alternativa sempre disponibile verso la mappa esterna.
- Aggiunto nel footer il comando permanente “Preferenze cookie”, con revoca immediata, dialog accessibile, focus gestito e supporto da tastiera.
- Aggiornata in modo conservativo l’informativa privacy gestita da WordPress con durata delle preferenze, dati tecnici trasmessi a Google e modalità di revoca.
- Generate automaticamente `srcset`, `sizes` e dimensioni intrinseche per le immagini della hero e dei servizi collegate alla Media Library, riducendo payload e layout shift.
- Resa compatibile la risoluzione degli allegati con i vecchi URL Multisite che includono il percorso del sottosito.
- Aggiunte dimensioni esplicite alle icone SVG dei servizi e rimosse le transizioni di layout da header e navigazione, mantenendo invariati stati e composizione.

