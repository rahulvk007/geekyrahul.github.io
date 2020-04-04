---
layout: post
title: 'How To Install And Configure WP Super Cache Plugin In WordPress In 2019 ? '
author: Rahul
categories: blogging
image: assets/images/blog.jpg
permalink: /:categories/:title
comments : false
---
What is WP Super Cache?

WP Super Cache is a caching plugin for WordPress.It generates static html files for your website which is then directly served by your web server.Caching can increase your WordPress website speed.
Generally without caching active when a page or post of your WordPress site is visited it involves a lot of php processing and database queries. Those things take time and will also exhaust your server resources during traffic spikes. Therefore caching is very important for your website.Two most famous plugins are WP Super Cache and W3 Total Cache.

In this article we are going to look at installing and configuring WP Super Cache.

Step 1:Go to plugins tab on your WordPress dashboard and select Add New. There search for WP Super Cache

<img src='{{site.baseurl}}/assets/images/plugin.jpg'>

Step 2: After activating the plugin go to WP Super Cache settings page.Here you can turn caching on/off in one click. Turn on Caching

<img src='{{site.baseurl}}/assets/images/supercache-settings.jpg'>

here enable caching
Step 3: Go to Advanced tab of WP Super Cache Settings. Then I am showing you the recommended settings. It is better you copy it.

<img src='{{site.baseurl}}/assets/images/cache-delivery.jpg'>


enable caching
Here we choose the Cache Delivery method. Here we have two options – Simple and Expert . Simple uses php itself to deliver the cached files. It is recommended. If you are an expert user and have no problem in editing .htaccess then you may choose Expert method.

Expert Method is the fastest since it uses Apache mod_rewrite rules to deliver static content directly. But this may require editing .htaccess file.

<img src='{{site.baseurl}}/assets/images/wp-super-cache-other-settings-1-1024x386.jpg'>

These are the settings that I recommend:

Check- Don’t Cache pages for known users.

Check- Compress pages so they’re served more quickly to visitors. (Recommended)

Check- Cache rebuild. Serve a supercache file to anonymous users while a new file is being generated. (Recommended)

Check- 304 Not Modified browser caching. Indicate when a page has not been modified since it was last requested. (Recommended)

Check- Mobile device support. (External plugin or theme required. See the FAQ for further details.)

Update status

<img src='{{site.baseurl}}/assets/images/cache-expiry.jpg'>


This is the Expiry Time & Garbage Collection section. Here you can set the time in seconds after which your cache should be deleted and renewed.We chose to go with default setting which is 1800 seconds. After this you should save all settings by clicking on Change Expiration.

Now lets check if the cache is working properly. For that go to easy tab

<img src='{{site.baseurl}}/assets/images/test-cache.jpg'>


Click on Test Cache. If the result comes green OK then your cache is working.

Our Experience with this plugin

Our experience with this plugin has been great. After installing and configuring it our web site started loading faster and we started getting higher scores in Website optimization tests.
