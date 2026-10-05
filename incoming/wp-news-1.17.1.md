
*   **Fixed**: deleting or renaming a list (and removing / blacklisting a member from a list) could silently do nothing on some sites. These actions were GET requests on the Lists page with a generic `action=delete` parameter that other plugins may intercept; they now go through `admin-post.php` (`wpnews_list_action`, nonce bound to operation and list) and redirect back with a confirmation message.
*   **Fixed**: running *Import from MailPoet* a second time created a duplicate of every list. Lists with the same name are now reused (memberships are added with `INSERT IGNORE`).


