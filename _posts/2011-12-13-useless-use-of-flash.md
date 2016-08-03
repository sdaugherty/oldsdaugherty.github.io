---
id: 85
title: Useless use of flash
date: 2011-12-13T07:42:52+00:00
author: Stephanie Daugherty
layout: post
guid: http://stephaniedaugherty.wordpress.com/?p=85
permalink: /useless-use-of-flash
draftfeedback_requests:
  - 's:121:"a:1:{s:13:"4e2c63e4300c0";a:3:{s:3:"key";s:13:"4e2c63e4300c0";s:4:"time";s:10:"1311532004";s:7:"user_id";s:7:"4471717";}}";'
geo_latitude:
  - 35.928301
geo_longitude:
  - -79.054889
geo_accuracy:
  - 48
geo_public:
  - 1
publicize_results:
  - 'a:1:{s:7:"twitter";a:1:{i:11588052;a:2:{s:7:"user_id";s:14:"stephdaugherty";s:7:"post_id";s:18:"146495289010823168";}}}'
categories:
  - Uncategorized
tags:
  - standards
  - web development
---
Once upon a time, the renowned Perl wizard <a class="zem_slink" title="Randal L. Schwartz" href="http://www.stonehenge.com/merlyn/" rel="homepage">Randal L. Schwartz</a> used to issue a series of &#8220;<a class="zem_slink" title="Cat (Unix)" href="http://en.wikipedia.org/wiki/Cat_%28Unix%29" rel="wikipedia">useless use of cat</a>&#8221; awards to posters on the usenet newsgroup comp.unix.shell that abused the &#8220;cat&#8221; utility for purposes other than which it was intended.

The classic UUoC was something like:

<pre>$ cat file | grep foo</pre>

The UUoC awards highlighted the most egregious misuses &#8211; the cat utility is designed for concatenating two files, not for display of a single file, and certianly not as the first stage of a pipe.

On the modern web, we see similar occurrences with Flash in websites, where it has no business being used.

Flash is useful when it does something that web standards either can&#8217;t do, or can&#8217;t do easily. Flash is useless when it adds nothing to the content of the site that can&#8217;t be duplicated with a few lines of JavaScript and CSS.

Interacting with webcam and microphone? Useful.

Embedding a video game into a web page? Useful.

Performing rollover effects on a link? Useless.

Playing a slideshow? Useless.

Displaying advertising? Useless.

Playing video? Still useful. (But on the way out, thanks to HTML5 video).

Useless use of flash is a more serious violation than useless use of cat ever was &#8211; instead of costing you a process, it costs every visitor to your website a process, along with the memory that goes with it. It also costs accessibility &#8211; assistive technologies like <a class="zem_slink" title="Screen reader" href="http://en.wikipedia.org/wiki/Screen_reader" rel="wikipedia">screen readers</a> and braille terminals don&#8217;t really work for flash.

Using Flash when it&#8217;s not called for is a demonstration of laziness and incompetence on the part of web designers &#8211; it&#8217;s unprofessional, and it needs to stop.  I&#8217;m going to start highlighting examples of useless use of flash (UUoF) when I see them, in the hope that it will draw attention to the epidemic of poor web design that is a UUoF.

There are many examples out there, and I plan to start showcasing the worst of them here 🙂