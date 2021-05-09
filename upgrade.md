# Upgrade Guide

- [Upgrade to FlexHome 2.23](#version_2_23)
- [Upgrade to FlexHome 2.22](#version_2_22)
- [Upgrade to FlexHome 2.21](#version_2_21)
- [Upgrade to FlexHome 2.20](#version_2_20)
- [Upgrade to FlexHome 2.19](#version_2_19)
- [Upgrade to FlexHome 2.18](#version_2_18)
- [Upgrade to FlexHome 2.17](#version_2_17)
- [Upgrade to FlexHome 2.16](#version_2_16)
- [Upgrade to FlexHome 2.15](#version_2_15)
- [Upgrade to FlexHome 2.14](#version_2_14)
- [Upgrade to FlexHome 2.13](#version_2_13)
- [Upgrade to FlexHome 2.12](#version_2_12)
- [Upgrade to FlexHome 2.11](#version_2_11)
- [Upgrade to FlexHome 2.10](#version_2_10)
- [Upgrade to FlexHome 2.9](#version_2_9)
- [Upgrade to FlexHome 2.8](#version_2_8)
- [Upgrade to FlexHome 2.7](#version_2_7)
- [Upgrade to FlexHome 2.6](#version_2_6)
- [Upgrade to FlexHome 2.5](#version_2_5)
- [Upgrade to FlexHome 2.4](#version_2_4)
- [Upgrade to FlexHome 2.3](#version_2_3)
- [Upgrade to FlexHome 2.2](#version_2_2)
- [Upgrade to FlexHome 2.1](#version_2_1)
- [Upgrade to FlexHome 2.0](#version_2_0)
- [Upgrade to FlexHome 1.3](#version_1_3)
- [Upgrade to FlexHome 1.2](#version_1_2)
- [Upgrade to FlexHome 1.1](#version_1_1)

<a name="version_2_23"></a>
## Upgrade to version 2.23

>  {warning} This version requires PHP >= 7.3, make sure your hosting support PHP 7.3 or higher.

- For developers:
  - Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan migrate` to update database.
  - Run `php artisan optimize:clear` to clear cache.

- For non-developers:
  - Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Plugins then deactivate plugin Payment and Real Estate then re-activate it.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
  
<a name="version_2_22"></a>
## Upgrade to version 2.22

>  {warning} This version requires PHP >= 7.3, make sure your hosting support PHP 7.3 or higher.

- For developers:
  - Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan migrate` to update database.
  - Run `php artisan optimize:clear` to clear cache.

- For non-developers:
  - Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Plugins then deactivate plugin Payment and Real Estate then re-activate it.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.

>  {warning} To show properties on maps, you will need to update property's latitude and property's longitude in property editing page.
  
<a name="version_2_21"></a>
## Upgrade to version 2.21

>  {warning} This version requires PHP >= 7.3, make sure your hosting support PHP 7.3 or higher.

- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.

- For developers:
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan migrate` to update database.
  - Run `php artisan optimize:clear` to clear cache.

- For non-developers:
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Plugins then deactivate plugin Payment and Real Estate then re-activate it.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
  
<a name="version_2_20"></a>
## Upgrade to version 2.20

>  {warning} This version requires PHP >= 7.3, make sure your hosting support PHP 7.3 or higher.

- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.

- For developers:
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan migrate` to update database.
  - Run `php artisan optimize:clear` to clear cache.

- For non-developers:
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
  
<a name="version_2_19"></a>
## Upgrade to version 2.19

>  {warning} This version requires PHP >= 7.3, make sure your hosting support PHP 7.3 or higher.

- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.

- For developers:
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan optimize:clear` to clear cache.
  - Go to Admin -> Plugins and activate the plugin SslCommerz Payment Gateway to use it.

- For non-developers:
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
  - Go to Admin -> Plugins and activate the plugin SslCommerz Payment Gateway to use it.
  
<a name="version_2_18"></a>
## Upgrade to version 2.18

>  {warning} This version requires PHP >= 7.3, make sure your hosting support PHP 7.3 or higher.

- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.

- For developers:
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan optimize:clear` to clear cache.

- For non-developers:
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
  
<a name="version_2_17"></a>
## Upgrade to version 2.17

>  {warning} This version requires PHP >= 7.3, make sure your hosting support PHP 7.3 or higher.

- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `public/index.php` from the latest version.

- For developers:
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan optimize:clear` to clear cache.

- For non-developers:
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.

<a name="version_2_16"></a>
## Upgrade to version 2.16
- Override folder `app`, `config`, and `platform` from the latest version.

- For developers:
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan optimize:clear` to clear cache.

- For non-developers:
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
  
- Go to Admin -> Plugins and activate plugin RSS Feed.

<a name="version_2_15"></a>
## Upgrade to version 2.15
- Override folder `app`, `config`, and `platform` from the latest version.

- For developers:
  - Update file `composer.json` and `composer.lock` from new source code.
  - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
  - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
  - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
  - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
  - Run `php artisan optimize:clear` to clear cache.

- For non-developers:
  - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
  - Delete all files in `storage/framework/views` and `storage/framework/cache`.
  - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
  - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.

- Important changes: 
  - If you have customized Flex Home theme source code, you need to make sure is updated. Function `getIndex()` and `getView()` are deleted in `platform/themes/flex-home/src/Http/Controllers/FlexHomeController.php`.
  

<a name="version_2_14"></a>
## Upgrade to version 2.14
- Override folder `app`, `config`, and `platform` from the latest version.

- For developers:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
    - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
    - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
    - Run `php artisan optimize:clear` to clear cache.
    
- For non-developers:
    - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
    - Delete all files in `storage/framework/views` and `storage/framework/cache`.
    - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
    - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.
    
<a name="version_2_13"></a>
## Upgrade to version 2.13
- Override folder `app`, `config`, and `platform` from the latest version.

- For developers:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
    - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
    - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
    - Run `php artisan optimize:clear` to clear cache.
    
- For non-developers:
    - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
    - Delete all files in `storage/framework/views` and `storage/framework/cache`.
    - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
    - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.
    
<a name="version_2_12"></a>
## Upgrade to version 2.12
- Override folder `app`, `config`, and `platform` from the latest version.

- For developers:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Delete folder `public/vendor` and run command `php artisan vendor:publish --tag=cms-public --force`
    - Delete folder `public/themes` and run command `php artisan cms:theme:assets:publish`
    - Run command `php artisan vendor:publish --tag=cms-lang --force` to update translations.
    - Run `php artisan optimize:clear` to clear cache.
    
- For non-developers:
    - Override folder `public/themes`, `public/vendor`, `bootstrap`, `vendor` from the latest version.
    - Delete all files in `storage/framework/views` and `storage/framework/cache`.
    - Go to Admin -> Translations -> Admin translations then click on `Import group` to update translations.
    - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.
    
<a name="version_2_11"></a>
## Upgrade to version 2.11
- Delete folder `platform/plugins/vendor`.
- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `resources` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Override folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate, Career then re-activate it.
    
<a name="version_2_10"></a>
## Upgrade to version 2.10
- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `resources` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
<a name="version_2_9"></a>
## Upgrade to version 2.9
- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `resources` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Override folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate, Vendor, Payment, Location then re-activate it.
    
<a name="version_2_8"></a>
## Upgrade to version 2.8
- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `resources` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Override folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate, Vendor, Payment, Location then re-activate it.
    
<a name="version_2_7"></a>
## Upgrade to version 2.7
- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `resources` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Override folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate, Vendor, Payment, Location then re-activate it.
    
<a name="version_2_6"></a>
## Upgrade to version 2.6
- Override folder `app`, `config`, `platform`, `public/themes`, `public/vendor` and `resources` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Override folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate, Vendor, Payment, Location then re-activate it.

<a name="version_2_5"></a>
## Upgrade to version 2.5
- Override folder `app`, `config`, `platform`, `public/themes` and `public/vendor` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Override folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate, Vendor, Payment then re-activate it.
    
<a name="version_2_4"></a>
## Upgrade to version 2.4
- Override folder `app`, `platform`, `public/themes` and `public/vendor` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Override folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate, Vendor, Payment then re-activate it.
    
<a name="version_2_3"></a>
## Upgrade to version 2.3
- Override folder `app`, `platform`, `public/themes` and `public/vendor` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Override folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.

<a name="version_2_2"></a>
## Upgrade to version 2.2
- Override folder `platform`, `public/themes` and `public/vendor` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.
    
<a name="version_2_1"></a>
## Upgrade to version 2.1
- Override folder `platform/plugins/real-estate`, `resources/lang/vendor`, `platform/themes/real-estate`

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.

<a name="version_2_0"></a>
## Upgrade to version 2.0

- Override folder `app`, `platform`, `public/themes` and `public/vendor` from the latest version.

- For developer:
    - Update file `composer.json` and `composer.lock` from new source code.
    - Delete folder `/vendor` then run `composer install` to upgrade vendor packages.
    - Run `php artisan migrate` to update database.
    
- For non-developer:
    - Update folder `/vendor` from the latest version.
    - Go to Admin -> Plugins then deactivate plugin Real Estate then re-activate it.
    
- Go to admin and activate plugins: Social Login, Vendor, Payment.

<a name="version_1_3"></a>
## Upgrade to version 1.3
- Override folder `platform`, `public/themes`, `public/vendor` and `vendor` from version 1.3.
- Run command `php artisan migrate` to update database or change column `images` in table `re_properties` & `re_projects` to `TEXT`

![Update images field](./images/fix-images-field.png)

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
