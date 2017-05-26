# ngxpkg [![Build Status](https://travis-ci.org/webpkg/ngxpkg.svg?branch=master)](https://travis-ci.org/webpkg/ngxpkg)

A cli tool for nginx

## Default Env

* NGX_CONFIG = 〜／.config／ngxpkg
* NGX_DIRECTORY_URL = https://acme-v01.api.letsencrypt.org/directory
* NGX_RESOURCE = https://rc.ngxpkg.com/
* NGX_SITE_CONFIG = /etc/nginx/conf.d
* NGX_SITE_ROOT = /opt/local/www

## Create new sites with domains test1.com, test2.com ...

```bash
ngx new test1.com test2.com
```

it will create conf files:

* /etc/nginx/conf.d/test1.com.conf
* /etc/nginx/conf.d/test2.com.conf

and create sites:

* /opt/local/www/test1.com/
* /opt/local/www/test2.com/

and apply ssl Certificates for sites.

## Notice.

please replace the files with yours after create new site.

* dhparam.pem
* ticket.pem