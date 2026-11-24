
### Fixed
- Le stampanti nuove non comparivano mai nelle impostazioni («No printer found for this site»): l'elenco delle stampanti non riportava l'indirizzo verso cui ogni stampante fa polling (`serverUrl`, registrato da `cloudprnt.php` in `data.json`), quindi il filtro «solo le stampanti di questo sito» non ne trovava nessuna su nessun sito. Funzionavano solo le stampanti scelte prima della 3.0.x. Successo il 23.11.2026 con la TSP143IV della Pizzeria Edlibacherhof.
- Le stampanti già scelte da un sito restano sempre nel suo elenco, qualunque sia l'indirizzo verso cui fanno polling (nessuno, uno vecchio o quello di un altro sito): se l'elenco le nascondesse, salvando la pagina WordPress cancellerebbe la scelta. Correggere una scelta sbagliata resta una decisione dell'amministratore.

