
- **Gli articoli del blog in russo si aprono di nuovo.** Tutte le pagine degli articoli in `/ru/` rispondevano con un errore (pagina 500). Nel riquadro «articoli correlati» il tempo di lettura usa il testo «%d min»: la traduzione automatica in russo aveva trasformato il segnaposto del numero in «%д», e PHP si fermava con un errore fatale.
- I testi tradotti che contengono un numero o un nome (tempo di lettura, «Trovati N prodotti», prezzo unitario nel carrello, testo alternativo del logo, numero di trattamenti nel menu, titoli dei trattamenti correlati) passano ora da `synergy_tf()`: la traduzione si usa solo se ha gli stessi segnaposto dell'originale, altrimenti compare il testo originale. Una traduzione rovinata non può più bloccare una pagina.

Perché: l'errore era nel log dal 4 novembre almeno; una stringa tradotta male non deve mai rendere irraggiungibile una pagina, tanto meno il menu, che è in tutte le pagine.

