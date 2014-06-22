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
<div>
<a href="{{ site.url }}{{ post.url }}">
<p>{{ post.date | date: "%b %-d, %Y" }}</p>
<h2>{{ post.title }}</h2>
</a>
<div>
{% endfor %}

<!--<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>-->
