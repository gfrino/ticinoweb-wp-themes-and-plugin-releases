- **Posizioni aperte gestite dalla bacheca.** Prima l'elenco era scritto nel tema: il Plant Manager è
  rimasto online anche dopo che il cliente l'aveva tolto dal suo sito, e toglierlo richiedeva un
  rilascio. Ora ogni posizione è un contenuto «Lavora con noi»: titolo, testo dell'annuncio e PDF del
  profilo (facoltativi). Pubblicata compare su /jobs/, in bozza sparisce. Senza posizioni la pagina lo dice.
  Ogni posizione ha il pulsante «Candidati», che apre il modulo con la posizione già compilata.
- **Modulo di candidatura spontanea**, con i campi di tenconi.ch/jobs: nome, cognome, data di nascita,
  telefono, indirizzo con paese, email, posizione, messaggio, allegati (fino a 5 file, 10 MB) e consenso
  privacy. Le candidature arrivano per email con gli allegati e restano anche in ticinoWEB CMS → Invii
  Ricevuti (senza allegati). reCAPTCHA del CMS attivo quando le chiavi sono configurate.
- Il modulo contatti non va più in cache: la copia in cache aveva un codice di sicurezza scaduto e
  dopo un giorno ogni invio rispondeva «sessione scaduta».
- **Selettore delle lingue**: non si chiude più mentre il mouse scende dal pulsante all'elenco (un
  «ponte» invisibile copre gli 8 px vuoti fra i due, più un attimo di tolleranza in chiusura).

