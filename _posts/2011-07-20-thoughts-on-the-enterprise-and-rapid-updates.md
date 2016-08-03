---
id: 94
title: Thoughts on the enterprise and rapid updates
date: 2011-07-20T06:55:00+00:00
author: Stephanie Daugherty
layout: post
guid: https://stephaniedaugherty.wordpress.com/2011/07/20/thoughts-on-the-enterprise-and-rapid-updates/
permalink: /thoughts-on-the-enterprise-and-rapid-updates
geo_longitude:
  - -79.054889
geo_latitude:
  - 35.928301
geo_accuracy:
  - 48
geo_public:
  - 1
categories:
  - Uncategorized
---
Despite the widely held belief that rapid release spells the death of <a class="zem_slink" title="Firefox" href="http://www.mozilla.com/firefox/" rel="homepage">Firefox</a> in the enterprise, I still believe that its a blessing in disguise.

Enterprise apps have been absurdly brittle for years. This in and of itself is a huge risk, but beyond that, its a trap and a money pit. By passing problems down the line we might see lower costs here and now, but in reality we just wrote a whole book of blank checks that will eventually get cashed in one at a time.

Rapid release introduces change into Firefox at a rate that seems staggering, especially to IT departments that are already gunshy about changes from dealing with brittleness all the time.

The only answer to this kind of volatility is to build more robust applications, and to rely on standards rather than release numbers. You see, **standards are a sort of contract with the future** &#8211; you may not know what direction the browser world will take, but in 5 years its a safe bet that the html5 family of technologies will still be there, and that a site using them will still function more or less as intended.

Besides needing to test applications for compatibility though, there are other issues, as Mike Kaply [points out](http://mike.kaply.com/2011/06/24/why-do-companies-need-time-to-deploy-browsers/ "Why Do Companies Need Time to Deploy Browsers? "). Documentation has to be updated, sometimes including a lot of screenshots. Support staff may have to be trained. Deployment plans have to be developed.

These aren&#8217;t minor problems, and I totally agree it&#8217;s a concern. There are a few possible solutions already there, and enterprises have no further to look than Mozilla&#8217;s own development and QA processes for answers. You see, these aren&#8217;t new problems, Mozilla had to address them to even be able to implement rapid release.

Mozilla has a much smaller budget than many enterprise IT departments, but they have a widely used product, that&#8217;s used in an environment that&#8217;s anything but heterogeneous. The &#8220;tier 1&#8221;, or fully supported operating systems include at least 5 different versions of Windows, numerous Linux distributions, and 3 major version of <a class="zem_slink" title="Mac OS" href="http://www.apple.com/macosx/" rel="homepage">MacOS</a> X.  Mozilla also has community support for as many as several dozen other platforms to stay busy &#8211; including <a class="zem_slink" title="Solaris (operating system)" href="http://oracle.com/solaris" rel="homepage">Solaris</a>, <a class="zem_slink" title="FreeBSD" href="http://www.freebsd.org/" rel="homepage">FreeBSD</a>, and <a class="zem_slink" title="OpenBSD" href="http://www.openbsd.org" rel="homepage">OpenBSD</a>, and an emerging mobile effort using the same codebase to support Android and Maemo users.

How do they do that kind of testing within the short time tables of rapid release? Automated testing is a large part of it, but here are some highlights.

The QA process starts with the developers &#8211; strict code review requirements, and a culture that chastises developers for &#8220;breaking the tree&#8221; with code that fails tests. As soon as code is checked in to version control, automated tests start to fire off, with builds for every platform triggering. As soon as a build finishes, automated tests are triggered to assess basic functionality, insure regressions don&#8217;t return, and makes sure performance doesn&#8217;t suffer.

These tests are just a start, tens of thousands of users follow nightly builds and report bugs. The QA team performs verifications as bugs are fixed to validate the fixes. The QA team also performs more automated tests. Both manual and automated tests are crowdsourced also, through [Litmus](http://litmus.mozilla.org "Mozilla Litmus"), and [MozMill Crowd](https://addons.mozilla.org/en-US/firefox/addon/mozmill-crowd/).

As each version moves closer to release through the Aurora and Beta stages, testing efforts become more intense, and the number of users on early versions increases dramatically.

Now, how this applies to the enterprise is that there is no reason why enterprise adopters can&#8217;t benefit from the same automation that Mozilla uses &#8211; in fact, I&#8217;d say by now the [Mozilla QA team](http://quality.mozilla.org/) are automation experts.

[MozMill](https://developer.mozilla.org/en/Mozmill) is a good tool to drive automated testing of Firefox itself. [Selenium](http://seleniumhq.org/) is good to drive automated tests of your web applications themselves. Litmus can be used to drive and organize your manual testing process for both new versions of Firefox and your applications themselves.

MozMill could probably be easily adapted to being used for documentation purposes too &#8211; scripting all the dialogs and dropping screenshots as it goes would make it possible to update screenshots very quickly, and would also validate your documents &#8211; documentation probably doesn&#8217;t need to be changed until the documentation screenshot scripts fail.

Training is still an issue, but it doesn&#8217;t have to be a big issue. The benefit of small, but frequent changes is that the user impact will also be small, so training can just focus on the highlights of the changes.

As it stands now, enterprises will have to start their testing at the moment that a new version enters beta to get 6 weeks of testing time. While this should be enough, that still leaves one major enterprise need &#8211; a backout plan. Right now, they don&#8217;t have it unless they deploy at beta. That&#8217;s understandably unacceptable. N+1 might be realistic for security support for Mozilla, but just as enterprises have a fear of change, Mozilla has a fear of LTS becoming &#8220;the version that won&#8217;t go away&#8221;, as happened with Internet Explorer 6. Remember that Mozilla&#8217;s mission isn&#8217;t market share or necessarily to push a browser &#8211; it&#8217;s to push open web standards forward. Given this mission, having the web be stuck at a particular level of technology goes against everything they stand for.

Hopefully, the rift between the enterprise and Mozilla will work out, and it&#8217;s good to see the Enterprise Working Group back on the radar, but it&#8217;s going to take compromises and ongoing effort on both ends to make this work. Fortunately, being an open source project, enterprise customers don&#8217;t just have to be customers &#8211; they can be developers as well &#8211; and hopefully this encourages them to contribute the resources Firefox needs for more enterprise adoption.

&nbsp;

&nbsp;

&nbsp;