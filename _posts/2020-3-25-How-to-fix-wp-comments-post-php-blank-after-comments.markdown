---
layout: post
title: How to fix wp-comments-post.php blank after comments ?
author: Rahul
categories: blogging
comments: false
image: assets/images/wordpress.jpg
---

Ok this will be a very simple fix and most probably this is not a problem on your end but the web host or server side. This blog is hosted on awardspace and I also faced this program. But not to worry there is a very simple solution. I don’t know why this problem occurs but I think may be for some reason the server is not executing this specific file ‘wp-comments-post.php’ or may be the server might have blocked that file. But there is a very simple solution that we are going to share.
<h3>Solution</h3>
All you have to do is open the file manager or you can use a FTP client to access the files and find the file wp-comments-post.php . This file will be located at the root of your WordPress installation. The same area where the wp-config.php is located.

Then what you have to do is rename wp-comments-post.php to any new name. For example I renamed my file to fixed-comments.php. Then after doing that open the folder wp-includes and find the file <strong>comment-template.php</strong>. Now open comment-template.php in editor. Inside that file there is a reference to wp-comments-post.php which you should change to the new name that you earlier renamed the file to. In our case it is fixed-comments.php. In my WordPress version the reference was at line number 2401 of the comment-template.php so in your case it should be something near that number Or you can simply download that file and open it in a text editor and search for the reference to wp-comments-post.php and change it.
