
### Cambiato
- **Voto medio e numero di recensioni vengono da Google**, non più dall'AI. Prima il voto era la media dei 6 punteggi AI diviso 20 (es. 3.5 per ticinoWEB, che su Google ha 4.8 con 51 recensioni).
- Lo scanner cerca l'azienda su Google Places e mette per prima la scheda con lo stesso sito web: nell'anteprima scegli la scheda giusta, oppure "pubblica senza voto". Non c'è più un campo per scrivere il voto a mano.
- Usa la chiave Google già configurata in ticinoWEB CMS > Google Reviews (la stessa delle recensioni del parent).
- Voto e recensioni delle aziende collegate si aggiornano da soli ogni 7 giorni (cron giornaliero, al massimo 25 aziende per volta).
- Metabox Azienda: nuovo campo "Google Place ID" per collegare a Google anche le aziende già pubblicate; al salvataggio i dati vengono riletti da Google.
- Scheda azienda: accanto al voto, "Fonte: recensioni Google, aggiornate al …" con link alla scheda Google.

