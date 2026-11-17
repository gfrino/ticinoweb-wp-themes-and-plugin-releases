### Added
- Accesso app: **«Elimina account» dall'app** (`DELETE simple-jwt-login/v1/users`), con gli stessi controlli, le stesse risposte e gli stessi codici di errore di Simple JWT Login 3.6.8. Serve alle app che lasciano eliminare il proprio account al cliente passando da questa rotta (il nuovo backend di un'app la usa già): senza, quei siti non potevano lasciare Simple JWT Login.
- Funziona solo sui siti dove l'eliminazione era già permessa nelle impostazioni copiate da Simple JWT Login; sugli altri risponde «Delete is not enabled» (codice 39), come prima. La pagina Accesso app mostra la riga «Elimina account dall'app».
- Come in Simple JWT Login, su una rete di siti il cliente viene tolto dal sito da cui parte la richiesta: l'account della rete resta, perché altri siti della rete possono usarlo.

### Security
- Un account che può lavorare in bacheca (amministratore, gestore del negozio, editore…) non può essere eliminato da questa rotta, nemmeno con un token valido: la risposta è 403.

