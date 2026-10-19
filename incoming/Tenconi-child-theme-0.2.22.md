- **Nessun recapito del cliente nel codice del tema** (regola ticinoWEB dei dati dinamici). Il
  destinatario del modulo contatti si legge dalle impostazioni: prima "Email di Ricezione Form"
  (ticinoWEB CMS → Contatti), poi l'indirizzo pubblicato nella pagina Contatti, infine l'email
  dell'amministratore. Prima l'ultimo ripiego era un indirizzo scritto nel codice.
- Tolta `tenconi_footer()`: non la chiamava più nessuno (il footer legge già la pagina Contatti)
  e conteneva indirizzo, telefono ed email della sede.
- Tolti telefono, email e indirizzo da tre commenti.

