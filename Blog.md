---
#Title and Zone:
title: Blog
zone: Prawnsgame

#Path and Metadata
folder:
permalink: /blog/
layout: default
description: The blog for prawnsgame.org.uk, where you can keep track of everything happening to do with prawnsgame.org.uk. Featuring news, game updates (for Prawns and Kalamala), and posts about new site features.
published: true

#Links
link1name: Home
link1path: /
link2name: About
link2path: /about/
link3name: Blog
link3path: /blog/
link4name: Contact Us
link4path: /contact/
---

This blog is where we will be posting any news about website updates, new games or rules, app releases and more! Check back often to see what's going on.

Posts:
======

(Newest to oldest)

{% for post in site.posts %}
<div>
<a href="{{ post.url }}" class="post">
<p>{{ post.date | date: "%b %-d, %Y" }}</p>
<h2>{{ post.title }}</h2>
</a>
<div>
{% endfor %}

<!--<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>-->
