
### Added
- Primo rilascio: nuovo sito dell'Associazione Dico NO alla Droga, Dico Sì alla Vita, rifatto da zero sul parent `ticinoweb-ai-theme` (prima: Elementor).
- Design bold: inchiostro profondo, ciano del logo, giallo per l'azione; titoli Manrope (già self-hosted dal parent, nessun font esterno in più).
- Il sito ruota attorno a un'azione sola, **«Richiedi materiale per una conferenza»**: pulsante nell'header, nell'hero e nel footer, e modulo nella home (`[dnd_richiesta_materiale]`) con scelta tra materiale e conferenziere.
- Il modulo usa il gestore del parent (token fresco, honeypot, limite per IP, reCAPTCHA v3, «Invii Ricevuti», e-mail all'indirizzo del CMS): nessuna logica parallela. I campi della richiesta arrivano nel messaggio con i filtri `ticinoweb_form_fields` / `ticinoweb_form_errors`.
- Opuscoli: campo «File PDF» e shortcode `[dnd_opuscoli]` (copertina = immagine in evidenza), con «Richiedi copie» che preseleziona l'opuscolo nel modulo.
- Dati strutturati: l'Organization del parent diventa `NGO` con contatti e social dal CMS.
- Banner dei cookie del parent con i colori e il font del sito.
