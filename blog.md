---
#Title and Zone:
title: Blog
zone: Prawnsgame

#Path and Metadata
folder:
permalink: /blog/
layout: default
published: true

#Links
link1name: Home
link1path: /
link2name: About
link2path: /about/
link3name: Contact Us
link3path: /contact/
---

Posts
=====

{% for post in site.posts %}
 > {{ post.date | date: "%b %-d, %Y" }}
 > 
 > [{{ post.title }}]({{ site.url }}{{ post.url }})
 > ================================================
  
{% endfor %}

<!--<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>-->
