### Fixed
- Cache: lo `style.css` caricato dal parent (`?ver=3.13.1`) restava in cache 30 giorni nei browser e annullava le correzioni di 1.8.3. Ora usa la versione del child; il child non usa più `time()` come versione, quindi il browser ricarica CSS e JS solo a ogni rilascio.

