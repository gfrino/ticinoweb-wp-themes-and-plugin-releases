### Changed
- Cookie banner (del parent) restilizzato nello stile del sito: card bianca compatta (max 560px) con bordo rosso, testo 13px, bottoni a pillola uppercase (Accetta giallo come "Ordina online", Personalizza bordato rosso, Rifiuta come link). Su mobile i tre bottoni stanno su una riga.
- `MACHEPIZZA_VERSION` ora usa la `Version` del tema invece di `time()`: CSS/JS non cambiano più URL a ogni richiesta (cache del browser e di LiteSpeed di nuovo efficaci), il cache busting avviene alzando la versione.

