# ticinoWEB — release temi e plugin WordPress

Repository pubblico che contiene **solo le release** (zip installabili) dei temi e
plugin WordPress sviluppati da ticinoWEB. Il codice sorgente vive in repository
privati; da qui l'updater integrato nel tema `ticinoweb-ai-theme` legge le nuove
versioni e le propone in Bacheca → Aggiornamenti.

## Convenzione

- Una release per versione, **tag** `<slug>-v<versione>` (es. `ticinoweb-ai-theme-v3.10.0`,
  `idealugano-v1.12.0`, `tw-translate-plus-v1.3.0`).
- **Asset**: `<slug>-<versione>.zip` con la cartella `<slug>/` alla radice.
- **Corpo della release**: changelog della versione (mostrato in WordPress nella
  finestra "Dettagli versione").

## Pubblicazione

Dal server ticinoweb04:

```bash
/var/www/webroot/scripts/release-to-github.sh theme  ticinoweb-ai-theme
/var/www/webroot/scripts/release-to-github.sh child  <child-slug>
/var/www/webroot/scripts/release-to-github.sh plugin <plugin-slug>
```

## Installazione manuale

Scaricare lo zip dall'ultima release del prodotto e caricarlo da
Aspetto → Temi → Aggiungi → Carica tema (o Plugin → Aggiungi → Carica plugin).
