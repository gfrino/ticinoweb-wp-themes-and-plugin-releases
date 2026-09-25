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

Si pubblica **su GitHub**, da qualsiasi macchina con accesso git (SSH) a
questo repo: non serve un token personale né un server particolare.

```bash
cp <slug>-<versione>.zip <slug>-<versione>.md incoming/   # .md = changelog, opzionale
git add incoming && git commit -m "release: <slug> <versione>"
git tag <slug>-v<versione>
git push origin main <slug>-v<versione>
```

Al push del tag il workflow `.github/workflows/release-from-tag.yml` (GitHub
Actions, con il token interno del repo) controlla che lo zip abbia la cartella
`<slug>/` alla radice e crea la release: titolo = tag, asset = lo zip, corpo =
il `.md`. Se la release esiste già non fa nulla. Lo stato si segue nella
scheda **Actions** del repo.

Prima di pubblicare, nel repo sorgente: bump della versione, changelog,
commit e push. Lo zip si costruisce dal sorgente escludendo gli artefatti di
sviluppo (`rsync-exclude.txt`: niente `*.md`, test, `node_modules`…).

## Installazione manuale

Scaricare lo zip dall'ultima release del prodotto e caricarlo da
Aspetto → Temi → Aggiungi → Carica tema (o Plugin → Aggiungi → Carica plugin).
