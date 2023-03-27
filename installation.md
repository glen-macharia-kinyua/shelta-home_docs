# Introduction

* [Requirement](installation.md#requirement)
* [Installation](installation.md#installation)
* [Note](installation.md#note)

## Requirement

* Apache, nginx, or another compatible web server.
* PHP >= 8.0.2 >> Higher
* MySQL Database server
* BCMath PHP Extension
* Ctype PHP Extension
* Fileinfo PHP extension
* JSON PHP Extension
* Mbstring PHP Extension
* OpenSSL PHP Extension
* PDO PHP Extension
* Tokenizer PHP Extension
* XML PHP Extension
* Module Re\_write server
* PHP\_CURL Module Enable

## PHP Configuration

Open your php configuration file php.ini and change the following settings.

```bash
memory_limit = 128M
max_execution_time = 300
```

If you are using Cpanel, you can follow this article to change your PHP memory limit settings https://chemicloud.com/kb/article/how-to-increase-the-php-memory-limit-in-cpanel/

> {warning} On this project, we're using the latest Laravel version (currently 8.x). Please go to [Laravel documentation page](https://laravel.com/docs) for more information.

> It’s based on Laravel framework, the root folder for it is /public. You shouldn’t install it on a sub-folder, use sub-domain is better than sub-folder. (we won’t support to install our product on sub-folder).

## Install on hosting

> {warning} If you're a Laravel developer and you want to customize our source code in `platform/core` and `platform/packages`, you need to delete folder `/vendor` then run command `composer install` to reinstall vendor packages.

* Upload all files into the root folder of your hosting (normally, it is`public_html`).
* Create a database and import data from `database.sql` (it's located in source code).
* Update your database credentials and `APP_URL` in `.env`
* Go to `/admin` to access to admin panel.
* The default admin account is noah.  password = 12345678

## Install locally or in VPS

> {warning} If you're a Laravel developer and you want to customize our source code in `platform/core` and `platform/packages`, you need to delete folder `/vendor` then run command `composer install` to reinstall vendor packages.

* Update your database credentials and `APP_URL` in `.env`.
* Using sample data:
  * Import database from `database.sql`.
* Don't use sample data:
  * Run `php artisan migrate` to create database structure.
  * Run `php artisan cms:user:create` to create admin user.
  * Run `php artisan cms:theme:activate flex-home`
* If you're pulled source code from GIT server:
  * Run `php artisan vendor:publish --tag=cms-public --force`
  * Run `php artisan cms:theme:assets:publish`
* Run web locally:
  * Change `APP_URL` in `.env` to `APP_URL=http://localhost:8000`
  * Run `php artisan serve`. Open `http://localhost:8000`, you should see the homepage.
  * Go to `/admin` to access to admin panel.
  * If you're using sample data, the default admin account is `botble` - `159357`.
  * If you don't use sample data, you need to go to Admin -> Plugins then activate all plugins.

## Setup cron job

Cron job used to renew properties automatically when it's expired. You can ignore this step if you don't need that feature.

```bash
* * * * * /usr/local/bin/php /path-to-your-project/artisan schedule:run >> /dev/null 2>&1
```

Setup cron job in cPanel: https://www.youtube.com/watch?v=t5mjWGegE-g
