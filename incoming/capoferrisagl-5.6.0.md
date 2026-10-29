
Riordino del backend, il sito pubblico resta identico. Il child non duplica più il parent:

- **Modulo di contatto**: invia con il gestore del parent (`ticinoweb_submit_form`). Le richieste arrivano in ticinoWEB CMS → Invii Ricevuti, con reCAPTCHA v3, limite di invii e destinatario/SMTP dal CMS. Eliminati il CPT «Moduli ricevuti», l'invio proprio e il destinatario separato.
- **Dati azienda**: telefono, email, indirizzi, social, dati fiscali, link alla mappa, orari e logo si leggono da ticinoWEB CMS → Contatti / Look & Feel. Rimossi dalle «Impostazioni sito» e dal codice i valori scritti a mano. Restano nel child solo nome e ragione sociale, logo alternativo e immagine predefinita.
- **Servizi**: la tab «Servizi Principali» del CMS rimanda a Capoferri → Servizi e `ticinoweb_get_services()` legge i servizi del sito.
- **Migrazione automatica** al primo avvio (`inc/migrate-to-parent.php`): copia i dati nei campi del parent senza sovrascrivere quelli già compilati, dopo aver salvato una copia in `cfs_premigration_backup`.
- Richiede ticinoweb-ai-theme 3.20.0.

