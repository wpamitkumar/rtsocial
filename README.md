![alt text](https://plugins.svn.wordpress.org/rtsocial//assets/banner-772x250.jpg)

# rtSocial #

* **Contributors:** [rtcamp] (http://profiles.wordpress.org/rtcamp), [rahul286] (http://profiles.wordpress.org/rahul286), [rutwick] (http://profiles.wordpress.org/rutwick), [saurabhshukla] (http://profiles.wordpress.org/saurabhshukla), [HarishChaudhari] (http://profiles.wordpress.org/HarishChaudhari), [faishal] (http://profiles.wordpress.org/faishal), [5um17] (http://profiles.wordpress.org/5um17), [JoshuaAbenazer] (http://profiles.wordpress.org/JoshuaAbenazer),

* **License:** [GPL v2 or later] ( http://www.gnu.org/licenses/gpl-2.0.html)

* **Donate Link:** http://rtcamp.com/donate/


This plugin uses non-blocking JavaScript to display social media sharing counters on posts/pages

## Description ##
Normally social sharing codes provided by facebook, twitter, etc renders iframes at run-time. These iframes increases page-size and slow-down your website (on client-side).

The power of this plugin lies in non-blocking JavaScript. Normally social sharing links use iframes to output their content viz. icon images, share counts etc. The load time of these iframes block the page load, and hence slow down the site. The slowest is on pages with multiple instances of sharing links (e. g. blog indexes). rtSocial uses non blocking JavaScript to get all the data in one shot, and injects them in the mark-up. And it uses a single sprite with all the images required, hence eliminating the need to load the images from the service provider's CDN. Comes with minimal settings, options to display the links automatically above and below the content, choose FB button styles and layouts. A simple function call lets you to display the links anywhere in your theme!

With just 1 image (CSS-sprite), 1 JavaScript and 1 CSS file loaded from WordPress-running server; counts are fetched using AJAX request for sites like facebook/twitter after page loading finishes.

#### Supported Social Channels ####
* Facebook
* Twitter
* Google+
* LinkedIn
* Pinterest

#### Useful Links ####
* [rtSocial Plugin's Homepage](http://rtcamp.com/rtsocial/)
* [Free Support Forum](http://rtcamp.com/support/forum/rtsocial/)

## Installation ##
Install rtSocial plugin from the 'Plugins' section in your dashboard (Plugins > Add New > Search for rtSocial).

Alternatively you can [download latest version](http://downloads.wordpress.org/plugin/rtsocial.2.0.1.zip) of rtSocial plugin from the repository. Unzip it and upload it to the plugins folder of your WordPress installation (wp-content/plugins/ directory of your WordPress installation).

Activate it through the 'Plugins' section.

Adjust the plugin settings from the settings section (Settings > rtSocial Options).

## Screenshots ##
Please visit [rtSocial Plugin's Homepage](http://rtcamp.com/rtsocial/)

## Frequently Asked Questions ##

#### Can I use the plugin anywhere in the theme? ####

Yes you can. Use the function call
`<?php
if ( function_exists( 'rtsocial' ) ) {
       echo rtsocial();
}
?>`


#### Can I modify the images/icons used? ####

No. Right now you cannot.


## Changelog ##

#### 2.1.9 ####
* Fixed bug where 0's turned up in RSS entries

#### 2.1.8 ####
* Removed page summary from Linked in share. It was too undependable and unpredictable.

#### 2.1.7 ####
* Reverted excerpt function. Fixed non-display of rtsocial.

#### 2.1.6 ####
* Fixed inadvertent typo.

#### 2.1.5 ####
* Fixed bug with post excerpts on archive pages. Thanks to [iseroma](http://profiles.wordpress.org/iseroma/) for reporting this.

#### 2.1.4 ####
* Fixed bug with facebook counts on IE. Thanks to [ward00](http://profiles.wordpress.org/ward00/) for reporting this.

#### 2.1.3 ####
* Fixed bug on archive pages

#### 2.1.2 ####
* Fixed LinkedIn share button
* Updated facebook button because the earlier graph url won't give counts anymore

#### 2.1.1 ####
* Improved title output

#### 2.1 ####
* Added rel nofollow to all buttons.
* Fixed bug where unnecessary slashes were added to _blank. Thanks to [Vinity](http://rtcamp.com/support/topic/minor-html-code-flaw-suggestions/) for pointing this out
* Added titles to all buttons

#### 2.0.2 ####
* Added fallback image for Pinterest
* Added functionality to over-ride options (Manual Mode)
* Fixed ID conflicts
* Changed default text for Pinterest to post title

#### 2.0.1 ####
* Fixed few issues reported by users

#### 2.0 ####
* Added support for Google Plus, LinkedIn and Pinterest
* Custom URL Encode function
* Fixed few issues reported by users
* Enhanced Options Page

#### 1.0.2 ####
* URL Encode Improved

#### 1.0.1 ####
* Fixed minor CSS issue

#### 1.0 ####
* Initial Release

#### 2.1.9 ####
Fixed RSS entry issue.
