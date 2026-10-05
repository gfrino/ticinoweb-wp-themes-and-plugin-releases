
*   **Fixed**: confirmation, unsubscribe and tracked links in emails could arrive broken ("Invalid or expired confirmation link") when the SendGrid account has *Google Analytics* tracking enabled: it appends `utm_*` parameters and does not decode `&#038;`, turning the rest of the query string into a `#` fragment. Links in email bodies are now written with `&amp;` (`WPNews_Security::email_url()`) and Google Analytics tracking is disabled per message, like click/open tracking already were.


