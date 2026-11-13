
- Aggiunti i codici promozionali nativi di Stripe Checkout: durante il pagamento il cliente può inserire un coupon configurato nel pannello Stripe, senza affidare sconti o importi al browser.
- Creata l’Area cliente WordPress in `/area-clienti/`, collegata automaticamente all’email dell’acquisto e separata dal backend amministrativo.
- Trasformate le lezioni incluse nei pacchetti pagati in crediti distinti per offerta, con saldo, storico, prenotazione autonoma sugli orari realmente disponibili e protezione dalle prenotazioni concorrenti.
- Applicata la regola di annullamento a 24 ore: fino al limite incluso la lezione può essere annullata e il credito viene restituito; sotto le 24 ore l’annullamento online è bloccato e il credito resta utilizzato.
- Registrati subtotale, sconto e importo realmente pagato dal webhook Stripe firmato, incluse le transazioni interamente scontate.
- Estesi schema, privacy, amministrazione e test automatici mantenendo compatibilità con clienti, ordini e crediti storici.

