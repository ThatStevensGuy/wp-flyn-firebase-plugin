=== Firebase URL Shortener ===
Contributors: kovshenin
Donate link: https://www.flynsarmy.com/
Tags: links, twitter, short, url, socialmedia, permalinks, redirect, trim, identi.ca, microblogging, shorturl, canonical, analytics
Requires at least: 3.0
Tested up to: 4.9.4
Stable tag: 1.0.0

Uses Google's URL shortener (Firebase) to create short links for your WordPress posts.

== Description ==

Google has launched a URL Shortener API (Firebase) - one of the fastest and most reliable URL shortners out there. This plugin creates short URLs for your posts, which then could be retrieved using the "Get Shortlink" button in your admin UI or the `wp_get_shortlink()` WordPress function.

== Installation ==

1. Upload archive contents, or git clone to 'flyn-firebase' directory in '/wp-content/plugins/'
2. Visit https://console.firebase.google.com and create a project 'URL Shortener'. If you already have a Google Cloud Platform project, you can use that.
3. From the 'Project Overview > Gear Icon > Project settings' page, copy the Web API Key value and paste it into a line in *wp-config.php* `define('FLYN_FIREBASE_API_KEY', '<API KEY HERE>');`
4. From the 'Project Overview' page, add a dummy iOS App by entering any value for the Bundle ID and skip the subsequent steps
5. From the 'Grow - Dynamic Links' page, hit 'Get Started' and Google will offer a provided URL. Proceed through the steps, then Copy and Paste the URL to a line in *wp-config.php* `define('FLYN_FIREBASE_URL', '<YOUR URL>');` (Should look like *https://example.page.link/*)
6. Activate the plugin through the 'Plugins' menu in WordPress
7. You're done!

== Screenshots ==

1. Shortened URLs
2. Posts List Column

== Change log ==

= 1.0 =
* First version
