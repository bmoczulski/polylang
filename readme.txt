=== Polylang ===
Contributors: Chouby, manooweb, raaaahman, marianne38, sebastienserre
Donate link: https://polylang.pro
Tags: multilingual, bilingual, translate, translation, language, multilanguage, international, localization
Requires at least: 5.1
Tested up to: 5.7
Requires PHP: 5.6
Stable tag: 3.0.2
License: GPLv3 or later
License URI: https://www.gnu.org/licenses/gpl-3.0.html

Making WordPress multilingual

== Description ==

= Features  =

Polylang allows you to create a bilingual or multilingual WordPress site. You write posts, pages and create categories and post tags as usual, and then define the language for each of them. The translation of a post, whether it is in the default language or not, is optional.

* You can use as many languages as you want. RTL language scripts are supported. WordPress languages packs are automatically downloaded and updated.
* You can translate posts, pages, media, categories, post tags, menus, widgets...
* Custom post types, custom taxonomies, sticky posts and post formats, RSS feeds and all default WordPress widgets are supported.
* The language is either set by the content or by the language code in url, or you can use one different subdomain or domain per language
* Categories, post tags as well as some other metas are automatically copied when adding a new post or page translation
* A customizable language switcher is provided as a widget or in the nav menu

> The author does not provide support on the wordpress.org forum. Support and extra features are available to [Polylang Pro](https://polylang.pro) users.

If you wish to migrate from WPML, you can use the plugin [WPML to Polylang](https://wordpress.org/plugins/wpml-to-polylang/)

If you wish to use a professional or automatic translation service, you can install [Lingotek Translation](https://wordpress.org/plugins/lingotek-translation/), as an addon of Polylang. Lingotek offers a complete translation management system which provides services such as translation memory or semi-automated translation processes (e.g. machine translation > human translation > legal review).

= Credits =

Thanks a lot to all translators who [help translating Polylang](https://translate.wordpress.org/projects/wp-plugins/polylang).
Thanks a lot to [Alex Lopez](http://www.alexlopez.rocks/) for the design of the logo.
Most of the flags included with Polylang are coming from [famfamfam](http://famfamfam.com/) and are public domain.
Wherever third party code has been used, credit has been given in the code’s comments.

= Do you like Polylang? =

Don't hesitate to [give your feedback](http://wordpress.org/support/view/plugin-reviews/polylang#postform).

== Installation ==

1. Make sure you are using WordPress 5.1 or later and that your server is running PHP 5.6 or later (same requirement as WordPress itself)
1. If you tried other multilingual plugins, deactivate them before activating Polylang, otherwise, you may get unexpected results!
1. Install and activate the plugin as usual from the 'Plugins' menu in WordPress.
1. Go to the languages settings page and create the languages you need
1. Add the 'language switcher' widget to let your visitors switch the language.
1. Take care that your theme must come with the corresponding .mo files (Polylang automatically downloads them when they are available for themes and plugins in this repository). If your theme is not internationalized yet, please refer to the [Theme Handbook](https://developer.wordpress.org/themes/functionality/internationalization/) or ask the theme author to internationalize it.

== Frequently Asked Questions ==

= Where to find help ? =

* First time users should read [Polylang - Getting started](https://polylang.pro/doc-category/getting-started/), which explains the basics with a lot of screenshots.
* Read the [documentation](https://polylang.pro/doc/). It includes a [FAQ](https://polylang.pro/doc-category/faq/) and the [documentation for developers](https://polylang.pro/doc-category/developers/).
* Search the [community support forum](https://wordpress.org/search/). You will probably find your answer here.
* Read the sticky posts in the [community support forum](http://wordpress.org/support/plugin/polylang).
* If you still have a problem, open a new thread in the [community support forum](http://wordpress.org/support/plugin/polylang).
* [Polylang Pro](https://polylang.pro) users have access to our helpdesk.

= Is Polylang compatible with WooCommerce? =

* You need a separate addon to make Polylang and WooCommerce work together. [A Premium addon](https://polylang.pro/downloads/polylang-for-woocommerce/) is available.

= Do you need translation services? =

* If you want to use professional or automatic translation services, install and activate the [Lingotek Translation](https://wordpress.org/plugins/lingotek-translation/) plugin.

== Screenshots ==

1. The Polylang languages admin panel
2. The Strings translations admin panel
3. Multilingual media library
4. The Edit Post screen with the Languages metabox

== Changelog ==

= 3.0.2 (2021-03-16) =

* Move hreflang attributes higher in the head section #771
* Fix custom flags not working (introduced in 3.0)
* Fix translation of the confirmation modal when changing the language of a post
* Fix js and css not loaded when Polylang is used as a mu-plugin ((introduced in 3.0))
* Fix support for html5 stylesheet link tags #775
* Fix possible warning in frontend-filters-links.php
* Yoast SEO Premium: Take over the multilingual compatibility removed in Yoast SEO Premium 15.8 #796
* Yoast SEO: Fix CPT breadcrumb title when the option is left empty #794
* Yoast SEO: Fix sitemap.xml not redirected on secondary domains #789

= 3.0.1 (2021-03-10) =

* Fix media gallery messed when editing a post in the classic editor
* Fix missing script dependency on old WP versions
* Fix CSS conflict with WooCommerce Bookings for WP < 5.6
* Fix conflict resulting in '__' already defined in block-editor.js. #779
* Fix search form removed for some themes. Props Marián Kadaňka. #780
* Fix fatal error with very old versions of Yoast SEO. Props Nicola Peluchetti. #781

= 3.0 (2021-03-08) =

* Add compatibility with WordPress 5.7
* Remove upgrades from Polylang older than 1.8
* Remove deprecated class PLL_Pointer
* Pro: Hide the license keys
* Pro: Fix redirect to the home page of a deactivated language
* Pro: Fix synchronization of post status not working
* Pro: Fix language switcher block not working in a post retrieved in REST API
* Pro: Fix PO export of strings with line breaks
* Pro: Fix file block title customization lost
* Add a dialog box to ask a confirmation about a language change in classic and block editors
* Improve browser language detection #591
* Improve robustness and documentation of code
* Fix media library after the language has been chnaged in the editor metabox
* Fix duplicated title attribute on flag link in posts list
* Fix legacy block editor language metabox compatibility with WordPress 5.6
* Fix uploaded theme and plugin files in media library
* Fix site title not translated in email change confirmation email
* Fix remaining deprecated jQuery notices #741
* Fix compatibility with GN publisher
* Fix compatibility with Woodmart theme search form
* Fix compatibility issue with 3rd party ajax requests since jQuery 3.3 #744
* Fix CSS conflict with WooCommerce Bookings
* Fix browser error when displaying an embed and using a cache plugin #757
* Fix post type archive title and metadesc not translated in Yoast SEO
* Fix PHP notice in REST API

= 2.9.2 (2021-02-02) =

* Pro: Fix translation of CPTUI plural label and description not working
* Add Spanish (Ecuador) to the list of predefined languages
* Fix typo in "WordPress" string translation group. Props Viktor Szépe #682

= 2.9.1 (2020-12-15) =

* Fix PHP notice: Undefined property: PLL_Cache_Compat::$options with cache plugins. Props bahaa-almahamid. #658
* Fix title of the search results page with Yoast SEO > 14.0

= 2.9 (2020-12-07) =

* Add compatibility with WordPress 5.6
* Pro: Add locale fallback used when the theme or plugins translations are not available
* Pro: Fix SSO and browser preferred language redirect when using multiple domains
* Pro: Fix post slugs for German and Danish in the REST API
* Pro: Fix a fatal error in ACF integration when saving url modifications with multiple domains
* Pro: Fix a deprecated notice fired by ACF since the version 5.9.2
* Pro: Fix ACF relationship fields not reloaded when changing the language in the classic editor
* Update plugin updater to version 1.8
* Add Lower Sorbian to the list of predefined language
* Options are now translated on backend when using the admin language filter
* Keep previous translations when modifying an option value
* Add navigation markup to the language switcher widget
* Fix canonical redirect for taxonomy terms
* Fix a fatal error when deleting a post with a translation group corrupted in the database
* Fix a fatal error when switching to plain permalinks and using multiple domains
* Fix a conflict with WP Sweep which could corrupt languages
* Fix title displayed instead of meta description with Yoast SEO > 14.0
* Fix PHP Notice: Undefined index: wp_the_query in /frontend/choose-lang-content.php on line 92

See [changelog.txt](https://plugins.svn.wordpress.org/polylang/trunk/changelog.txt) for older changelog
