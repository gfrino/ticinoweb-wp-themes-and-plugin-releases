- **Tema riutilizzabile per qualsiasi studio medico**: tolti dal tema tutti i dati di Fratila-Blanc (nome, medici, recapiti di riserva, località, coordinate, loghi, partner, attestati PDF, foto di Melano, testi SEO e privacy). Se un dato manca il blocco che lo mostra non viene stampato.
- Pannello **Studio medico** ampliato: logo testuale (prefisso e nome), sigla e appartenenza (es. FMH, con link e logo nel footer), testo e nota della sezione Contatti, specialità, zone servite e coordinate per i dati strutturati.
- Dati strutturati `MedicalClinic`: indirizzo, località e CAP ricavati dall'indirizzo del CMS; specialità, zone servite e coordinate dal pannello (niente più valori fissi).
- Seeder ridotto alla struttura (Home, Privacy Policy, home statica, fuso orario svizzero): non scrive più contatti, SEO o medici. La Privacy Policy è generata con i dati del sito.
- Immagini del cliente fuori dal tema: la foto della sezione Chi siamo si sceglie dal pannello (vuota = riquadro nascosto); resta la foto hero predefinita e il logo FMH ufficiale.
- Nuova copertina `screenshot.png` neutra.
- **Migrazione**: sui siti già online aggiungere nel pannello Studio medico i campi nuovi (per Fratila-Blanc già fatto nel database).

