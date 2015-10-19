JavaScript frontend for Nginx JSON autoindex format
===================================================

Since nginx version 1.7.9 it supports `autoindex_format json;` directive.
When the directive is on, nginx produces very lightweight autoindex in JSON format.
This project is a JS frontend (written with AngularJS and Twitter Bootstrap) which
builds on this feature to provide modern AJAX autoindex facility.

Minimal nginx config example is in `nginx.conf` file included in the repository.
Once nginx is configured and running, put contents of the repository under some
document root, so nginx can serve it, and open `index.html` in browser via nginx.

To configure, rename `config-example.json` to `config.json` and set `base_index_url`
option to a path configured in nginx with `autoindex_format json;`.
