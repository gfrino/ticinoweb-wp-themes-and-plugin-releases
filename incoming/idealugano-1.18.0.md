- Nuova pagina **Marchi → Fornitori**: i tre elenchi della pagina Marchi (sistemi per tende, editori tessili, passamanerie) si gestiscono dalla bacheca. Una scheda per gruppo, una riga per fornitore con nome e logo, si trascina per cambiare ordine (o con le frecce, per chi usa la tastiera), più un pulsante per ordinare dalla A alla Z. Accessibile agli editor, come la pagina Marchi.
- Un fornitore senza logo non è un errore: resta il nome composto nel carattere del sito, e la pagina lo dice.
- C'è un modo per tornare indietro: "Riporta i tre elenchi a come erano alla consegna" rimette i 60 fornitori originali.
- Gli elenchi ora vivono nel database (opzione `idealugano_suppliers`, fuori autoload). `inc/suppliers-data.php` resta come seme della prima volta ed è generato da `tools/gen-suppliers.py`: modificarlo a mano non cambia più il sito.
- Il primo sottomenu si chiama ora "Partner in evidenza", per distinguerlo da "Fornitori".
- Gli editor possono raggiungere la nuova pagina: il tema limita le schermate admin a un elenco, e Fornitori è stato aggiunto (`inc/editor-role.php`).

