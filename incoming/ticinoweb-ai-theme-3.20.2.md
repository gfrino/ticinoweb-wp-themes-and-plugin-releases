- **Email via SendGrid**: l'invio con l'API SendGrid ora passa Reply-To, Cc e Bcc di `wp_mail()` e disattiva la riscrittura dei link.
  - Motivo: le richieste dal modulo arrivavano senza Reply-To (rispondendo si scriveva al sito, non a chi aveva scritto) e con l'indirizzo del sito trasformato in un lungo link di tracciamento.

