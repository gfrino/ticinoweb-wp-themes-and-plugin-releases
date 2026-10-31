- Home, telefono: il titolo della hero **non spezza più le parole** a metà («D / I VIVERE»). Ogni parola
  resta intera e l'a capo avviene solo tra le parole; carattere un po' più piccolo e righe bilanciate.
- Titoli animati: il testo completo è letto correttamente da screen reader (prima veniva letto lettera
  per lettera); con «riduci animazioni» attivo i titoli compaiono subito; il tracciamento del mouse
  è attivo solo dove esiste il puntatore.
- Modulo contatti: ora usa il gestore del parent. I messaggi finiscono in **Invii Ricevuti**, con
  antispam (honeypot e limite di invii), reCAPTCHA se configurato, casella di consenso alla privacy,
  errori sotto ogni campo e conferma senza ricaricare la pagina. Prima inviava una mail diretta
  all'amministratore, senza archivio né antispam.
- SEO: tolto il secondo `<title>` della pagina (ne restava uno vuoto o a metà accanto a quello di WordPress).
- Prestazioni: le pagine standard non sono più escluse dalla cache LiteSpeed.
- Hero: il video si legge dalla libreria **Media** (non più dalla cartella del tema, che l'aggiornamento
  sostituisce); se manca, la hero resta visibile con lo sfondo blu.
- Pulizia: rimossi `check_page.php` e `front-page.php.bak`; tolta la barra rossa laterale e il
  gradiente dal riquadro del manifesto in Attività; aggiunta la copertina `screenshot.png`.
