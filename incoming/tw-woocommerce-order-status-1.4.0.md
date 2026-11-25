### Added
- **Licenza**: il plugin è venduto su ticinoweb.com con licenza perpetua per un sito. Nuova pagina
  Impostazioni → Licenze ticinoWEB: si incolla la chiave ricevuta con l'acquisto e il sito si attiva da solo.
  I siti ospitati da ticinoWEB risultano «Incluso con l'hosting ticinoWEB» senza fare nulla. Controllo in
  background ogni pochi giorni; senza licenza valida il plugin continua a funzionare, compare un avviso e non
  arrivano gli aggiornamenti. Libreria `includes/tw-license.php` 1.0.0 del development kit.

### Changed
- Aggiornatore `includes/tw-release-updater.php` 1.3.0: un plugin a pagamento senza licenza valida vede la
  versione nuova ma non la installa (filtro `tw_release_updater_package`).

