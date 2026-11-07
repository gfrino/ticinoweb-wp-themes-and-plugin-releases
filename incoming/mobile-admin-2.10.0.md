### Added
- **Gestione App → Collegamento app** (solo sito principale del brand): indirizzo di ritorno, Apple Team ID, Bundle ID, package Android e impronte SHA-256. Da questi dati il sito pubblica da solo `/.well-known/apple-app-site-association` e `/.well-known/assetlinks.json`, con stato «Pubblicato / Mancano …» per ogni file, e una pagina «Torna all'app» sull'indirizzo di ritorno se viene aperto nel browser. Nessun file da caricare via FTP.

### Why
- Il Datatrans Mobile SDK rifiuta i pagamenti con carta («Visa requires option appCallbackURL») finché l'app non ha un universal link / App Link verificato per il ritorno dal 3-D Secure. L'app Little Inka 3.2.0 usa `https://littleinka.ch/app/pagamento`.

