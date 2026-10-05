
The signup shortcode existed but could not be used in practice: nothing in the admin mentioned it, list ids were not shown, and a form without `list_id` stored subscribers in no list.

*   **Added**: every list card in *Lists* and the single-list page show the list's signup shortcode with a *Copy* button and the available options.
*   **Added**: *Settings → Default signup list*, used by `[wpnews_subscribe_form]` without `list`.
*   **Added**: shortcode attributes `list` (alias of `list_id`), `description`, `button`, `consent` (required checkbox with privacy policy link), `title="none"`.
*   **Fixed**: signups failed on pages served from full-page cache once the embedded nonce expired. The nonce is now checked only for logged-in users.
*   **Fixed**: an already active subscriber could not join a further list from a form (the form answered "Thank you" and did nothing). The list is now added after confirmation (or immediately without double opt-in).
*   **Security**: the list id is HMAC-signed in the form and verified server-side, so visitors cannot subscribe themselves to internal lists by editing the hidden field; unknown lists are rejected.
*   **Changed**: refreshed form styling (inherits the theme font, two-column name fields, mobile layout, CSS custom properties), result messages stay visible in an `aria-live` region.
*   **Added**: updates through the standard WordPress updater from the ticinoWEB releases repo (`Update URI` header + bundled `includes/tw-release-updater.php`, installed as mu-plugin on activation / in admin; removed on uninstall only if no other plugin uses it).
*   **Chore**: removed stray iCloud duplicate files from `build/`.


