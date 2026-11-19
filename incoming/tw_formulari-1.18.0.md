
### Added
- **Su Stripe si vede chi ha pagato.** Il nome e l'e-mail scritti nel modulo (campo «Nome» e campo e-mail) accompagnano ora ogni pagamento: compaiono nella colonna «Cliente» dell'elenco pagamenti di Stripe e nei dati del pagamento (`twf_name`, `twf_email`). Prima il nome arrivava solo con Google Pay o Apple Pay, che lo mandano da soli: con una carta scritta a mano la colonna restava vuota e per capire di chi fosse un pagamento bisognava cercarlo nel sito. Non serve impostare niente; se il modulo ha scelto un'e-mail per la ricevuta, vale quella. Se Stripe non accetta il nome o l'e-mail, il pagamento va avanti lo stesso senza.
- **Codice della transazione nella compilazione**: sotto l'importo c'è il codice che Stripe dà al pagamento (`pi_…`), con il pulsante «Copia». Serve per ritrovare il pagamento su Stripe o per darlo all'assistenza. L'esportazione CSV ha la colonna «Codice della transazione», e incollando il codice nella ricerca delle Compilazioni si apre la compilazione di quel pagamento.

### Changed
- Il riquadro **Rimborso** è ora chiuso finché non serve: l'intestazione dice già quanto è stato rimborsato («rimborsato 0,00 CHF di 50,00 CHF») e si apre con un clic o da tastiera. Si apre da solo quando si torna da un rimborso o da «Aggiorna da Stripe», per mostrare l'esito. Prima occupava mezza pagina in ogni compilazione pagata, con il pulsante di rimborso sempre a portata di clic.
- Test: 4 nuovi controlli su nome ed e-mail del pagamento (124 in totale).

