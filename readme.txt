=== BlogMechanics KeywordLink ===
Contributors: blogmechanic
Tags: keyword,link,replacement
Requires at least: 2.3
Tested up to: 2.7
Stable tag: trunk

A plugin that allows you to define keyword/link pairs. The keywords are automatically linked in each of your posts. 

== Description ==

A plugin that allows you to define keyword/link pairs. The keywords are automatically linked in each of your posts. This is usefull
for improving the internal cross referencing pages inside your site or to automatically link to external partners (SEO).

You can decided for each link if you would like to: 

* Add a "No Follow" 
* Match only on the first mention
* Open a new window on clicking the link
* Match any case (ignore case) in the keyword
* Apply the link also to your posts comment section

It is possible to CSS style links: 

* If the link is an affiliate you would like to disclose 
* Any other link tagged by the plugin  

To help maintain longer keyword lists it is also possible to import and export lists of keywords to a comma seperated values (CSV) 
file, handy if you would like to edit the list of keywords in a spreadsheet.  

Example:  "A visit to the UK is not complete without a visit to Stonehenge."

Would become:  "A visit to the UK is not complete without a visit 
                to <A href="link">Stonehenge</a>."

v0.7.1

* Fixed a warning message for first time users 

v0.7

* You can now also (optionally) link keywords in the comments section  
* A reverse keysort is now applied before matching keywords to text. As a result
  "Widgets for sale in America" now matches before "Widgets for sale" and "Widgets"
  independent of their order in the definition list
* Fixed an issue with the "Edit" action not correctly selecting fields

v0.6 

* It is now possible to use apostrophes in keywords (the boy's hat)
* You can import and export the keyword list to and from a comma seperated values file

v0.5

* Fixed a "space" issue
* Added basic help to the configuration page
* Added support for affiliate links

v0.4.5 

* Added: A little bit of javascript to allow for editing of existing keywords as some of you 
         now have over 150 entries it will also jump to the editor at the bottom of the screen. 

v0.4.2

* Fixed: Compatibly problem with Ozh Click counter plugin

v0.4 

* Fixed the linking of matching url's problem
* It is now possible to open a new window for a link (target=_blank)
* It is now possible to ignore case when matching a keyword

v0.3.1

It is now possible to specify per link if you would like to :

* Link only the first mention of the keyword in the article (or all, which is the default)
* Tag a link as “nofollow” , useful for external links.

The replacement routine is also smarter about linking keywords. For example: “magic” will match “magic” , but no longer to “magically”.

version 0.2: 
                
If you would like to modify the style of the link. For example to make the link
bold add the following to your style.css file: 

.bm_keywordlink { font-weight: bold; }                


== Installation ==

(1) unzip the bm_keywordlink.zip file in /wp-content/plugins
(2) Active the plugin 

The plugin is designed for western languages that use spaces between the words to avoid matching
against variants of the same word (magic, magician..) 