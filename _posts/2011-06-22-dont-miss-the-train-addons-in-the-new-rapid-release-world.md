---
id: 71
title: 'Don&#8217;t miss the train &#8211; addons in the new rapid release world'
date: 2011-06-22T22:41:35+00:00
author: Stephanie Daugherty
layout: post
guid: http://stephaniedaugherty.wordpress.com/?p=71
permalink: /dont-miss-the-train-addons-in-the-new-rapid-release-world
geo_latitude:
  - 35.928301
geo_longitude:
  - -79.054889
geo_accuracy:
  - 48
geo_public:
  - 1
categories:
  - addons
  - firefox
  - mozilla
  - rapidrelease
---
_Disclaimer: I&#8217;m not an addon developer, just a concerned end-user that tries to be involved with the Mozilla community and follow the development process. Hopefully this will still make sense._

_Updated June 23: Added links to http://blog.mozilla.com/addons/2011/04/19/add-on-compatibility-rapid-releases/ &#8211; thanks @jruderman for pointing this out_.

Firefox 5 shipped yesterday, on time, the first of many releases on the new, accelerated [rapid release](http://blog.mozilla.com/blog/2011/04/13/new-channels-for-firefox-rapid-releases/ "New Channels for Firefox Rapid Releases") schedule.

There&#8217;s been a lot of talk of rapid release being a negative for users, particularly due to addon compatibility. While it&#8217;s certainly a valid concern, it&#8217;s not as bad of a situation as it appears on the surface. The Mozilla developers, in particular the [Addons.mozilla.org](http://addons.mozilla.org "Mozilla Addons") team have been doing a lot to prepare for rapid release and to make the transition less painful for both users and addon developers. The addons team has even put an automatic compatibility update in place that [finds addons that will work](http://blog.mozilla.com/addons/2011/04/19/add-on-compatibility-rapid-releases/) and marks them compatible early in the release cycle.

<!--more-->

**Help! My Addons aren&#8217;t updated!**

First of all, keep in mind this was the first release under the new schedule, and developers are still adjusting to the new cycle. The AMO team introduced an <a href="http://blog.mozilla.com/addons/2011/04/19/add-on-compatibility-rapid-releases/" target="_blank">automatic compatibility updating system</a> in  time for this release, so most addons were updated even without any special effort from addon developers.

If the addon you need is hosted on addons.mozilla.org and it wasn&#8217;t updated, it probably didn&#8217;t pass the compatibility  checks &#8211; hopefully it&#8217;s developer will release an update soon, if not, there&#8217;s a link to contact the author on the addon page at AMO. If that fails, chances are, you may also be able to find another addon that provides the same functionality.

If the addon you need is hosted elsewhere, then it&#8217;s quite likely that it&#8217;s compatible, but just hasn&#8217;t been updated yet. There were very few changes between 4.0.1 and 5 that would have affected addon compatibility, so you can try to load it anyway by telling Firefox to skip compatibility checks. The easiest way to do that is by installing [Add-on Compatibility Reporter](https://addons.mozilla.org/en-US/firefox/addon/add-on-compatibility-reporter/ "Add-on Compatibility Reporter"). Add-on compatibility reporter does two important things. First of all, it turns off the version checking for addons, so that you can load addons that aren&#8217;t marked by the developer as being compatible with the version you are using, and second, it provides a &#8220;compatibility&#8221; button next to each addon in the addons manager that you can use to send feedback to the developer about whether or not the addon works in your version of Firefox. This is important, because it helps addon developers know whether or not their addons are working, and also because the AMO team plans to use the feedback in the future to improve on the automatic compatibility updating process.

A special note regarding addons included with your antivirus software. Antivirus vendors have been slow to update in the past, but antivirus software should still protect you with or without an addon. Make sure real-time scanning is still enabled, and you&#8217;ll still be protected.

I expect that in the future, once developers get used to rapid release, almost all addons will be updated in time, so hopefully by the time Firefox 6 releases we&#8217;ll see a huge improvement in addon compatibility on release day.

**Why this is really a blessing in disguise for developers&#8230;**

(Or whaaaat? I have to worry about new releases every 6 weeks now?!?!!)

For addon developers, rapid release seems like a scary, frustrating mess but it really doesn&#8217;t have to be. Sure,  we&#8217;re looking at a new Firefox every 6 weeks once the cycle is fully underway, but we&#8217;re also looking at a few big improvements for addon developers. Faster releases mean smaller releases, and regular releases mean a predictable cycle &#8211; just like a train timetable &#8211; just don&#8217;t miss the train.

**AMO maxVersion Bumping**

If your addon is hosted at addons.mozilla.org, all you&#8217;ll have to do in most cases is watch for the <a href="http://blog.mozilla.com/addons/2011/04/19/add-on-compatibility-rapid-releases/" target="_blank">version bump</a> to happen.

**Smaller Releases**

There&#8217;s only 6 weeks of heavy, active development in the new release cycle, which means each release will be smaller. The development team has committed to documenting the changes in each release that affect extension compatibility. This documentation not only highlights what to change, but also highlights what to test against, allowing developers to focus testing on specific areas.

**Predictable Releases**

Now that releases won&#8217;t be waiting on features to ship, but instead will ship at regular intervals, it&#8217;s easier to plan ahead so that you don&#8217;t miss a release.

**12 Week Testing Window**

The rapid release formula is to shift each channel closer to release every 6 weeks. Development happens constantly on mozilla-central, and every 6 weeks mozilla-central is merged over to the Aurora channel. Aurora is designed to be &#8220;mostly&#8221; stable &#8211; generally only backouts and pref-offs will show up in aurora. After 6 weeks, aurora shifts to beta, where it&#8217;s practically frozen for 6 weeks &#8211; only bug fixes needed to ship are likely to land on beta. This means 12 solid weeks to test, and _any addon that&#8217;s working in the beta is ready to be marked compatible with the release_.

**New SDK**

Mozilla brought out a new [Addon SDK](https://addons.mozilla.org/en-US/developers/builder) in time for Firefox 5, which makes it easier to develop addons that will work with both current and future versions of Firefox. As a bonus, addons built on top of the new SDK are restartless by default.

**Less risk of &#8220;last minute&#8221; changes**

In the old development model, changes continued to slip in almost up to the release, as developers tried to beat the release deadline to avoid waiting up to a year to ship a high priority feature. In the rapid release world, releases are time based, so the deadline is actually 6 to 12 weeks back from release date &#8211; and there&#8217;s another one coming up just a few weeks later, so last minute changes should be a thing of the past.

**Summary**

  * Releases are smaller &#8211; less to test, less to break.
  * Changes are better documented &#8211; easier to make addons compatible.
  * Releases are predictable &#8211; extension developers know when Firefox will ship and can treat release dates as compatibility deadlines.
  * What works on the Firefox Beta will work on the release.
  * New Addon SDK makes addon development and compatibility less hassle.
  * 12 weeks to develop and test for each new release &#8211; plenty of time to catch the train.
  * Last minute addon-breaking changes should be a thing of the past.

This seems like a net win for addon developers to me, even though it may take some getting used to. Just don&#8217;t miss the release train, and it will be a better Firefox world for everyone 🙂