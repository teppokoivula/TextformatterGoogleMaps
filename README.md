# ProcessWire Google Maps Textformatter

Looks for Google Maps URLs within paragraph (`<p>...</p>`) HTML tags and automatically converts them to embedded maps. Configurable options include embed type ("static" or "iframe"), API key, responsive embedding and Google Maps for Business settings.

## How to install

See "How-To Install or Uninstall Modules" page at modules.processwire.com: http://modules.processwire.com/install-uninstall/.

## How to use

Edit settings of any textarea field and enable "Google Maps" textformatter from Details tab. Recommended to be used with TinyMCE or CKEditor fields.

## Notes about Google Maps for Business

Generated signature is based on specific URL and private cryptographic key.

In order to use your private key within this module you'll have to save it in module configuration settings, which are stored as *plain text* in your database. Google's documentation, on the other hand, explicitly states that this private key should *not* be "stored on any websites".

Use this feature at your own risk and only if you're fully aware of the risks involved!

Code used by this module for generating encoded signatures was adapted from Google's Extended URL signing gallery sample for PHP: http://gmaps-samples.googlecode.com/svn/trunk/urlsigning/UrlSigner.php-source.

---
Copyright (c) 2013, Teppo Koivula
