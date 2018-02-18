# yourls-change-error-messages

When attempting a new short url, YOURLS default behavior is to simply send out an error message: 
-  whenever a requested custom keyword already exists in the database
-  when a url already exists in the databse and `define( 'YOURLS_UNIQUE_URLS', true );` is set in `config.php`

This plugin changes that behavior and the content of those messages so that:
-  If a keyword already exists, the error message will display the URL for that keyword.  
-  If the URL already exists, its shortened url will be returned and the share box will be displayed.

This also works so that the API returns postive values as well.
