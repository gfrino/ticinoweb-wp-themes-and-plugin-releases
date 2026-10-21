
Correzioni della review ticinoWEB sui cinque assi (sicurezza, performance, SEO, UI/UX, multilingua).

- **Recapiti da un solo posto**: telefono, e-mail e indirizzo del footer e della home non sono più scritti nel codice del tema; arrivano dal ticinoWEB CMS (Contatti), come già facevano header e pagina Contatti. Cambiando un recapito nel CMS cambia ovunque, e il dato visibile coincide con quello dei dati strutturati. Una riga senza valore non viene più mostrata;
- **SEO, un solo `<h1>` nella home**: il primo messaggio della hero resta `<h1>`, gli altri due hanno lo stesso aspetto ma non concorrono con il titolo principale;
- **Nessun ID di database nel codice**: il simbolo di ogni servizio arriva dalla scelta fatta nel CMS, il titolo su una riga si riferisce allo slug della pagina, la galleria ISO e il logo “Azienda formatrice” del footer si cercano per slug. Il tema è installabile su un'altra installazione senza ritocchi;
- **Video della hero**: tolto l'attributo `media` sulle sorgenti (i browser lo ignorano dentro `<video>`: su desktop si vedeva comunque la versione mobile); il video è quello caricato nella Libreria media e indicato nel CMS, con `preload="metadata"` e, se impostata come immagine in evidenza del video, una locandina;
- **Tema più leggero di 10,7 MB**: i quattro file video non vengono più trasportati nel tema a ogni aggiornamento; stanno nella Libreria media del sito;
- **Pagine più veloci**: l'elenco dei servizi, i recapiti e i testi istituzionali vengono ora calcolati una volta sola per pagina invece di essere ricostruiti a ogni richiamo (nella home decine di volte);
- versione allineata ovunque (`style.css`, costante del tema, asset della home) e `Theme URI` corretto;
- test aggiornati: contratto del video hero e del titolo unico, nessun ID numerico nel codice.
