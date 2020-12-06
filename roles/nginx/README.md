# Nginx

This role installs and configures Nginx and opens firewall ports for http.

## Variables

### Server Names

```yaml
nginx_server_name: example.com
```

### Web Root

Absolute path to the directory that content should be served from.

```yaml
nginx_webroot: /srv/http/example.com/public
```
