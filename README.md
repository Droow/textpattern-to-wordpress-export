Textpattern to WordPress Exporter
=================================

This script is based on [another export script](https://github.com/drewm/textpattern-to-wordpress), but uses classic mysql driver instead of PDO.

It creates a WordPress-format export file from a Textpattern blog.

# Installation

Put the `txp-exporter.php` file in your Textpattern site, at the same level as the textpattern folder (usually root), then load it up in your web browser. Your directory structure should look like this:

Navigate to this file (usually http://yoursite.com/txp-exporter.php) and download the XML file.

Install the [WordPress Importer Plugin](https://wordpress.org/plugins/wordpress-importer/), activate it and go to the Tools -> Import page in admin of your WP site. Click Wordpress and select the previously downloaded file.

# Configuration

* At the top of the file you can tweak the include path to your TXP config file
* If you want to export as raw Textile, append "?exportRaw" to the URL (http://yoursite.com/txp-exporter.php?exportRaw)

# Important note

This script does not exports any Textpattern custom fields yet.

# Requirements

* PHP 5.2