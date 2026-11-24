
Dopo l'invio del modulo Contatti il visitatore arriva sulla pagina «Grazie».

- nuova pagina di conferma (slug `grazie`): titolo e testo sono il contenuto della pagina WordPress, modificabili e tradotti da tW Translate Plus; pulsante «Torna alla Home» e telefono dal CMS;
- il modulo porta alla pagina nella lingua in cui è stato compilato (`/grazie/`, `/en/grazie/`, `/de/grazie/`), sia con JavaScript sia con l'invio classico senza JavaScript (redirect 303);
- se la pagina `grazie` non esiste o non è pubblicata, il modulo mostra la conferma nella pagina come prima;
- e-mail, salvataggio in Invii Ricevuti e reCAPTCHA invariati;
- aggiunto il test `tools/test-thank-you-page.php`.

