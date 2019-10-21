## Nginx role

Some description for Nginx role would be nice. Any volunteers?

### Parameters

**nginx_version** (type `string`, default `1.14.*`)

Example:
```yaml
nginx_version: 1.14.*
```

**nginx_modules** (type `array`, default `[]`)

Example:
```yaml
nginx_modules:
  - ngx_http_geoip_module
```

**nginx_configs** (type `array`, defalt `[]`)

Example:
```yaml
nginx_configs:
  - name: fqdn
    src: /vagrant/templates/fqdn.conf.j2
```

**nginx_snippets** (type `array`, defalt `[]`)

Example:
```yaml
nginx_snippets:
  - name: fastcgi
    src: /vagrant/templates/fastcgi.conf.j2
```

**nginx_sites** (type `array`, default `[]`)

Example:
```yaml
nginx_sites:
  - name: athena
    src: /vagrant/templates/athena.conf.j2
```
