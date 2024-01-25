# Let's Encrypt Add-On with ECDSA

**Depreciated - features now available in official addon starting with version 5.0.13**

This add-on was created after my PR to add ECDSA to the official Let's Encrypt add-on was not accepted. Since I still want to use ECDSA certificates with Home Assistant, this version adds the options I want to use.

My ECDSA version adds configuration settings to generate a certificate key using RSA or ECDSA (default ECDSA), and an optional elliptic curve selection (256 or 384, default 384) for ECDSA keys.

Note: RSA is still the most backwards compatible with older devices or operating systems that won’t be updated to support ECDSA, but anything in the last 5+ years should support ECDSA.

### What happens if you need to revert to RSA?

You will need to uninstall and re-install the add-on because Certbot will check the last certificate it requested and won't generate a new one until it's within 30 days of expiration. Make sure to copy your configuration (YAML mode is easiest to copy/paste) before uninstalling so you can quickly reconfigure the integration when you install it again.

# Add-On Repository

Configure `https://github.com/WillCodeForCats/ha-addon-letsencrypt-ecdsa` in your add-on repositories.

# References
* https://github.com/home-assistant/addons/tree/master/letsencrypt
* https://github.com/home-assistant/addons/pull/3130
