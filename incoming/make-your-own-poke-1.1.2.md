
### Fixed
- «"Base" è un campo obbligatorio» quando si aggiunge la poke al carrello. Product Add-ons 8.4 chiama i campi `addon-<prodotto>-<numero>` (es. `addon-1912186493-0`) e non più `addon-<prodotto>-<nome>-<numero>`: il configuratore inviava le scelte con il nome vecchio, Product Add-ons non le vedeva e rifiutava la Base. Ora il widget prende i nomi dei campi direttamente da Product Add-ons (abbinati per nome del gruppo), con il nome vecchio solo come riserva.

