Opauth-Dropbox
=============
[Opauth][1] strategy for Dropbox authentication.

Implemented based on https://www.dropbox.com/developers/blog/45/using-oauth-20-with-the-core-api

Getting started
----------------
1. Install Opauth-Dropbox:

   Using git:
   ```bash
   cd path_to_opauth/Strategy
   git clone https://github.com/t1mmen/opauth-dropbox.git Dropbox
   ```

  Or, using [Composer](https://getcomposer.org/), just add this to your `composer.json`:

   ```bash
   {
       "require": {
           "t1mmen/opauth-dropbox": "*"
       }
   }
   ```
   Then run `composer install`.


2. Create Dropbox application at https://www.dropbox.com/developers

3. Configure Opauth-Dropbox strategy with at least `Client ID` and `Client Secret`.

4. Direct user to `http://path_to_opauth/dropbox` to authenticate

Strategy configuration
----------------------

Required parameters:

```php
<?php
'Dropbox' => array(
	'client_id' => 'YOUR CLIENT ID',
	'client_secret' => 'YOUR CLIENT SECRET'
)
```

License
---------
Opauth-Dropbox is MIT Licensed
Copyright © 2014 Timm Stokke (http://timm.stokke.me)

[1]: https://github.com/opauth/opauth
