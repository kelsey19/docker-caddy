# Dockerfile for Caddy
[![](https://images.microbadger.com/badges/image/sithladyraven/docker-caddy.svg)](https://microbadger.com/images/sithladyraven/docker-caddy)[![](https://images.microbadger.com/badges/version/sithladyraven/docker-caddy.svg)](https://microbadger.com/images/sithladyraven/docker-caddy)[![](https://images.microbadger.com/badges/commit/sithladyraven/docker-caddy.svg)](https://microbadger.com/images/sithladyraven/docker-caddy)

Includes the following plugins:

* dyndns
* http.cache
* http.cgi
* http.cors
* http.datadog
* http.expires
* http.filemanager
* http.filter
* http.forwardproxy
* http.geoip
* http.ipfilter
* http.jwt
* http.locale
* http.login
* http.minify
* http.nobots
* http.prometheus
* http.proxyprotocol
* http.ratelimit
* http.realip
* http.reauth
* http.webdav


## How to run

```
docker run \
  --volume $PWD/Caddyfile:/etc/caddy/Caddyfile \
  --volume $PWD/certs:/var/lib/caddy \
  --volume $PWD/html:/var/www \
  --publish 80:80 \
  --publish 443:443 \
  sithladyraven/docker-caddy:latest
```
