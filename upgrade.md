# Upgrade Guide

- [Upgrade to FlexHome 1.1](#version_1_1)

<a name="version_1_1"></a>
## Upgrade to version 1.1

- Override folder `/platform` from new source code.
- Run `php artisan vendor:publish --tag=cms-public --force` to update assets.
- Run `php artisan cms:theme:assets:publish` to update theme.
