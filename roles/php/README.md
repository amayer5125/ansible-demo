# PHP

This role installs php-fpm and php-cli from [Remi's Repository](https://rpms.remirepo.net/). It also ensures php-fpm is enabled and started.

By default this role installs all the php modules required to run [Laravel](https://laravel.com/docs/7.x#server-requirements).

## Variables

### PHP Packages

You may override the php_packages that are installed.

```yml
php_packages:
  - php-bcmath
  - php-cli
  - php-common
  - php-fpm
  - php-gd
  - php-json
  - php-mbstring
  - php-mysqlnd
  - php-pdo
  - php-xml
```
