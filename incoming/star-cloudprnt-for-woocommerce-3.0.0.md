
### Changed
- Il plugin richiede PHP 8.5 (header `Requires PHP`, `readme.txt`, controllo all'avvio del plugin e del modulo Call Center). Il supporto a PHP 8.4 e precedenti è stato tolto: su un sito con PHP più vecchio WordPress non propone l'aggiornamento, e se il plugin viene comunque installato mostra un avviso in amministrazione e non si carica (le stampanti smettono di stampare). Prima di aggiornare un sito, portarlo a PHP 8.5.
- Nessun polyfill o ramo di compatibilità da togliere: il codice era già pulito; tutti i file passano `php -l` con PHP 8.5 senza avvisi di deprecazione.

