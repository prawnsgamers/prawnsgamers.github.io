---
#Title and Zone:
title: Sitemap
zone: Prawnsgame

#Path and Metadata
folder: 
permalink: /sitemap/
layout: default
description: The sitemap of prawnsgame.org.uk. This contains a hierarchically ordered list of all the pages on prawnsgame.org.uk for human reading.
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

This sitemap is meant primarily for human reading, and is therefore presented as a .html document. An unformatted [sitemap.xml](/sitemap.xml) file is available for machines on this site, though the one hosted here is slightly less likely to be fully up-to-date in comparison with this one: [sitemap.xml]({{ site.baseurl }}/sitemap.xml).

[Main Site (Prawnsgame Zone)](/)
================================

 - [Home](/) *The home page of the entire site.*
 - [About](/about/) *A little information about this site and the people behind it.*
 - [Blog](/blog/) *This site's blog, where we put all our news and updates. Not that individual blog posts are listed below, in the blog section.*
 - [Contact Us](/contact/) *This site's overall contact page, for how to reach us.*
 - [Sitemap](/sitemap/) *This page. Nothing new here. (Actually, that's not true 100% of the time.)*
 - [Copyright](/copyright/) *The copyright notice. Please pay attention to it before copying things.*

[Prawns Site (Prawns Zone)](/prawns/)
=====================================

 - [Home](/prawns/) *The home page of the Prawns subsite.*
 - [Rules](/prawns/rules/) *More than enough information to let you be able to play the brilliant game of Prawns.*
 
[Kalamala Site (Kalamala Zone)](/kalamala/)
===========================================

 - [Home](/kalamala/) *The home page of the Kalamala subsite.*
 - [Rules](/kalamala/rules/) *The rules page for Kalamala. Select which ruleset you need.*
    + [Quick Rules](/kalamala/rules/quick/) *The quick rules: ideal for use as a basic reference, memory-jog, or argument settler.*
    + [Short Rules](/kalamala/rules/short/) *The short rules: realy only of academic interest, a sort of competition.*
 - [Play](/kalamala/play/) *The page where you'll so be able to play the exciting game called Kalamala in your browser.*
    + [Proto-Game](/kalamala/proto/) *A sneak peek at what's coming - we had this game thrown together, even though it doesn't yet have all the features.*

[Blog Posts](/blog/)
====================

{% for post in site.posts %}
 - [{{ post.title }}]({{ post.url }}) *{{ post.date | date: "%b %-d, %Y" }}*
{% endfor %}