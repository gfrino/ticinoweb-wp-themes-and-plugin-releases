Correzioni dalla review TDK della 0.2.40.
- **Canonical di nuovo su tutte le pagine.** Il child toglieva il canonical del parent e contava su
  quello del core, che il parent però spegne: home, pagine e singoli ne erano senza (anche online).
  Ora il canonical lo scrive il parent e il child aggiunge solo, col filtro `ticinoweb_seo_canonical_url`,
  il numero di pagina sugli archivi dalla pagina 2 in poi.
- **Descrizione per Google sugli archivi** (Jobs, Parco macchine, Certificazioni, Referenze, ecc.):
  presa dalla pagina con lo stesso slug se esiste, altrimenti dalla descrizione del tipo di contenuto,
  riscritta come frase vera. Traducibile.
- **Modulo Contatti**: ogni richiesta si salva anche in Invii Ricevuti del CMS, usa il reCAPTCHA del CMS
  quando è configurato, e tutti i testi (etichette, pulsante, messaggi) passano dal filtro di traduzione.
  Sotto il modulo, una riga con il link a Protezione dati.
- Candidatura: stessi aiuti condivisi per reCAPTCHA e Invii Ricevuti (`tenconi_recaptcha_accoda()`,
  `tenconi_recaptcha_ok()`, `tenconi_salva_invio()`), comportamento invariato.
- Nuovo `README.md` con l'inventario di cosa il tema usa dal parent e cosa no.
- `.gitignore`: separate due regole finite sulla stessa riga.

