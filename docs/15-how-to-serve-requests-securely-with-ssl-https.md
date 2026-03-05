---
Category: 1
---
# How to serve requests securely with SSL / HTTPS

## IIS

If you are [running OwnCDN under IIS](12-how-to-enable-iis-on-windows-server.md), you follow normal procedures for enabling SSL / HTTPS for IIS websites.

That is, you get an SSL certificate, install this on Windows (follow instructions from the certificate issuer) and select the certificate in the IIS Manager under "Bindings..." for the OwnCDN website.

You can purchase certificates from many different companies - search the Internet for "ssl certificate".

Or, you can use a free SSL certification from [Let's Encrypt](https://letsencrypt.org) or similar.

We use the software [Certify the web](https://certifytheweb.com) on our Windows servers to automatically obtain, install, and continuously renew free SSL certificates (Let's Encrypt) for all our websites.


## Command line

If you are running OwnCDN from the command line, we recommend putting a reverse proxy server that can handle the SSL stuff in front of it.

For example, [Caddy](https://caddyserver.com), which can also automatically obtain, use, and renew free SSL certificates.

Or, you can use [URL Rewrite](https://www.iis.net/downloads/microsoft/url-rewrite) to turn IIS into a reverse proxy server and then enable SSL as described above. 