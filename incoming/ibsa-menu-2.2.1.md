
### Fixed
- Il luogo di ritiro dell'ultimo ordine viene di nuovo proposto al checkout successivo. Lo svuotamento del carrello (nuovo giorno, nuovo menu dal wizard) azzerava la scelta nella sessione WooCommerce e il cliente doveva ripeterla a ogni ordine.

### Added
- Aggiornamenti dal repo delle release ticinoWEB con l'aggiornatore standard di WordPress (header `Update URI`, mu-plugin `tw-release-updater`).
- Il luogo di ritiro si salva nella user meta `ibsa_ultimo_luogo_ritiro` alla creazione dell'ordine (checkout classico e a blocchi). Per chi ha già ordinato vale il dato che WooCommerce conserva in `shipping_method`, quindi funziona da subito. Se il luogo non è più disponibile si usa il predefinito, e una scelta già fatta nella sessione non viene mai sovrascritta.
