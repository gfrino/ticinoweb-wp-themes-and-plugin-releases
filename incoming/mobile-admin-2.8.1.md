### Security
- L'endpoint `app-keys` esce dalla cache di LiteSpeed con l'hook `litespeed_control_set_nocache` (sul sito principale «Cache REST API» è attiva e il solo header Cache-Control della risposta veniva ignorato: la risposta, e anche il 403, risultavano cacheabili per ore). Vale sia per la risposta con le chiavi sia per il rifiuto senza segreto.

