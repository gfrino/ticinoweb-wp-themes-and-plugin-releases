### Added
- Accesso app → **Password dimenticata**: si sceglie, sito per sito, cosa riceve il cliente quando tocca «Password dimenticata» nell'app. Nuova scelta «E-mail del negozio (consigliata)»: parte l'e-mail «Reimposta password» di WooCommerce, con la grafica e il mittente del negozio e il link alla pagina «Il mio account» di quel sito, dove il cliente scrive la nuova password. Le altre scelte sono l'e-mail standard di WordPress e quella che il sito aveva già in Simple JWT Login (e-mail con codice, oppure nessuna e-mail).
- Serve dove il sito era impostato su «nessuna e-mail» (il cliente toccava «Password dimenticata» e non riceveva nulla) e dove il link dell'e-mail di WordPress porta al dominio tecnico della rete invece che al sito del ristorante.
- Se si sceglie l'e-mail del negozio su un sito senza WooCommerce, senza pagina «Il mio account» o con quell'e-mail spenta, il cliente riceve comunque l'e-mail standard di WordPress, e la pagina lo dice.

### Changed
- Le scelte fatte in Mobile Admin restano anche quando le impostazioni vengono ricopiate da Simple JWT Login, e non vengono segnalate come «diverse dalla copia».
- Valgono gli stessi limiti di prima: al massimo 5 e-mail di reset all'ora per lo stesso account. La risposta data all'app non cambia («Reset password email has been sent.»).

