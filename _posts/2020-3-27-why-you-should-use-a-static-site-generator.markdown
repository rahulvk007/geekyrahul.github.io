---
layout: post
title: Why you should use a static site generator ?
author: Rahul
categories: blogging
comments: false
image: assets/images/webdesign.jpg
---
Most website owners uses a CMS like <a href= "https://wordpress.org">WordPress</a> to power their website on the internet. In fact according to WordPress more than 60 million people use Wordpress. That’s a lot of people. Moreover WordPress is open source that means you can modify WordPress according to your needs and you don’t need to pay anything. So for a beginner it is highly recommend that you use a CMS like WordPress so that you can focus more on creating good quality content. One of the best things about WordPress is you don’t need to have any technical knowledge to use WordPress.

WordPress and all other similar CMS has some common disadvantages also. Mainly WordPress is very resource intensive. That means hosting becomes very expensive as your site grows and you start getting a lot of traffic. Another big disadvantage of these CMS is speed. Usually when some one visits a site that uses a CMS like Wordpress php file is executed to query the database and generate HTML.
This is all takes time. You can use caching to speed up your site but it will still be slower than a static site.

Now what you can do to get a very fast and efficient site without compromising much on ease of use is to go with a static site generator. In this article we are going to give you the pros and cons of using a static site generator instead of using a CMS and we will try to answer the question Why you should use a static site generator and we will be giving you an introduction to most popular static site generators out there.

<h3> Why you should use a static site generator ? </h3>

One of the best advantages of using a static site generator is that you can easily generate a beautiful clean static website without the need of knowing HTML,CSS or JavaScript.
The advantage of a static site is that since there is no processing it is very fast. A basic static website will be much faster than a website that is powered by a CMS like WordPress. Even without any caching. Another very big advantage is that you can host a static website for free or very cheap prices. You can actually host a popular website for free with GitHub pages or <a href="https://www.netlify.com">Netlify</a>. Both provide excellent hosting services.
Yes there are many hosting services that allow you to host php powered sites like WordPress for free but they are too slow or will have many other limitations. My website was initially using WordPress and I was very hesitant to spend money on hosting because I was afraid it would prove to be a failure.I am very sure most of the people who want to start blogging are also thinking the same way that if the website becomes successful then we would upgrade to paid hosting. But the main problem is if you want your website to be successful then it should be very fast and responsive, two things that are difficult to accomplish with free hosting.

But if you are hosting a static site then you have a lot of choices. You can basically host your site anywhere. Since there is no server side processing  involved even the most basic hosting services could power your site with appreciable speed.

If you are planning to make your website static then I highly recommend that you use Netlify as their services are excellent. You can host your website on their free plan itself. They provide you CDN and even free ssl on their free plan itself. You can also host your site on GitHub pages, they also provide you free ssl.

<h3> How does a static site generator works ? </h3>

Ok, now let me try to give you a general idea about how a static site generator works. It could be slightly different for different static site generators. So I will try to explain the workings of a static site generator by taking the case of the most popular static site generator out there <a href="https://jekyllrb.com/">Jekyll</a> . Jekyll is powered by ruby programming language. But you don't need to have any prior knowledge about ruby to use Jekyll. In Jekyll we write posts and pages in markdown language. And then Jekyll runs and generates HTML from the markdown files using the layout of the theme that we have installed. When a user visits our website the user is served the already generated HTML. Whenever you make any changes Jekyll runs and regenerates HTML . So it basically works like a static site and you get all the speed and other benefits of using a static site.  You don't need to worry about having to learn markdown because for using Jekyll you only need to learn very basic things and it will not take you even five minutes. Currently this blog uses Jekyll. I already told you that initially I used WordPress. I was very hesitant to change to Jekyll because I was afraid of having to learn a new language. But now I am very happy that changed to Jekyll. There is very less to learn.  All you have to learn is the folder structure and in every post or page you have to start with four or five lines of markdown code that tells Jekyll about the permalink , title and which layout to use.

You also get the full freedom of using your own layout.
One of the best things about Jekyll is that it is simple enough so that a simple user who just wants to get a blog running(like me) can use it and also advanced enough so that some one who has in depth knowledge of HTML and CSS and wants total control of their blog can also use it. You will get full HTML and CSS freedom in Jekyll if you choose so. That is a very big advantage for Jekyll. Now many large sites are also switching to static site generators like Jekyll. One of the things I would like to say again is the cost. Hosting a static site is much cheaper than hosting a dynamic site.
Now I will post the image of my website speed test from <a href="https://tools.pingdom.com">pingdom</a>. I haven't done any optimization. This is just the out of the box speed test.

<img src='{{site.baseurl}}/assets/images/result.jpg'>

This is fast and I mean insanely fast considering that there is no optimization done by me.

Many studies show that a huge percentage of visitors will leave a website if it takes more than three seconds to load. Also google uses speed as a one of the important ranking factors. So having a very fast website is a necessity now.

Another big advantage of static sites is security. WordPress and other similar CMS are less secure. They require a lot of work by the user to get them safe. It often includes having to install a premium plugin . There are many plugins that do this for free also. But still such sites are more prone to getting hacked. Since static sites are less complex and simple there are not much exploits a hacker can use to gain access to .Chances of your static site getting hacked or infected with malware is very less. When I was using WordPress one time I got a notification from google that my site was not secure and it was infected by malware. Google chrome also started showing a warning message when people tried to visit my site. That gave me a lot of headaches. It took me lot of effort to find a solution and clean my site. In the case of a static site things are much simple. All you have is a few HTML pages and your static files. Chances of getting a malware is very low and even if you get it you will be able to easily fix it.

<h3> So should you use a static site generator instead of a CMS like WordPress ? </h3>

Well there is no straight answer. We spend the entire article telling you the reasons to make a switch. But the final answer is it depends. Are you ready to pay for expensive hosting ? Do you want to entirely devote your time to writing good quality content and don't want to be bothered by the workings of your site ? Are you ready to pay a small price for good plugins ?

If your answer is yes then there is no reason for you to make a switch. But if you are more focused on speed , don't want to pay for hosting and is ready to go into the behind the scenes of how a website works then give it a try.
What I suggest is try both WordPress and a static site generator like Jekyll and go with the one with which you are more comfortable.

The background image in the top of the page was downloaded from Pixabay. Image by Image by <a href="https://pixabay.com/users/kreatikar-8562930/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=3411373">Mudassar Iqbal</a> from <a href="https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=3411373">Pixabay</a>
