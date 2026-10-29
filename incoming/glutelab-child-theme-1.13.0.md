
- Aggiunto il nuovo accesso dedicato `/glutelab-login/`, affiancato al normale `/tw-login/` senza modificarne il funzionamento.
- Introdotto il ruolo per-sito “Gestore Glute Lab”, limitato realmente a Gestione Glute Lab e ai suoi sei tab.
- Bloccato per il ruolo dedicato l’accesso diretto a dashboard, articoli, pagine, impostazioni, utenti e strumenti; amministratori e accesso classico restano invariati.
- Allineati menu, Settings API, Pacchetti e azioni amministrative alla capability specifica `manage_glutelab`.
- Personalizzata la schermata di accesso con logo ufficiale, layout viola/lilla responsive, focus accessibile e messaggi chiari.
- Mantenute disponibili soltanto le funzioni tecniche indispensabili alla gestione, compresa la Libreria Media usata dai pacchetti.
- Aggiunti test automatici per route Multisite, ruolo, capability, redirect, allowlist e separazione dagli amministratori.

