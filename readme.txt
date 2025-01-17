=== News Ticker FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, news, ticker, free, flash, as3, autoscroll, xml, rss, feed, animation, feeds, css, text, roll, over, out, effects
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

One of the most advanced News Ticker on the web. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without even using Flash. It has autoscroll functionality with customizable roll over/out effects. It supports external RSS feeds and custom created with HTML/CSS formatted text. There are many more customizable properties on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/news-ticker-fx.zip "News Ticker FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/news-ticker.zip "News Ticker FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **news-ticker-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **News Ticker FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[news-ticker-fx][/news-ticker-fx]` where you want the Flash to show up in your post/page
5. If you want to make the News Ticker FX part of your theme, edit the template files and add `<?php newstickerfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your News Ticker FX](http://www.flashxml.net/news-ticker.html "News Ticker FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/news-ticker-fx/settings.xml`

= Additional settings file =

To embed the News Ticker FX more than once, you will need another settings file. Let's assume your new file is called `settings2.xml`. Add `[news-ticker-fx settings="settings2.xml"][/news-ticker-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `newstickerfx_echo_embed_code()` function call (for example `<?php newstickerfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[news-ticker-fx]` and `[/news-ticker-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `newstickerfx_echo_embed_code()` function call (for example `<?php newstickerfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[news-ticker-fx width="600" height="300"][/news-ticker-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `newstickerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/news-ticker.html "News Ticker FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/news-ticker-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/news-ticker.html "News Ticker FX") is the utility that helps easily customize your News Ticker FX to fit all your needs.