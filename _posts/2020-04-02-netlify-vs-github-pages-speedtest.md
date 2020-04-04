---
layout: post
title: Netlify vs Github Pages Speedtest
author: Rahul
categories: blogging
permalink: /:categories/:title
comments: false
image: assets/images/server.jpg
description: "Netlify vs Github Pages Speed Test.In this article we conduct multiple speed tests on two versions of same website one hosted on github pages and the other hosted on Netlify and attempt to find out which one is the fastest"
---
Netlify one of the most popular choice among those looking to host a static website. Github pages is a free static site hosting service offered by the largest git service Github. Both are popular among those looking to host a static site. Both are excellent and responsive and provide a great hosting solution. Today we are going to find out among the two which is the fastest. Speed is one of the factors considered by the search engine on ranking. And also it is said that a large number of people will exit the site if the site does not load under 3 seconds. In this article we are going to compare both Github pages and Netlify on the basis of their speed.

<h3>Our Test Conditions</h3>

We set up a two identical websites on github pages and netlify. In fact both of them were deployed from the same github repository. The site was built using the static site generator Jekyll. We installed the mediumish theme on our test site. The theme already had a few posts built in complete with images. This helped us to simulate a real world scenario. The size of the webpage was around 1.9 MB. So the average size. There was a good number of css and js files on the webpage. We took multiple runs to minimize error and also to give the cdn time to cache resources. Because usually the first one or two requests will be cache miss as the cdn cache will be probably expired. But after a few visits everything will start to get served from the cdn.

Services we used for the speed test are given below. 

<ul>
  <li> Inspect option in Google Chrome</li>
  <li> <a href="https://tools.pingdom.com">Pingdom Tools</a> </li>
  <li> <a href="https://gtmetrix.com">GTmetrix</a></li>
  <li> <a href="https://www.dotcom-monitor.com">dotcom-monitor</a>  </li>
  <li> <a href="https://www.dareboost.com/en/tool/website-speed-test">Dareboost</a></li>
  <li> <a href="https://www.webpagetest.org/">Webpage Test</a></li>
  <li> <a href="https://tools.keycdn.com/speed">Keycdn Speed Test</a></li>
</ul>

So these are tools and services we used to conduct this test. Before giving you the results I have to tell you in some cases they were not consistent for both services.The next thing is just my personal opinion. So i have blurred it if you want you can click on the blurred text to un blur it.Among the two services i found<span class="spoiler"> Netlify </span>to be little more consistent.

Both Github pages and Netlify are excellent solutions for hosting your site.Now lets find out who is faster and by how much.
<h3> Results </h3>
<h4> Inspect option in Google Chrome </h4>

<h5>Netlify speed test result</h5>
<img src='{{site.baseurl}}/assets/images/netlify-version.jpg'>
This speed test may not be that accurate as my internet is a bit slow.

<h5>Github Pages Speed Test</h5>
<img src='{{site.baseurl}}/assets/images/chrome-inspector.jpg'>
This speed test may not be that accurate as my internet is a bit slow.

<h4>Pingdom Results</h4>

<h5>Netlify speed test result</h5>
<img src='{{site.baseurl}}/assets/images/pingdom-netlify.jpg'>
As you can see a 2 MB webpage loaded in 475ms which is very fast.We ran multiple tests and took the most concordant result.

<h5>Github Pages Speed Test</h5>
<img src='{{site.baseurl}}/assets/images/pingdom-github.jpg'>
As you can see the 2 MB webpage loaded in 522 ms which is also very fast. A 47 ms difference in loading times is negligible. You may have noticed that the github pages version had 30 requests compared to 29 requests on netlify version. We don't know why. Both are exactly the same site and are even deployed from the same repository.

<h4>GTmetrix </h4>

<h5>Netlify speed test result</h5>
<img src='{{site.baseurl}}/assets/images/gtmetrix-netlify.jpg'>
It is the same web page. It took 1.3 seconds to load.I don't understant why different sites are showing different number of requests. So as you can see it is very fast. Don't mind the low page speed score it is because I haven't done any sort of optimizations like serving server scaled images or anything like that at all. This is just the out of the box speed test.

<h5>Github Pages Speed Test</h5>
<img src='{{site.baseurl}}/assets/images/gtmetrix-github.jpg'>
It is the exactly same web page and it took 2.0 seconds to load which is not in any means is slow. But in comparison netlify achieved 1.3 seconds. 

<h4>dotcom-monitor </h4>

<h5>Netlify speed test result</h5>
<img src='{{site.baseurl}}/assets/images/dotcom-netlify.jpg'>
It is the same web page. The average first time visit took 2.3 seconds where as a second time visit took 1.3 seconds which is one second less compared to first time visit. It is probably because when the site was visited first time the cdn cache might have been empty. But during the second visit probably everything was served from the cdn cache.

<h5>Github Pages Speed Test</h5>
<img src='{{site.baseurl}}/assets/images/dotcom-githubpages.jpg'>
It is the exactly same web page. Here the average first time visit took a big 4.6 seconds which is slow and the average second time visit took only 634.4 ms which is very fast.

But here we have to give the point to netlify because netlify version of the site took only 2.3 seconds for first time visit which is fast and github pages version took twice as long. The reason for giving point to netlify is that netlify managed to load the site in a average time of 2.3 and 1.3 seconds for the first and second visit respectively.Both were fast. But in the case of github pages version one was extremely fast and other was slow. So I am giving point to netlify in this round.

<h4> Dareboost speed test </h4>

<h5>Netlify speed test result</h5>
<img src='{{site.baseurl}}/assets/images/dareboost-netlify.jpg'>
The time to first byte was 0.15 seconds and start render was 0.87 seconds.The fully loaded time was 2.02 seconds

<h5>Github Pages Speed Test</h5>
<img src='{{site.baseurl}}/assets/images/dareboostspeedtest-github.jpg'>
The time to first byte was 0.12 seconds and start render was 0.47 seconds. The fully loaded time was 2.05 seconds.

The difference is negligible.

<h4>Webpage test Speed Test</h4>

<h5>Netlify speed test result</h5>
<img src='{{site.baseurl}}/assets/images/webpagetest-netlify.jpg'>
<img src='{{site.baseurl}}/assets/images/webpagetest-netlify2.jpg'>
Here it took 3.816s to load. 

<h5>Github Pages Speed Test</h5>
<img src='{{site.baseurl}}/assets/images/github-webpagetest.jpg'>
<img src='{{site.baseurl}}/assets/images/webpagetest-github2.jpg'>
So here it took 3.793 seconds to load the site.
The difference is very small but here github pages did better in Load Time, Speed Index..

<h4> Keycdn Speed Test </h4>

<h5>Netlify speed test result</h5>
<img src='{{site.baseurl}}/assets/images/keycdn-netlify.jpg'>
Here netlify version took only 2.2 seconds which is fast

<h5>Github Pages Speed Test</h5>
<img src='{{site.baseurl}}/assets/images/keycdn-githubpages.jpg'>
Here the github pages version took 3 seconds to fully load.

<h3>Conclusion</h3>

I know some people are going to think that this test was not fair because one version has one request less than the other.But I want to tell you that both websites were deployed from the same github repository so I don't know why that happened. But I don't think it is going to make much of a difference as both pages were the same size. I am not going to say one service lost and the other won.As you can see in most cases the differences very small. For me personally I think Netlify did better.
In the below table the fully loaded times of both the versions are given.

<table style="width: 266px; border-color: black; float: left;" border="2">
<tbody>
<tr style="height: 23px;">
<td style="width: 136px; height: 23px;">&nbsp;Tool or Service used</td>
<td style="width: 54px; height: 23px;">&nbsp;Netlify</td>
<td style="width: 75px; height: 23px;">&nbsp;Github Pages</td>
</tr>
<tr style="height: 23px;">
<td style="width: 136px; height: 23px;">&nbsp;Chrome Inspector</td>
<td style="width: 54px; height: 23px;">&nbsp;3.78s</td>
<td style="width: 75px; height: 23px;">&nbsp;4.57s</td>
</tr>
<tr style="height: 23px;">
<td style="width: 136px; height: 23px;">&nbsp;Pingdom</td>
<td style="width: 54px; height: 23px;">&nbsp;475ms</td>
<td style="width: 75px; height: 23px;">&nbsp;522ms</td>
</tr>
<tr style="height: 23px;">
<td style="width: 136px; height: 23px;">&nbsp;GTmetrix</td>
<td style="width: 54px; height: 23px;">&nbsp;1.3s</td>
<td style="width: 75px; height: 23px;">&nbsp;2.0s</td>
</tr>
<tr style="height: 23px;">
<td style="width: 136px; height: 23px;">&nbsp;dotcom-monitor</td>
<td style="width: 54px; height: 23px;">&nbsp;2.3s,1.3s</td>
<td style="width: 75px; height: 23px;">&nbsp;4.6s,634.4ms</td>
</tr>
<tr style="height: 23px;">
<td style="width: 136px; height: 23px;">Dareboost</td>
<td style="width: 54px; height: 23px;">2.02s</td>
<td style="width: 75px; height: 23px;">2.05s</td>
</tr>
<tr style="height: 23px;">
<td style="width: 136px; height: 23px;">&nbsp;Webpage Test</td>
<td style="width: 54px; height: 23px;">&nbsp;3.816s</td>
<td style="width: 75px; height: 23px;">&nbsp;3.793s</td>
</tr>
<tr style="height: 23px;">
<td style="width: 136px; height: 23px;">&nbsp;Keycdn Speed Test</td>
<td style="width: 54px; height: 23px;">&nbsp;2.2s</td>
<td style="width: 75px; height: 23px;">&nbsp;</td>
</tr>
</tbody>
</table>
<!-- DivTable.com -->

<p>Feel free to pick your own winner. For my use cases I think Netlify is the winner. This site you are reading now is hosted on Netlify.</p>

The featured image on the top was from pixabay. Image by <a href="https://pixabay.com/users/bsdrouin-5016447/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2402637">Bethany Drouin</a> from <a href="https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2402637">Pixabay</a> 
















