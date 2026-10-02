
### Nuovo
- **Ricerca web con la chiave OpenAI** (Responses API, tool `web_search`): per ogni azienda cerca registro di commercio (ragione sociale, forma giuridica, UID, anno di fondazione), voto e numero di recensioni Google, altre piattaforme di recensioni (local.ch, search.ch, Trustpilot…), orari, servizi e profili social.
- **Dati veritieri**: ogni dato trovato dall'AI viene tenuto solo se la sua fonte è una pagina realmente consultata dalla ricerca (o il sito ufficiale). Il resto viene scartato e l'anteprima dice quanti dati sono stati scartati. Accanto ai campi verificati c'è il link alla fonte; voti fuori scala, UID non validi e numeri di recensioni mancanti vengono rifiutati.
- **Bottone "Aggiorna dati con AI"** nel metabox "Dati Reputazionali Azienda" e azione "Aggiorna con AI" nella lista Aziende: rilegge il sito e rifà la ricerca solo con OpenAI, mostra l'anteprima e aggiorna la stessa scheda (stato e immagine attuali mantenuti).
- Schede più complete: ragione sociale, forma giuridica, UID, anno di fondazione, orari, servizi, altre recensioni e fonti, nel metabox, nell'anteprima, nella pagina pubblica e nel PDF.
- **Interfaccia nuova**: anteprima e metabox a sezioni con icone, badge recensioni Google con icona G, stelle e link, colonna "Voto" con stelle nella lista Aziende; nella scheda pubblica badge Google, altre piattaforme, servizi, dati aziendali, orari, social e fonti.
- Impostazioni: "Modello OpenAI per la ricerca web" (default `gpt-4.1-mini`; se il modello non è disponibile si passa da solo a `gpt-4.1-mini` / `gpt-4.1`, e da `web_search` a `web_search_preview`).

### Cambiato
- Il voto modificato a mano nel metabox non viene più presentato come voto Google.
- Google Places resta facoltativo: se in ticinoWEB CMS c'è una chiave Google, le schede Places con lo stesso sito vengono proposte per prime.
- Sostituita `get_page_by_title()` (deprecata da WordPress 6.2).

