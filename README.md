prawnsgamers.github.io
======================

The Prawnsgame Official Site Repository

-------------------------------------------------------------

Can be edited using Git (both web, console, and app) and Prose.
Markdown is prefferred on most pages, the exceptions being pages that need high levels of HTML, custom CSS, or Javascript (such as /kalamala/proto/), and the site's main page (index.html).

The site's pages is actually hosted on Hostinger, but it pulls content from here as necessary.

Hostinger currently has four files live:

 - .htaccess <-- This parses the url from the user and passes it to index.php
 - index.php <-- This understands their request and gets the right content from github-pages
 - robots.txt <-- This allows access to the relevant pages for search engines
 - sitemap.xml <-- This is a list of pages for search engines

Unfortunately these four pages haven't yet been programmed to act upon pages that aren't HTML (Jekyll/github-pages convertd .md and .markdown to .html).

This means that for external resources (such as images or external .css documents), it is necessary to prefix the src or href with {{ site.baseurl }}, like this:

code for an image: *![image description]({{ site.baseurl }}/images/example.png)*

Links to pages should be done as usual, with external links starting with http:// and internal links starting with the root directory / 
