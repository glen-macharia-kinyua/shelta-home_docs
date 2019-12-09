# Upgrade Guide

- [Upgrade to FlexHome 1.2](#version_1_2)
- [Upgrade to FlexHome 1.1](#version_1_1)

<a name="version_1_2"></a>
## Upgrade to version 1.2

- Override folder `/platform` from new source code.
- Update file `composer.json` and `composer.lock` from new source code.
- Delete folder `/vendor` then run `composer install` to upgrade vendor packages
- Run `php artisan vendor:publish --tag=cms-public --force` to update assets.
- Run `php artisan cms:theme:assets:publish` to update theme.

<a name="version_1_1"></a>
## Upgrade to version 1.1

- Override folder `/platform` from new source code.
- Update file `composer.lock` from new source code.
- Delete folder `/vendor` then run `composer install` to upgrade vendor packages
- Run `php artisan vendor:publish --tag=cms-public --force` to update assets.
- Run `php artisan cms:theme:assets:publish` to update theme.
