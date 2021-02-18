# Release Notes

- [FlexHome 2.18](#version_2_18)
- [FlexHome 2.17](#version_2_17)
- [FlexHome 2.16](#version_2_16)
- [FlexHome 2.15](#version_2_15)
- [FlexHome 2.14](#version_2_14)
- [FlexHome 2.13](#version_2_13)
- [FlexHome 2.12](#version_2_12)
- [FlexHome 2.11](#version_2_11)
- [FlexHome 2.10](#version_2_10)
- [FlexHome 2.9](#version_2_9)
- [FlexHome 2.8](#version_2_8)
- [FlexHome 2.7](#version_2_7)
- [FlexHome 2.6](#version_2_6)
- [FlexHome 2.5](#version_2_5)
- [FlexHome 2.4](#version_2_4)
- [FlexHome 2.3](#version_2_3)
- [FlexHome 2.2](#version_2_2)
- [FlexHome 2.1](#version_2_1)
- [FlexHome 2.0](#version_2_0)
- [FlexHome 1.3](#version_1_3)
- [FlexHome 1.2](#version_1_2)
- [FlexHome 1.1](#version_1_1)
- [FlexHome 1.0](#version_1_0)

## FlexHome 2.18
### Feb 18, 2021
- Update screenshot & allow display shortcode in career page.
- Allow to insert youtube video in the property's detail.
- Improve page SEO meta.
- Improve breadcrumbs.
- Fix search box.
- Fix projects page.
- Fix bug on Location plugin when country/state disabled.
- Fix Custom CSS.
- Fix bug Editor on PHP 8.
- Refactor code & improve queries for better performance.

## FlexHome 2.17
### Feb 04, 2021
- Upgraded to Laravel 8.
- Update JS/CSS assets.
- Allow to config thousands & decimal separators.
- Add username in the registration form.
- Improve admin language settings.
- Improve permalinks.
- Prevent access Ajax URLs.
- Fix language plugin.
- Fix bug locale & account's username.
- Fix missing pagination in careers page
- Fix bugs on PHP 8.
- Refactor code & optimize UI.

## FlexHome 2.16
### Jan 13, 2021
- Add wishlist (favorites properties).
- Add RSS feed for posts [https://flex-home.botble.com/feed/posts](https://flex-home.botble.com/feed/posts) and properties [https://flex-home.botble.com/feed/properties](https://flex-home.botble.com/feed/properties)
- Count number of images for each property https://prnt.sc/wma0e7.
- Improve contact form.
- Fix bug on add/edit property (rent/sale option).
- Fix save facilities.
- Remove unused CSS/JS to make site loads faster.
- Update translations.

## FlexHome 2.15
### Dec 10, 2020
- Add multi-currency.
- Add advanced search on the homepage.
- Add sort properties on the properties page.
- Improve contact page.
- Improve responsive.
- Update translations, added missing keys.
- Improve DO Spaces integration.
- Fix roles & permissions.
- Optimize page speed and performance.

## FlexHome 2.14
### Nov 14, 2020
- Update menu: optimize queries, cache menu URL for better performance.
- Optimize queries on menu & widgets.
- Update Cookie consent: Add option to change background color, text color.
- Update error pages, make it more beautiful.
- Update UI contact form.
- Improve permalink & custom CSS page.
- Improve Analytics plugin, make it compatible with PHP 7.4.
- Fix UI homepage search box on mobile.
- Fix theme translations: new keys in English doesn't show in other languages.
- Fix IP in activity logs, allow IP v6.
- Refactor code.

## FlexHome 2.13
### Oct 27, 2020
- Add RTL support.
- Fix error when activating plugin Real Estate.
- Fix upload images in vendor dashboard.
- Fix bug update facility distances.
- Update missing translations.
- Improve UI homepage search box.
- Improve performance.


## FlexHome 2.12
### Oct 14, 2020
- Add filter by location.
- Add export properties/projects to csv, excel.
- Fix multi-language with Ajax.
- Fix views count.
- Fix properties table.
- Fix save property's facilities.
- Update permissions config.
- Update email encryption settings.
- Improve Recaptcha: add an option to hide v3 badge.
- Improve payment via PayPal.
- Improve export posts to csv, excel.
- Improve theme UI.
- Refactor code.

## FlexHome 2.11
### 15-09-2020
- Update to Laravel version 7.28
- Merge plugin Vendor into plugin Real Estate.
- Support chunk upload in agent dashboard.
- Add agent page. Ex: https://flex-home.botble.com/agents/randy-koelpin-5
- Add Distance key between facilities.
- Update homepage & blog page settings. Now, it's moved into Appearance -> Theme options.
- Move settings for Cookie Consent into Appearance -> Theme options.
- Add settings for watermark. Now, you can add watermark by changing setting in Admin -> Settings -> Media.
- Allow to change permalink in Admin -> Settings -> Permalinks.
- Add language settings. Allow to set default language in Admin -> Settings -> General.
- Allow admin to login using email or username.
- Optimize queries to make site loads faster.
- Update UI.
- Refactor code.
- Fix duplicate settings.
- Fix responsive in agent dashboard.
- Fix UI social login buttons.
- Fix webpack.mix.js config, issue with path on Windows.
- Fix assets path.
- Fix copy folder in Admin -> Media.

## FlexHome 2.10
### 05-08-2020
- Upgrade to the latest Laravel framework version 7.22.
- Deprecated some media functions: `is_image`, `get_image_url`, `get_object_image`, `rv_media_handle_upload`. 
  Replacements: `RvMedia::isImage()`, `RvMedia::getImageUrl()`, `RvMedia::handleUpload()`.
- Add support **Digital Ocean Spaces**.
- Fix timezone, it doesn't work before.
- Fix filter posts.
- Update email settings. Add support **SES**, **Postmark**, **Array**, **Log**.
- Improve performance & refactor source code.
- Improve license system, make it works better.
- Add **Razorpay** & **Paystack** payment gateways. 
    Notes: 
        - You need to go to Admin -> Plugins and activate plugin **Razorpay** & **Paystack** if you want to use it. 
        - Go to Admin -> Payment -> Payment Methods to setup API keys. 
        - If you don't want to use it, you can deactivate or remove that plugins in Admin -> Plugins.
        - Razorpay just displays on checkout page if your amount < ₹5,00,000 (Check maximum payment amount here: https://razorpay.com/docs/payment-pages/faqs)
        - Paystack payment method just displays on checkout page if your currency is NGN https://prnt.sc/ttlcqz


<a name="version_2_9"></a>
## FlexHome 2.9
### 03-07-2020

- Update to the latest Laravel version 7.18.
- Optimize database queries.
- Add support Recaptcha v3.
- Improve cookie consent.
- Fix bugs plugin Language.
- Add default open graph image.
- Improve admin UI.
- Refactor code.

<a name="version_2_8"></a>
### 29-05-2020

- Update to the latest Laravel version 7.13.
- Fix bug on "Properties by locations" shortcode.
- Improve media module: support upload chunk size.
- Improve email system.
- Upgrade jQuery to v3.5.1 and Bootstrap 4.5.0.
- Improve admin UI.
- Refactor code.

<a name="version_2_7"></a>
### 01-05-2020

- Update to the latest Laravel version 7.8.
- Refactor code & optimize performance.
- Add backup commands:
    - php artisan cms:backup:create
    - php artisan cms:backup:restore
    - php artisan cms:backup:remove
    - php artisan cms:backup:list
- Fix image's watermark.
- Change default avatar, remove Gravatar as default avatar.
- Fix widget & plugin language.
- Remove package `davejamesmiller/laravel-breadcrumbs`, build own breadcrumbs.
- Fix theme options when using `editor` field.

<a name="version_2_6"></a>
### 2020-03-28
- Display the property's status. Allow sold, rented properties to show on the homepage.
- Allow free plan packages. Now, new users can get 1 credit for free.
- Allow changing theme primary color.
- Fix search properties, projects.
- Improve performance & clean source code.
- Update to the latest Laravel version 7.3

<a name="version_2_5"></a>
### 2020-03-12
- Upgrade to Botble CMS v5.2 (using Laravel framework 7.x)
- Improve theme UI.
- Update payment, vendor, real-estate plugin.
- Refactor code.

<a name="version_2_4"></a>
### 2020-02-08
- Improve theme UI.
- Update payment plugin.
- Fix bug when searching properties in the admin panel.
- Fix consult email template.
- Fix installer package.
- Refactor code.

<a name="version_2_3"></a>
### 2020-01-20
- Add translation plugin to allow administrators translate site from admin panel.
- Update ckeditor to allow to add image's caption.
- Fix ACL module.
- Add license.

<a name="version_2_2"></a>
### 2020-01-12
- Fix update member's avatar & settings.
- Change property types to categories.
- Add filter by category in search box.
- Optimize source code.

<a name="version_2_1"></a>
### 2020-01-08
- Added property/project types. Ex: Condo, Apartment, Villa, Land...

<a name="version_2_0"></a>
### 2020-01-06

- Added agency with subscription feature.
- Added social login.
- Added payment gateway (PayPal & Stripe).
- Added REST API.
- Update UI.
- Update the latest code from Laravel framework.
- Optimize source code.

<a name="version_1_3"></a>
### 2019-12-14

- Update UI: using VueJS to render blocks.
- Update missing sitemap /sitemap.xml
- Upgrade to the latest Laravel version 6.7.

<a name="version_1_2"></a>
### 2019-12-09
- Fix installer tool.
- Update theme options.
- Add breadcrumb.
- Add cookie consent.

<a name="version_1_1"></a>
### 2019-12-07
    - Improve UI.
    - Improve dev tools packages.
    - Add advanced search into Properties, Projects page.

<a name="version_1_0"></a>
### 2019-12-03
    - Initial release version 1.0
