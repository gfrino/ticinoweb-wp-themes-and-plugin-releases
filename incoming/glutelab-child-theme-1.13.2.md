
- Reso persistente il tipo di accesso scelto: entrando da `/glutelab-login/` si arriva e si resta nella sola Gestione Glute Lab anche usando un account amministratore esistente.
- Mantenuto `/tw-login/` come ingresso separato al backend WordPress completo; aprirlo azzera esplicitamente la modalità Glute Lab.
- Limitato il contesto dedicato al singolo sottosito Multisite tramite cookie sicuro, HTTP-only e SameSite, senza modificare il parent theme.
- Estesi i test di regressione per verificare la separazione tra i due ingressi e i relativi redirect.

