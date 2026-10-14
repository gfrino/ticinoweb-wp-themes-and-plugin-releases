
- corretto l’errore fatale della 1.21.0 (funzione `telecomsecurity_attachment_id_from_url` dichiarata due volte): la sincronizzazione CMS → pagina usa ora l’helper già esistente;
- aggiunto il test `tools/test-no-duplicate-functions.js` contro le dichiarazioni doppie;
- footer: “Azienda formatrice” diventa una scheda come Swisscom e ISO (sfondo chiaro, etichetta, titolo e testo breve accanto al logo); con tre schede la riga occupa tutta la larghezza;
- footer: il link “Area riservata” porta alla pagina di accesso `/tw-login` (`wp_login_url()`) invece di `/wp-admin`.

