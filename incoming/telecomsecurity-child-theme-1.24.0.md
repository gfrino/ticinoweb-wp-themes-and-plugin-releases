
Il modulo Contatti ora salva le richieste nel backend e usa il reCAPTCHA impostato nel CMS.

- **Invii Ricevuti**: ogni richiesta del modulo viene registrata in ticinoWEB CMS → Invii Ricevuti (prima partiva solo l'e-mail e la tabella restava vuota). Il salvataggio avviene prima dell'invio, così la richiesta resta anche se la posta non parte; azienda, località, tipo di immobile e «già cliente» sono accodati al messaggio;
- **reCAPTCHA v3**: se nel CMS sono impostate le chiavi, il modulo carica lo script di Google e invia il token; il server lo verifica con la soglia scelta nel CMS e rifiuta l'invio senza token valido. Senza chiavi il modulo funziona come prima.

