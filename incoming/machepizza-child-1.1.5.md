### Fixed
- Footer: l'immagine "Divieto alcolici minori" puntava a `http://localhost:8081/...` (residuo dell'ambiente locale). Chrome mostrava ai visitatori la richiesta "Accedere ad altre app e servizi su questo dispositivo" (Local Network Access) e l'immagine risultava rotta. Ora viene caricata da `assets/img/alcolici-minori.jpg` del tema ed è mostrata solo se il file esiste.

### Changed
- Nuova copertina `screenshot.png` 1200×900 (logo ufficiale su rosso del tema), richiesta da `release-theme.sh`.
- Include le modifiche già su `main` dopo la 1.1.4: redirect `/app` verso gli store con apertura automatica del pannello app su desktop, titoli dei prodotti dell'hero mostrati per intero.
