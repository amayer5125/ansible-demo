# Webserver

Configures a webserver to serve a website using Nginx and PHP.

## Role Dependencies

- nginx
- php

## Variables

### Writable Files

A list of files and directories that should be able to be written to. These are added as SELinux rules.

```yaml
webserver_writeable_files:
  - /srv/http/example.com/storage(/.*)?
  - /srv/http/example.com/bootstrap/cache(/.*)?
```
