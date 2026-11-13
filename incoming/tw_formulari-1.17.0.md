
### Added
- **Rimborsi dalla compilazione.** Nel dettaglio di una compilazione pagata c'è il riquadro **Rimborso** con quanto è stato pagato, quanto è già stato rimborsato e quanto si può ancora rimborsare. Si scrive l'importo (tutto o una parte), si sceglie il motivo e si può aggiungere una nota interna; «Rimborsa con Stripe» chiede conferma con l'importo e restituisce il denaro al cliente sullo stesso metodo con cui ha pagato. Prima i rimborsi si facevano solo sul pannello di Stripe e la compilazione restava «pagata», senza traccia nel sito.
- **Storico dei rimborsi**: ogni rimborso resta registrato con data, importo, stato, motivo, nota e chi l'ha fatto, anche i tentativi non riusciti (con il motivo dell'errore). La compilazione diventa «Rimborsata in parte» o «Rimborsata»; i due stati sono nel filtro dell'elenco e l'esportazione CSV ha la colonna «Rimborsato».
- **Rimborsi fatti direttamente su Stripe** compaiono da soli: il webhook riceve ora anche `charge.refunded` e `refund.updated`, e il pulsante «Aggiorna da Stripe» li legge su richiesta. La pagina Pagamenti avvisa quando il webhook esistente va ricreato per ricevere questi eventi.
- Compilazioni pagate con bonifico o in altro modo: il rimborso si registra (il plugin non muove denaro), così resta nello storico.
- Un pagamento di prova si rimborsa con le chiavi di prova anche se il sito è già passato in modalità reale.
- Sicurezza del denaro: importo mai oltre il rimborsabile (controllato dal server), chiave di idempotenza verso Stripe e blocco per compilazione contro il doppio clic, permessi da amministratore e nonce. Con una chiave «con restrizioni» l'errore spiega di dare il permesso «Refunds: Scrittura».
- Azione `twf_payment_refunded` per chi vuole collegare altro (e-mail, contabilità).
- Test: 24 nuovi controlli sui rimborsi nel test d'integrazione con lo Stripe finto (120 in totale).

### Fixed
- Test del motore (`tests/builder-run.php`): al finto WordPress mancava `wp_attachment_is_image()`, usata dalla foto del buono dalla 1.13.0, e 30 test fallivano senza motivo.

