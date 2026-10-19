- **Ogni scheda del mega menu ha la sua immagine modificabile dal backend**, nel posto della cosa
  a cui porta:
  - **pagina** → "Imposta immagine in evidenza" nell'editor della pagina;
  - **settore** (Ferroviario infrastruttura e rotabile, Energia) → campo "Immagine nel menu" in
    Settori → modifica;
  - **archivio** (Parco macchine, Progetti e referenze, Certificazioni) → voce "Immagine nel menu" nel
    menu laterale di quel tipo di contenuto.
- L'immagine in evidenza non compare dentro le pagine (usano il modello legacy): serve solo al menu.
- Se il posto è vuoto, la scheda usa l'immagine predefinita: togliere un'immagine non lascia buchi.
- Le immagini di oggi vanno caricate una volta in questi posti, così si vedono già impostate nel
  backend (operazione sul database, fuori dal tema).

