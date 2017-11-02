# ssi-defaultpage
Default webserver page on SSI, showing some useful info about client's connection.

## Usage:
* Upload index.shtml to default virtual host's root directory
* Enable SSI processing, if you see only blank fields instead of info. For [NGINX](http://nginx.org/en/docs/http/ngx_http_ssi_module.html), for [Apache2](https://httpd.apache.org/docs/2.2/howto/ssi.html).
* Enjoy! :)

## Is it secure?
Literally - yes, the only risk - disclosure info about your server behind CDN if hosts misconfigured. You can simply delete server info block from `index.shtml`.

## Troubleshooting
Wrong client's IP address: use corresponding headers for your CDN ([CloudFlare example](https://www.cloudflare.com/technical-resources/#mod_cloudflare))
