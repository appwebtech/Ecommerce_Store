<div align="center">
<h1>E-Commerce Website</h1> 
<h2>Synopsis of Software Development</h2>
  <h3>
    <a href="https://en.wikipedia.org/wiki/WordPress">
      Wordpress
    </a>
  </h3>
</div>

<div align="center">
  <sub>Developed and Designed by
  <a href="#">Joseph M Mwania</a> for
  <a href="#http://theappwebtech.com">
    Appwebtech
  </a>
</div>

<h2>Table of Contents</h2>
<details>
- [Introduction](#introduction)
- [Why Wordpress](#why-wordpress)
- [Technical Requirements](#technical-requirements)
  - [WooCommerce](#woocommerce)
  - [Akismet](#akismet)
  - [Slider Revolution](#slider-revolution)
  - [WP Super Cache](#wp-super-cache)
  - [YITH WooCommerce Wishlist](#yith-woocommerce-wishlist)
  - [Deployment instructions](#deployment-instructions)
  - [Developer](#developer)
  - [Contacts](#contacts)
</details>

# Introduction

Chances are that if you have landed on this page via Google searching for CMS platforms and open-source developers, then you already have heard of Wordpress and lucky you because here you got both. An open-source fanatic with a documented code. 

Firstly, I would like to point out that code, whether basic or sophisticated like a mixture of Lisp and Intercal, it should bear documentation if it so happens that an application is built from it. All this hype from programmers online hangouts that (**Real programmers don't document their programs. Documentation is for simpletons who can't read listings or the object code from dumps**) doesn't make sense if someone is engaging with clients who want to know how their software works. 

Secondly, this documentation is not written to learn how to use the website. Everyone at this age and time can browse a website and download or purchase stuff online. This is a brief synopsis of how I created the software and with what technologies. Important! I get requested for it a lot by nontechnicals, but I still stand with Eric S. Raymond's quote. *if they have to read documentation to use it you designed it wrong.*  

Since it's release in 2003, Wordpress has evolved tremendously and now has become one of the best web technologies in building websites. 
At the time of writing, Wordpress powers close to 75 million websites. So what is it? 

Wordpress is an open-source [Content Management System (CMS)](https://en.wikipedia.org/wiki/WordPress) that uses [Hypertext Preprocessor (PHP)](https://en.wikipedia.org/wiki/PHP) for its BackEnd (server-side) system and [MySQL](https://en.wikipedia.org/wiki/MySQL) to manage it's databases (DB). PHP is a server-side scripting language which is amazing in web development; this is due to it's flexibility to be embedded in [HTML](https://en.wikipedia.org/wiki/HTML), more or less the way [Ruby](https://en.wikipedia.org/wiki/Ruby_on_Rails) is embedded in Rails. PHP is very versatile and compatible across many browsers, web servers and operating systems. The preference of using it for server-side systems has grown and will continue due to it's de-facto pro-bono policy. Same applies to MySQL.

Wordpress uses MySQL to manage it's DB's. MySQL is an RDBMS and most of it's functionalities are open-source. It's a main component of [LAMP](https://en.wikipedia.org/wiki/LAMP_(software_bundle)) open-source web application software stack. 

Below is a snapshot of the DB I used. It can be queried, searched and exported to other servers. That is the main reason I used SoC to have a reputable external source to process payments. Actually, [WooCommerce](https://woocommerce.com/) will not process payments but will direct them to be processed by [Paypal](https://www.paypal.com/). If at all a black hat hacker can for some reason gain access to the DB, they would just steal merchandise listing (Irrelevant to a hacker). The ISP, the vendor and the developer would by no means have any customer payment data stored in the DB and thus exonerating them from any liability.
<hr>
![screen shot 2016-12-20 at 22 02 19](https://cloud.githubusercontent.com/assets/20464709/21368093/2f56400c-c701-11e6-8478-94f896af7aa2.png)
<hr>

There are a myriad of reason as to why I love using open-source software in design and development. Compelling advatanges gravitate towards the following factors which are quite intuitive;
* Security
* Customizability
* Freedom
* Auditability
* Ready Support (Bug fixes are timely)
* Try and discard if you dont like.
* Quality etc etc


# Why Wordpress?

Wordpress is great in building almost any website. A developer can design a theme and sell to whomever wants to buy, eg [themeforest](https://themeforest.net/search?utf8=%E2%9C%93&term=ecommerce&as=0&referrer=homepage), etc. Themes vary from free downloadables to a cost that would vary from  $2, see [here](https://themeforest.net/item/sketch-and-css-bridging-the-gap/15284085?s_rank=1) up to a cost way beyond $999, like  [this](https://themeforest.net/item/fightclub-fight-fitness-club-psd-template/12237033?s_rank=17). It all depends realy on what your website entails, your target audience, security features, design, etc. 

An e-commerce website like this one I've developed would fetch between $ 5000 and  $ 10,000 on the current market trend, without much subsequent support. Usually a three month follow-up is reasonable with a maximum of three free edits, free server maintenace, DB upgrades etc which takes me to the next point. 

The reason as to why I chose wordpress for an e-commerce store is to give the client some liberty in managing the store themselves. With Wordpress, it's easy to add merchandise, change prices, offers and other basic functionalities which the client can do without calling the developer to do it for them. Our policy is to keep prices down and afordable for everyone. That extra dollar which would have been spend in website maintenance can act as a Marginal Propensity to Consume (MPC) for the client and thus be diverted for some nice stuff like charity work. 

# Technical Requirements


## WooCommerce

An e-commerce that helps in processing of online payments. it does more by managing the delivery of emails to clients, generating invoices etc. 

### [WooCommerce](https://woocommerce.com/) [![Built with Grunt](https://cdn.gruntjs.com/builtwith.png)](http://gruntjs.com/) [![Build Status](https://travis-ci.org/woocommerce/woocommerce.svg?branch=master)](https://travis-ci.org/woocommerce/woocommerce) [![Code Coverage](https://scrutinizer-ci.com/g/woocommerce/woocommerce/badges/coverage.png?b=master)](https://scrutinizer-ci.com/g/woocommerce/woocommerce/?branch=master) [![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/woocommerce/woocommerce/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/woocommerce/woocommerce/?branch=master) [![Code Climate](https://codeclimate.com/github/woocommerce/woocommerce/badges/gpa.svg)](https://codeclimate.com/github/woocommerce/woocommerce)

Welcome to the WooCommerce repository on GitHub. Here you can browse the source, look at open issues and keep track of development. We recommend all developers to follow the [WooCommerce development blog](https://woocommerce.wordpress.com/) to stay up to date about everything happening in the project. You can also [follow @DevelopWC](https://twitter.com/DevelopWC) on Twitter for the latest development updates.

If you are not a developer, please use the [WooCommerce plugin page](https://wordpress.org/plugins/woocommerce/) on WordPress.org.

### Documentation
* [WooCommerce Documentation](https://docs.woocommerce.com/documentation/plugins/woocommerce/)
* [WooCommerce Knowledge Base](https://support.woothemes.com/hc/en-us/categories/200146917-WooCommerce)
* [WooCommerce Code Reference](https://docs.woocommerce.com/wc-apidocs/)
* [WooCommerce REST API Docs](https://woocommerce.github.io/woocommerce-rest-api-docs/)

### Reporting Security issues
To disclose a security issue to our team, [please submit a report via HackerOne here](https://hackerone.com/automattic/).

### Support
This repository is not suitable for support. Please don't use our issue tracker for support requests, but for core WooCommerce issues only. Support can take place in the appropriate channels:

* The [WooThemes premium support portal](https://support.woothemes.com/) for customers who have purchased themes or extensions.
* [Our community forum on wp.org](https://wordpress.org/support/plugin/woocommerce) which is available for all WooCommerce users.

Support requests in issues on this repository will be closed on sight.

### Contributing to WooCommerce
If you have a patch, or stumbled upon an issue with WooCommerce core, you can contribute this back to the code. Please read our [contributor guidelines](https://github.com/woocommerce/woocommerce/blob/master/.github/CONTRIBUTING.md) for more information how you can do this.


## WPGlobus for WPBakery Visual Composer 

**Contributors:** alexgff, tivnetinc, tivnet  
**Donate link:** http://www.wpglobus.com/  
**Tags:** globalization, i18n, international, l10n, visual composer, localization, multilanguage, multilingual, translate, WPGlobus  
**Requires at least:** 4.0  
**Tested up to:** 4.2.3
**Stable tag:** trunk  
**License:** GPLv2
**License URI:** https://github.com/WPGlobus/wpglobus-for-wpbakery-visual-composer/blob/master/LICENSE  

### Description 

**WPGlobus for WPBakery Visual Composer** is an extension to the WPGlobus plugin.

> **NOTE:** You need to install and activate the [WPGlobus Multilingual Plugin](https://wordpress.org/plugins/wpglobus/) version 1.0.14 or later before installing the WPGlobus for WPBakery Visual Composer extension.

#### More info

* [WPGlobus for WPBakery Visual Composer home page](http://www.wpglobus.com/extensions-archive/wpglobus-for-wpbakery-visual-composer-archive/).
* [GitHub code repository](https://github.com/WPGlobus/wpglobus-for-wpbakery-visual-composer).

### Installation 

You can install this plugin directly from your WordPress dashboard:

1. Go to the *Plugins* menu and click *Add New*.
1. Search for *WPGlobus for WPBakery Visual Composer*.
1. Click *Install Now* next to the *WPGlobus for WPBakery Visual Composer* plugin.
1. Activate the plugin.

Alternatively, see the guide to [Manually Installing Plugins](http://codex.wordpress.org/Managing_Plugins#Manual_Plugin_Installation).

### Frequently Asked Questions 

#### How do I contribute to WPGlobus for WPBakery Visual Composer? 

We appreciate all contributions, ideas, critique, and help.

* To speed up our development, please report bugs, with reproduction steps on [WPGlobus for WPBakery Visual Composer GitHub](https://github.com/WPGlobus/wpglobus-for-wpbakery-visual-composer).
* Plugin and theme authors: please try WPGlobus for WPBakery Visual Composer and let us know if you find any compatibility problems.
* Contact us directly on [WPGlobus.com](http://www.wpglobus.com/contact-us/).

#### More info? 

Please check out the [WPGlobus Website](http://www.wpglobus.com/extensions-archive/wpglobus-for-wpbakery-visual-composer-archive/) for additional information.

### Screenshots 

####  Plugin admin interface. 
![Plugin admin interface.](https://raw.githubusercontent.com/WPGlobus/wpglobus-for-wpbakery-visual-composer/master/assets/screenshot-1.png)

### Changelog 

#### 1.0.0 
* Initial release



## Akismet

Used by millions, Akismet is quite possibly the best way in the world to protect your blog from spam. It keeps your site protected even while you sleep. 

```
=== Akismet ===
Contributors: matt, ryan, andy, mdawaffe, tellyworth, josephscott, lessbloat, eoigal, cfinke, automattic, jgs
Tags: akismet, comments, spam, antispam, anti-spam, anti spam, comment moderation, comment spam, contact form spam, spam comments
Requires at least: 3.2
Tested up to: 4.3.1
Stable tag: 3.1.5
License: GPLv2 or later

Akismet checks your comments against the Akismet Web service to see if they look like spam or not.

== Description ==

Akismet checks your comments against the Akismet Web service to see if they look like spam or not and lets you review the spam it catches under your blog's "Comments" admin screen.

Major features in Akismet include:

* Automatically checks all comments and filters out the ones that look like spam.
* Each comment has a status history, so you can easily see which comments were caught or cleared by Akismet and which were spammed or unspammed by a moderator.
* URLs are shown in the comment body to reveal hidden or misleading links.
* Moderators can see the number of approved comments for each user.
* A discard feature that outright blocks the worst spam, saving you disk space and speeding up your site.

PS: You'll need an [Akismet.com API key](http://akismet.com/get/) to use it.  Keys are free for personal blogs; paid subscriptions are available for businesses and commercial sites.

== Installation ==

Upload the Akismet plugin to your blog, Activate it, then enter your [Akismet.com API key](http://akismet.com/get/).

1, 2, 3: You're done!

== Changelog ==

= 3.1.5 =
*Release Date - 13 October 2015*

* Closes a potential XSS vulnerability.

= 3.1.4 =
*Release Date - 24 September 2015*

* Fixed a bug that was preventing some users from automatically connecting using Jetpack if they didn't have a current Akismet subscription.
* Fixed a bug that could cause comments caught as spam to be placed in the Pending queue.
* Error messages and instructions have been simplified to be more understandable.
* Link previews are enabled for all links inside comments, not just the author's website link.

= 3.1.3 =
*Release Date - 6 July 2015*

* Notify users when their account status changes after previously being successfully set up. This should help any users who are seeing blank Akismet settings screens.

= 3.1.2 =
*Release Date - 7 June 2015*

* Reduced the amount of space Akismet uses in the commentmeta table.
* Fixed a bug where some comments with quotes in the author name weren't getting history entries
* Pre-emptive security improvements to ensure that the Akismet plugin can't be used by attackers to compromise a WordPress installation.
* Better UI for the key entry field: allow whitespace to be included at the beginning or end of the key and strip it out automatically when the form is submitted.
* When deactivating the plugin, notify the Akismet API so the site can be marked as inactive.
* Clearer error messages.

= 3.1.1 =
*Release Date - 17th March, 2015*

* Improvements to the "Remove comment author URL" JavaScript
* Include the pingback pre-check from the 2.6 branch.

= 3.1 =
*Release Date - 11th March, 2015*

* Use HTTPS by default for all requests to Akismet.
* Fix for a situation where Akismet might strip HTML from a comment.

= 3.0.4 =
*Release Date - 11th December, 2014*

* Fix to make .htaccess compatible with Apache 2.4.
* Fix to allow removal of https author URLs.
* Fix to avoid stripping part of the author URL when removing and re-adding.
* Removed the "Check for Spam" button from the "Trash" and "Approved" queues, where it would have no effect.
* Allow automatic API key configuration when Jetpack is installed and connected to a WordPress.com account

= 3.0.3 =
*Release Date - 3rd November, 2014*

* Fix for sending the wrong data to delete_comment action that could have prevented old spam comments from being deleted.
* Added a filter to disable logging of Akismet debugging information.
* Added a filter for the maximum comment age when deleting old spam comments.
* Added a filter for the number per batch when deleting old spam comments.
* Removed the "Check for Spam" button from the Spam folder.

= 3.0.2 =
*Release Date - 18th August, 2014*

* Performance improvements.
* Fixed a bug that could truncate the comment data being sent to Akismet for checking.

= 3.0.1 =
*Release Date - 9th July, 2014*

* Removed dependency on PHP's fsockopen function
* Fix spam/ham reports to work when reported outside of the WP dashboard, e.g., from Notifications or the WP app
* Remove jQuery dependency for comment form JavaScript
* Remove unnecessary data from some Akismet comment meta
* Suspended keys will now result in all comments being put in moderation, not spam.

= 3.0.0 =
*Release Date - 15th April, 2014*

* Move Akismet to Settings menu
* Drop Akismet Stats menu
* Add stats snapshot to Akismet settings
* Add Akismet subscription details and status to Akismet settings
* Add contextual help for each page
* Improve Akismet setup to use Jetpack to automate plugin setup
* Fix "Check for Spam" to use AJAX to avoid page timing out
* Fix Akismet settings page to be responsive
* Drop legacy code
* Tidy up CSS and Javascript
* Replace the old discard setting with a new "discard pervasive spam" feature.

= 2.6.0 =
*Release Date - 18th March, 2014*

* Add ajax paging to the check for spam button to handle large volumes of comments
* Optimize javascript and add localization support 
* Fix bug in link to spam comments from right now dashboard widget
* Fix bug with deleting old comments to avoid timeouts dealing with large volumes of comments
* Include X-Pingback-Forwarded-For header in outbound WordPress pingback verifications
* Add pre-check for pingbacks, to stop spam before an outbound verification request is made

= 2.5.9 =
*Release Date - 1st August, 2013*

* Update 'Already have a key' link to redirect page rather than depend on javascript
* Fix some non-translatable strings to be translatable
* Update Activation banner in plugins page to redirect user to Akismet config page

= 2.5.8 =
*Release Date - 20th January, 2013*

* Simplify the activation process for new users
* Remove the reporter_ip parameter
* Minor preventative security improvements

= 2.5.7 =
*Release Date - 13th December, 2012*

* FireFox Stats iframe preview bug
* Fix mshots preview when using https
* Add .htaccess to block direct access to files
* Prevent some PHP notices
* Fix Check For Spam return location when referrer is empty
* Fix Settings links for network admins
* Fix prepare() warnings in WP 3.5

= 2.5.6 =
*Release Date - 26th April, 2012*

* Prevent retry scheduling problems on sites where wp_cron is misbehaving
* Preload mshot previews
* Modernize the widget code
* Fix a bug where comments were not held for moderation during an error condition
* Improve the UX and display when comments are temporarily held due to an error
* Make the Check For Spam button force a retry when comments are held due to an error
* Handle errors caused by an invalid key
* Don't retry comments that are too old
* Improve error messages when verifying an API key

= 2.5.5 =
*Release Date - 11th January, 2012*

* Add nonce check for comment author URL remove action
* Fix the settings link

= 2.5.4 =
*Release Date - 5th January, 2012*

* Limit Akismet CSS and Javascript loading in wp-admin to just the pages that need it
* Added author URL quick removal functionality
* Added mShot preview on Author URL hover
* Added empty index.php to prevent directory listing
* Move wp-admin menu items under Jetpack, if it is installed
* Purge old Akismet comment meta data, default of 15 days

= 2.5.3 = 
*Release Date - 8th Febuary, 2011*

* Specify the license is GPL v2 or later
* Fix a bug that could result in orphaned commentmeta entries
* Include hotfix for WordPress 3.0.5 filter issue

= 2.5.2 =
*Release Date - 14th January, 2011*

* Properly format the comment count for author counts
* Look for super admins on multisite installs when looking up user roles
* Increase the HTTP request timeout
* Removed padding for author approved count
* Fix typo in function name
* Set Akismet stats iframe height to fixed 2500px.  Better to have one tall scroll bar than two side by side.

= 2.5.1 =
*Release Date - 17th December, 2010*

* Fix a bug that caused the "Auto delete" option to fail to discard comments correctly
* Remove the comment nonce form field from the 'Akismet Configuration' page in favor of using a filter, akismet_comment_nonce
* Fixed padding bug in "author" column of posts screen
* Added margin-top to "cleared by ..." badges on dashboard
* Fix possible error when calling akismet_cron_recheck()
* Fix more PHP warnings
* Clean up XHTML warnings for comment nonce
* Fix for possible condition where scheduled comment re-checks could get stuck
* Clean up the comment meta details after deleting a comment
* Only show the status badge if the comment status has been changed by someone/something other than Akismet
* Show a 'History' link in the row-actions
* Translation fixes
* Reduced font-size on author name
* Moved "flagged by..." notification to top right corner of comment container and removed heavy styling
* Hid "flagged by..." notification while on dashboard

= 2.5.0 =
*Release Date - 7th December, 2010*

* Track comment actions under 'Akismet Status' on the edit comment screen
* Fix a few remaining deprecated function calls ( props Mike Glendinning ) 
* Use HTTPS for the stats IFRAME when wp-admin is using HTTPS
* Use the WordPress HTTP class if available
* Move the admin UI code to a separate file, only loaded when needed
* Add cron retry feature, to replace the old connectivity check
* Display Akismet status badge beside each comment
* Record history for each comment, and display it on the edit page
* Record the complete comment as originally submitted in comment_meta, to use when reporting spam and ham
* Highlight links in comment content
* New option, "Show the number of comments you've approved beside each comment author."
* New option, "Use a nonce on the comment form."

= 2.4.0 =
*Release Date - 23rd August, 2010*

* Spell out that the license is GPLv2
* Fix PHP warnings
* Fix WordPress deprecated function calls
* Fire the delete_comment action when deleting comments
* Move code specific for older WP versions to legacy.php
* General code clean up

= 2.3.0 =
*Release Date - 5th June, 2010*

* Fix "Are you sure" nonce message on config screen in WPMU
* Fix XHTML compliance issue in sidebar widget
* Change author link; remove some old references to WordPress.com accounts
* Localize the widget title (core ticket #13879)

= 2.2.9 =
*Release Date - 2nd June, 2010*

* Eliminate a potential conflict with some plugins that may cause spurious reports

= 2.2.8 =
*Release Date - 27th May, 2010*

* Fix bug in initial comment check for ipv6 addresses
* Report comments as ham when they are moved from spam to moderation
* Report comments as ham when clicking undo after spam
* Use transition_comment_status action when available instead of older actions for spam/ham submissions
* Better diagnostic messages when PHP network functions are unavailable
* Better handling of comments by logged-in users

= 2.2.7 =
*Release Date - 17th December, 2009*

* Add a new AKISMET_VERSION constant
* Reduce the possibility of over-counting spam when another spam filter plugin is in use
* Disable the connectivity check when the API key is hard-coded for WPMU

= 2.2.6 =
*Release Date - 20th July, 2009*

* Fix a global warning introduced in 2.2.5
* Add changelog and additional readme.txt tags
* Fix an array conversion warning in some versions of PHP
* Support a new WPCOM_API_KEY constant for easier use with WordPress MU

= 2.2.5 =
*Release Date - 13th July, 2009*

* Include a new Server Connectivity diagnostic check, to detect problems caused by firewalls

= 2.2.4 =
*Release Date - 3rd June, 2009*

* Fixed a key problem affecting the stats feature in WordPress MU
* Provide additional blog information in Akismet API calls

```

## Slider Revolution

A responsive slider to design and tweak the slider images.

```
=== Plugin Name ===
Contributors: dragosgaf
Donate link: http://dragosgaftoneanu.com/
Tags: revolutionslider, vulnerability, exploit, security, patch
Requires at least: 3.0
Tested up to: 4.1
Stable tag: 2.4.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

This plugin patches the existent vulnerabilities in Revolution Slider plugin, including the latest SoakSoak vulnerability.

== Description ==

This plugin patches (as long as it is active) the existent vulnerabilities in Revolution Slider plugin, including the latest SoakSoak (Arbitrary File Upload) vulnerability. 

You can also monitor using the "Black list" option all the attackers that attempt to use a Revolution Slider exploit to gain access to your website.

== Installation ==

Just upload the plugin to wp-content/plugins/, activate it and you don't need to worry anymore about anyone trying to access your private information.

== Frequently Asked Questions ==

= Why should I use this plugin? =
It's useful to use it if your Revolution Slider is in a template and you can't update it at the moment (eg. if the template has been modified).

== Changelog ==

= 2.4.2 =
* The plugin now patches an old persistent XSS vulnerability (for versions older than 4.2)

= 2.3.2 =
* Removed http_response_code because not all hosts have this function
* Changed the algorithm for cleaning the post variables in Arbitrary File Upload section (thanks @darookee)

= 2.3.1 =
* Repaired the bug that broke some RevSlider functions

= 2.3 =
* Fixed a bug that broke some Wordpress functions

= 2.2 =
* Fixed a bug to display the Arbitrary File Upload in Black list

= 2.1 =
* Updated Soaksoak patch function.

= 2.0 =
* Rewrote the entire plugin, added more options and filters to keep your Wordpress safe

= 1.0 =
* First release

== Upgrade Notice ==

= 1.0 = 
* First release

== Screenshots ==

No screenshots available.
```

## WP Super Cache

```
=== WP Super Cache - Clear all cache ===
Contributors: apasionados, netconsulting
Donate link: http://apasionados.es/
Tags: empty cache, emtpy wp super cache, cache, caching, performance, wp-cache, wp-super-cache, web performance optimization, WPO, YUI, yslow, google speed
Requires at least: 3.0.1
Tested up to: 3.9.1
Stable tag: 1.3.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Clear all cache for WP Super Cache adds a menu entry to the admin menu to clear the cache completly.

== Description ==

The plugin clears completly the cache from WP Super Cache, directly from the admin menu.

We created this plugin, in order to be able to clear the cache completly from the admin menu and not having to navigate to CONTENTS tab in WP Super Cache Settings.

In some configuration WP Super Cache shows a menu entry to empty the cache in the menu, but it only empties the cache from the current page. See: [The "Delete Cache" button on the admin menu only deletes the cache for the current page.](http://wordpress.org/support/topic/plugin-wp-super-cache-menu-delete-cache-doesnt-work-but-on-contents-page-it-does)
Nevertheless in the mayority of the sites that have WP Super Cache installed it doesn't display this menu entry.

Please note that this menu option is only visible for SUPER ADMINS.

= What can I do with this plugin? =
The plugin clears completly the cache from WP Super Cache, directly from the admin menu.

= WP Super Cache - Clear all cache Plugin in your Language! =
This first release is avaliable in English and Spanish. In the languages folder we have included the necessarry files to translate this plugin.

If you would like the plugin in your language and you're good at translating, please drop us a line at [Contact us](http://apasionados.es/contacto/index.php?desde=wordpress-org-wp-super-cache-clear-cache-menu-home).

= Further Reading =
You can access the description of the plugin in Spanish at: [WP Super Cache - Clear all cache Plugin en castellano](http://apasionados.es/blog/vaciar-cache-wp-super-cache-plugin-wordpress-1933/).


== Installation ==

1. Upload the `wp-super-cache-clear-cache-menu` folder to the `/wp-content/plugins/` directory (or to the directory where your WordPress plugins are located)
1. Activate the WP Super Cache - Clear all cache Plugin through the 'Plugins' menu in WordPress.
1. Puling doesn't need any configuration.

Please don't use it with WordPress MultiSite, as it has not been tested.

== Frequently Asked Questions ==

= What is WP Super Cache - Clear all cache Plugin good for? =
It empties completly the WP SUPER CACHE cache without having to navigate to the CONTENTS tab in WP Super Cache Settings, this plugin is for you.

= Why should I make use of the WP Super Cache - Clear all cache Plugin? = 
If you use WP Super Cache and want to be able to empty completly the cache without having to navigate to the CONTENTS tab in WP Super Cache Settings, this plugin is for you.

= Does WP Super Cache - Clear all cache make changes to the database? =
No.

= How can I check out if the plugin works for me? =
Install and activate. You will see a new menu entry in the administration area to empty the cache. Access this menu entry and your cache will be emptied and you are taken to the CONTENTS tab in WP Super Cache Settings.

= Can every registered user use this plugin? =
No. This menu option is only available for SUPER ADMINS.

= How can I remove WP Super Cache - Clear all cache? =
You can simply activate, deactivate or delete it in your plugin management section.

= What happens if I activate the plugin without using WP SUPER CACHE? =
Nothing. The plugin checks that WP SUPER CACHE is activated.

= Are there any known incompatibilities? =
Please don't use it with WordPress MultiSite, as it has not been tested.

= Do you make use of WP Super Cache - Clear all cache yourself? = 
Of course we do. ;-)

== Screenshots ==

1. There is no configuration screen for "WP Super Cache - Clear all cache". This is a ScreenShot of the menu entry that it adds (in Spanish).
2. This second example shows the menu entry from WP Super Cache we see on some installations to empty the cache of the current page. See: [The "Delete Cache" button on the admin menu only deletes the cache for the current page.](http://wordpress.org/support/topic/plugin-wp-super-cache-menu-delete-cache-doesnt-work-but-on-contents-page-it-does)

== Changelog ==

= 1.3.1 =
* Minor update to fix a problem with automatic update from WordPress plugin repository.

= 1.3 =
* Updated the code to fix the bug inspirationdate found: "The link added is relative so it doesn't work when the toolbar is displayed on the frontend".

= 1.2 =
* Updated and corrected readme.txt.

= 1.1 =
* Updated and corrected readme.txt.

= 1.0 =
* First stable release.

= 0.5 =
* Beta release.

== Upgrade Notice ==

= 1.3.1 =
Updated the code to fix the bug inspirationdate found: "The link added is relative so it doesn't work when the toolbar is displayed on the frontend". Thanks.

== Contact ==

For further information please send us an [email](http://apasionados.es/contacto/index.php?desde=wordpress-org-wp-super-cache-clear-cache-menu-contact).
```

## YITH WooCommerce Wishlist

```
=== YITH WooCommerce Wishlist === 

Contributors: yithemes
Tags: wishlist, woocommerce, products, themes, yit, e-commerce, shop, ecommerce wishlist, yith, woocommerce wishlist, woocommerce 2.3 ready, shop wishlist
Requires at least: 4.0
Tested up to: 4.2.4
Stable tag: 2.0.10
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

YITH WooCommerce Wishlist add all Wishlist features to your website. Needs WooCommerce to work.
WooCommerce 2.3.x compatible.


== Description ==

What can really make the difference in conversions and amount of sales is without a doubt the freedom to share your own wishlist, even on social networks, increasing indirect sales: can you imagine the sales volume you can generate during holidays or birthdays, when relatives and friends will be looking for the wishlist of your clients to buy a gift?

Offer to your visitors a chance to add the products of your woocommerce store to a wishlist page. With YITH WooCommerce Wishlist you can add a link in each product detail page,
in order to add the products to the wishlist page. The plugin will create you the specific page and the products will be added in this page and
afterwards add them to the cart or remove them.

Working demo are available:

**[LIVE DEMO 1](http://preview.yithemes.com/room09/product/africa-style/)** - **[LIVE DEMO 2](http://preview.yithemes.com/bazar/shop/ankle-shoes/)**

Full documentation is available [here](http://yithemes.com/docs-plugins/yith-woocommerce-wishlist).

This plugin is 100% compatible with [WPML](http://wpml.org/?aid=24889&affiliate_key=Qn1wDeBNTcZV)

= Available Languages =

* Chinese - CHINA
* Chinese - TAIWAN
* English - UNITED KINGDOM (Default)
* German - GERMANY
* Spanish - ARGENTINA
* Spanish - MEXICO
* French - FRANCE
* Hebrew - ISRAEL
* Italian - ITALY
* Persian - IRAN, ISLAMIC REPUBLIC OF
* Portuguese - BRAZIL
* Portuguese - PORTUGAL
* Russian - RUSSIAN FEDERATION
* Turkish - TURKEY
* Ukrainian - UKRAINE

== Installation ==

1. Unzip the downloaded zip file.
2. Upload the plugin folder into the `wp-content/plugins/` directory of your WordPress site.
3. Activate `YITH WooCommerce Wishlist` from Plugins page

YITH WooCommerce Wishlist will add a new submenu called "Wishlist" under "YIT Plugins" menu. Here you are able to configure all the plugin settings.

== Frequently Asked Questions ==

= Can I customize the wishlist page? =
Yes, the page is a simple template and you can override it by putting the file template "wishlist.php" inside the "woocommerce" folder of the theme folder.

= Can I move the position of "Add to wishlist" button? =
Yes, you can move the button to another default position or you can also use the shortcode inside your theme code.

= Can I change the style of "Add to wishlist" button? =
Yes, you can change the colors of background, text and border or apply a custom css. You can also use a link or a button for the "Add to wishlist" feature.

= Wishlist page returns a 404 error? =
Try to regenerate permalinks from Settings -> Permalinks by simply saving them again.

= Did icons of your theme disappear after update to Wishlist 2.0.x? =
It might be a compatibility problem with the old version of font-awesome, which has been solved with version 2.0.2 of the plugin. Be sure that you are using a plugin version that is greater or equal to 2.0.2. If, after update, you cannot see icons in your theme yet, save again options of YITH WooCommerce Wishlist plugin (that you can find in YIT Plugin -> Wishlist).

= Have you encountered anomalies after plugin update, that did not exist in the previous version? =
This might depend on the fact that your theme overrides plugin templates. Check if the developer of your theme has released a compatibility update with version 2.0 or later of YITH WooCommerce Wishlist. As an alternative you can try the plugin in WordPress default theme to leave out any possible influences by the theme.

= I am currently using Wishlist plugin with Catalog Mode enabled in my site. Prices for products should disappear, yet they still appear in the wishlist page. Can I remove them? =
Yes, of course you can. To avoid Wishlist page to show product prices, you can hide price column from wishlist table. Go to YIT plugins -> wishlist -> settings and disable option "Show Unit price".

== Screenshots ==

1. The page with "Add to wishlist" button
2. The wishlist page
3. The Wishlist settings page
4. The Wishlist settings page

== Changelog ==

= 2.0.10 =

* Added: Compatibility with WC 2.4.2
* Tweak: added nonce field to wishlist-view form
* Tweak: added yith_wcwl_custom_add_to_cart_text and yith_wcwl_ask_an_estimate_text filters
* Tweak: added check for presence of required function in wishlist script
* Fixed: admin colorpicker field (for WC 2.4.x compatibility)

= 2.0.9 =

* Added: russian translation
* Added: WooCommerce class to wishlist view form
* Added: spinner to plugin assets
* Added: check on "user_logged_in" for sub-templates in wishlist-view
* Added: WordPress 4.2.3 compatibility
* Added: WPML 3.2.2 compatibility (removed deprecated function)
* Added: new check on is_product_in_wishlist (for unlogged users/default wishlist)
* Tweak: escaped urls on share template
* Tweak: removed new line between html attributes, to improve themes compatibility
* Fixed: WPML 3.2.2 compatibility (fix suggested by Konrad)
* Fixed: regex used to find class attr in "Add to Cart" button
* Fixed: usage of product_id for add_to_wishlist shortcode, when global $product is not defined
* Fixed: icon attribute for yith_wcwl_add_to_wishlist shortcode

= 2.0.8 =

* Added: support WP 4.2.2
* Added: Persian translation
* Added: check on cookie content
* Added: Frequently Bought Together integration
* Tweak: moved cookie update before first cookie usage
* Updated: Italian translation
* Removed: login_redirect_url variable

= 2.0.7 =

* Added: WP 4.2.1 support
* Added: WC 2.3.8 support
* Added: "Added to cart" message in wishlist page
* Added: Portuguese translation
* Updated: revision of all templates
* Fixed: vulnerability for unserialize of cookie content (Warning: in this way all the old serialized plugins will be deleted and all the wishlists of the non-logged users will be lost)
* Fixed: Escaped add_query_arg() and remove_query_arg()
* Removed: use of pretty permalinks if WPML enabled

= 2.0.6 =

* Added: system to overwrite wishlist js
* Added: trailingslashit() to wishlist permalink
* Added: chinese translation
* Added: "show_empty" filter to get_wishlists() method
* Fixed: count wishlist items
* Fixed: problem with price inclusive of tax
* Fixed: remove from wishlist for not logged user
* Fixed: twitter share summary

= 2.0.5 =

* Added: icl_object_id to wishlist page id, to translate pages
* Tweak: updated rewrite rules, to include child pages as wishlist pages
* Tweak: moved WC notices from wishlist template to yith_wcwl_before_wishlist_title hook
* Tweak: added wishlist table id to .load(), to update only that part of template
* Fixed: yith_wcwl_locate_template causing 500 Internal Server Error

= 2.0.4 =

* Added: Options for browse wishlist/already in wishlist/product added strings
* Added: rel nofollow to add to wishlist button
* Tweak: moved wishlist response popup handling to separate js file
* Updated: WPML xml configuration
* Updated: string revision

= 2.0.3 =

* Tweak: set correct protocol for admin-ajax requests
* Tweak: used wc core function to set cookie
* Tweak: let customization of add_to_wishlist shortcodes
* Fixed: show add to cart column when stock status disabled
* Fixed: product existing in wishlist

= 2.0.2 =

* Updated: font-awesome library
* Fixed: option with old font-awesome classes

= 2.0.1 =

* Added: spinner image on loading
* Added: flush rewrite rules on database upgrade
* Fixed: wc_add_to_cart_params not defined issue

= 2.0.0 =

* Added: Support to woocommerce 2.3
* Added: New color options
* Tweak: Add to cart button from woocommerce template
* Tweak: Share links on template
* Tweak: Code revision
* Tweak: Use wordpress API in ajax call instead of custom script
* Updated: Plugin core framework


= 1.1.7 =

* Added: Support to WooCommerce Endpoints (@use yit_wcwl_add_to_cart_redirect_url filter)
* Added: Filter to shortcode html
* Added: Title to share

= 1.1.6 =

* Updated: Plugin Core Framework
* Updated: Languages file
* Tweek:   WPML Support Improved

= 1.1.5 =

* Added: Share wishlist by email 

= 1.1.4 =

* Fixed: wrong string for inline js on remove link
* Fixed: wrong string for inline js on add to cart link

= 1.1.3 =

* Added: Options Tabs Filter
* Fixed: Various Bugs

= 1.1.2 =

* Fixed: Warnings when Show Stock Status is disabled
* Fixed: Restored page options on WooCommerce 2.1.x

= 1.1.1 =

* Fixed: Inability to unistall plugin 
* Fixed: Redirect to cart page from wishlist page

= 1.1.0 =

* Added: Support to WooCommerce 2.1.x
* Added: Spanish (Mexico) translation by Gabriel Dzul
* Added: French translation by Virginie Garcin
* Fixed: Revision Italian Language po/mo files

= 1.0.6 =

* Added: Spanish (Argentina) partial translation by Sebastian Jeremias
* Added: Portuguese (Brazil) translation by Lincoln Lemos
* Fixed: Share buttons show also when not logged in
* Fixed: Price shows including or excluding tax based on WooCommerce settings
* Fixed: Better compatibility for WPML 
* Fixed: Price shows "Free!" if the product is without price
* Fixed: DB Table creation on plugin activation

= 1.0.5 =

* Added: Shared wishlists can be seens also by not logged in users
* Added: Support for WPML String translation
* Updated: German translation by Stephanie Schlieske
* Fixed: Add to cart button does not appear if the product is out of stock

= 1.0.4 =

* Added: partial Ukrainian translation
* Added: complete German translation. Thanks to Stephanie Schliesk
* Added: options to show/hide button add to cart, unit price and stock status in the wishlist page
* Added: Hebrew language (thanks to Gery Grinvald)

= 1.0.3 =

* Fixed: Minor bugs fixes

= 1.0.2 =

* Fixed: Fatal error to yit_debug with yit themes

= 1.0.1 =

* Tweak: Optimized images
* Updated: internal framework

= 1.0.0 =

* Initial release

== Suggestions ==

If you have suggestions about how to improve YITH WooCommerce Wishlist, you can [write us](mailto:plugins@yithemes.com "Your Inspiration Themes") so we can bundle them into YITH WooCommerce Wishlist.

== Translators ==

= Available Languages =
* Chinese - CHINA
* Chinese - TAIWAN
* English - UNITED KINGDOM (Default)
* German - GERMANY
* Spanish - ARGENTINA
* Spanish - MEXICO
* French - FRANCE
* Hebrew - ISRAEL
* Italian - ITALY
* Persian - IRAN, ISLAMIC REPUBLIC OF
* Portuguese - BRAZIL
* Portuguese - PORTUGAL
* Russian - RUSSIAN FEDERATION
* Turkish - TURKEY
* Ukrainian - UKRAINE

Some of these translations are not complete.
If you have created your own language pack, or have an update for an existing one, you can send [gettext PO and MO file](http://codex.wordpress.org/Translating_WordPress "Translating WordPress")
[use](http://yithemes.com/contact/ "Your Inspiration Themes") so we can bundle it into YITH WooCommerce Wishlist Languages.

== Documentation ==

Full documentation is available [here](http://yithemes.com/docs-plugins/yith-woocommerce-wishlist).

== Upgrade notice ==

= 2.0.10 =

* Added: Compatibility with WC 2.4.2
* Tweak: added nonce field to wishlist-view form
* Tweak: added yith_wcwl_custom_add_to_cart_text and yith_wcwl_ask_an_estimate_text filters
* Tweak: added check for presence of required function in wishlist script
* Fixed: admin colorpicker field (for WC 2.4.x compatibility)
```


## Deployment instructions

Deploy to a server which supports Wordpress like Godaddy, HostGator etc. HostGator is more speedy in loading pages imo than other websites.

 In most cases I code locally and later upload to my cPanel. I will try and upload this website and fight the urge of pulling it down. (For some reason many people buy demo websites and request that they get pulled down. Let's cross fingures to thwart that.) 

## Developer

Joseph Musembi Mwania

## Contacts

http://www.theappwebtech.com/

https://github.com/appwebtech

https://twitter.com/appwebtech

https://www.facebook.com/theappwebtech/

https://it.pinterest.com/appwebtech/




