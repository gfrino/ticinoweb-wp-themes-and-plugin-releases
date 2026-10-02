### Security
- Rimosso `build/main.js` (1.28 MB): la vecchia interfaccia React compilata non era caricata da nessuna pagina (`build/index.html` non ha `<script>`, il plugin carica solo `build/main.css`), ma era scaricabile pubblicamente da ogni sito (`/wp-content/plugins/mobile-admin/build/main.js`) e conteneva in chiaro il vecchio secret delle notifiche push. Le notifiche si inviano dal pannello PHP "Notifiche" (header `x-fcm-admin-key`, opzione `fcm_admin_key` per sito): nessun cambiamento di funzionamento.

