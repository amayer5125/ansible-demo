# Laravel

This role configures a laravel application.

## Variables

### Configuration Location

The path to the root of the Laravel project on the server.

```yaml
laravel_directory: /srv/http/example.com
```

### App

```yaml
laravel_app:
  name: Laravel
  env: local
  key: ~
  debug: yes
  url: http://localhost
```

### Database

```yaml
laravel_db:
  connection: mysql
  host: 127.0.0.1
  port: 3306
  database: laravel
  username: root
  password: secret
```
