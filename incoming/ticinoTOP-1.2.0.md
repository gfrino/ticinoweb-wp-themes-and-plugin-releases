
### Nuovo
- **Scanner AI → sito aziendale**: legge home e pagine chiave del sito di un'azienda, compila la scheda con l'AI (descrizione, analisi, località, contatti, keywords, categoria, punteggi) e la pubblica in **Aziende** dopo un'anteprima modificabile. Se l'azienda è già presente (stesso dominio) la aggiorna invece di duplicarla.
- Schede azienda: campi sito web, località, indirizzo, telefono, email; descrizione, contatti e pulsanti reali nella pagina.
- La chiave API OpenAI si gestisce in Scanner AI → Impostazioni e non viene più mostrata nella pagina.

### Sicurezza
- Rimossi i proxy di terze parti e la chiave ScraperAPI scritta nel codice. Le letture di URL esterni usano `wp_safe_remote_get`, che blocca gli host interni.
- Il form Candidature e l'email TopScan passano dal gestore form del parent: token fresco compatibile con la cache, honeypot, limite di invii per IP, reCAPTCHA se configurato.
- Il tema non abilita più gli upload SVG non sanificati e non modifica più i tipi di file ammessi per tutto il network.
- Protezione CSRF sull'eliminazione dei log dello scanner e sul pulsante di test mail.

### Performance
- `style.css` del child viene caricato una volta sola (prima due) e non si carica più Poppins, che non era usato.
- Font Inter e Playfair Display ospitati nel tema e Chart.js con versione fissata, niente più Google Fonts e jsdelivr.
- Niente più lavoro pesante a ogni pagina admin: sideload delle immagini solo sul post salvato, privacy e riparazione log una tantum. Loghi e badge con cache invece di una query SQL a ogni pagina.
- La ricerca fa il join solo sulle keywords, non su tutti i meta.

### SEO e aspetti legali
- Niente più valori inventati quando mancano i dati (voto 4.8, 1.248 recensioni, AI Match 96%, "#1", barre fisse): il ranking è calcolato davvero e gli indicatori usano i punteggi reali.
- Le aziende dimostrative si importano solo con `TT_DEMO_DATA` definita (sviluppo).
- Informativa privacy sui form, titolare della privacy policy dai contatti del parent, link all'impressum nel footer se la pagina esiste.
- Nessun link `href="#"` sui pulsanti. La descrizione SEO delle schede pubblicate va nel campo tW SEO del parent.
