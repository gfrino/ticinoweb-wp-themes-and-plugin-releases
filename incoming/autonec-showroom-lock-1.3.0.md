
### Added
- Promo online: campo obbligatorio **Foto dell'auto**. Dal telefono si apre il menu per scattare la foto o sceglierla dalla galleria, dal computer la finestra dei file. Anteprima subito visibile, con «Cambia foto».
- La foto viene ridotta nel browser (massimo 2000 px, JPEG) prima dell'invio: invio veloce anche con la rete mobile.
- La foto arriva in allegato nell'e-mail di notifica e si vede in miniatura in Prenotazioni promo (clic per aprirla); il CSV ha il link.

### Changed
- La pagina Promo online è a tutta larghezza: sul computer titolo e sconto a sinistra, modulo a destra; sul telefono resta in colonna.

### Security
- Le foto sono salvate in `uploads/autonec-promo/` con nome casuale e la cartella è chiusa al pubblico: si aprono solo dalla bacheca, per chi ha i permessi. Il contenuto del file viene controllato (solo JPG, PNG, WEBP, HEIC, massimo 20 MB). Eliminando una prenotazione si elimina anche la foto.

