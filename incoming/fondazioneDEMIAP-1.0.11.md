- Font: Playfair Display, Plus Jakarta Sans e le icone arrivano in **una sola richiesta** a Google Fonts (prima Plus Jakarta Sans era caricato due volte, da `header.php` e da `functions.php`).
- Hero: il video ha un'**immagine di copertina** (poster) presa dalla libreria Media (`sfondo-animato-hero-demiap-poster`), visibile subito mentre il video si carica.
- Footer: pulsante **«Preferenze cookie»** per riaprire il banner dei cookie del parent (compare solo se il banner è attivo); il banner ha colori, font e angoli del sito.
- Footer: «Area Riservata» porta a `/tw-login/` (prima a `/wp-admin/`, che dà 404).
- Customizer: tolti i campi Hero, Fondazione e Donazioni, che nessun template leggeva (modificarli non cambiava nulla sul sito).

