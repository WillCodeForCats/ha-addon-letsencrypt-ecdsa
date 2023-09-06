# Let's Encrypt Add-On with ECDSA

This add-on was created after my PR to add ECDSA to the official Let's Encrypt add-on was not accepted. Since I still want to use ECDSA certificates with Home Assistant, this version adds the options I wanted.

My ECDSA version adds configuration settings to generste a certificate key using RSA or ECDSA (default ECDSA), and an optional elliptic curve selection (256 or 384, default 384) for ECDSA keys.
