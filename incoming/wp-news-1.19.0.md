
*   **Added**: *Resend confirmation* for pending subscribers (row button and bulk action in *Subscribers*), with a 2-minute guard against double clicks.
*   **Added**: multilingual support for **WPML** and **tW Translate Plus** (`WPNews_Language`): the page language is sent with the form and stored with the subscriber (`lang` column, also from the WooCommerce checkout); the reply, the confirmation email, its link (`/fr/…`) and the confirm/unsubscribe pages use it. The checkout checkbox text is registered in WPML String Translation / translated by tW Translate. Language badge in *Subscribers*.
*   **Added**: French and German translations of all visitor-facing strings (form, messages, emails, confirm/unsubscribe pages, checkout).
*   **Changed**: confirmation email redesigned for email clients: site logo (Settings → Logo in the emails, else Elementor/theme logo, else site icon), solid colours instead of a gradient (Gmail and Apple Mail dropped it and the white title was invisible), button colour setting, fallback link.
*   **Changed**: email links use a plain `&` (like the `tw-mail-link-entities-fix` mu-plugin), safest for every rewriter and client.
*   **Fixed**: subscriber delete/blacklist moved to `admin-post.php` (same generic `action=` issue as lists in 1.17.1).
*   **Changed**: the DB version check also runs on the front end (with a lock), so a signup right after an automatic update finds the new columns.


