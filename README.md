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

Unfortunately these four pages haven't yet been programmed to act upon pages that aren't HTML (Jekyll/github-pages converts .md and .markdown to .html).

This means that for external resources (such as images or external .css documents), it is necessary to prefix the src or href with {{ site.baseurl }}, like this:

    code for an image: ![image description]({{ site.baseurl }}/images/exampleimage.png)

Links to pages should be done as usual, with external links starting with http:// and internal links starting with the root directory / 

    code for an internal link: [link description](/examplepage/examplesubpage/)

    code for an external link: [link description](http://examplesite.com/examplepage/)

Unfortunately this also means that the sitemap doesn't update automatically. To update the sitemap, you should update the github version (both the .xml file and the .md file, unless you have added a blog post, in which case the .md file will auto-update), then contact Daniel to ask him to update it manually. It's not ideal, but it's all we can do for the moment, because otherwise the web thinks that we're cross-site scripting.
