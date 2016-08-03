---
id: 87
title: The problem with BrowserID and OpenID (and other website registration stuff)
date: 2011-07-15T04:26:00+00:00
author: Stephanie Daugherty
layout: post
guid: http://stephaniedaugherty.wordpress.com/?p=87
permalink: /the-problem-with-browserid-and-openid-and-other-website-registration-stuff
geo_latitude:
  - 35.928301
geo_longitude:
  - -79.054889
geo_accuracy:
  - 48
geo_public:
  - 1
categories:
  - Uncategorized
tags:
  - browserid
  - federation
  - openid
---
Both Mozilla&#8217;s up-and-coming BrowserID technology, and OpenID still have one fatal flaw &#8211; reliance on a single authority.

There&#8217;s no inherent recovery capability in either of these solutions &#8211; in order to be able to put full faith in them, I need to be able to revoke an identity and migrate to a new one at will. BrowserID concentrates the identity on the email address &#8211; which means my identity is in the hands of my ISP, a free mail service, or I have to pay money to host my own mail server. OpenID has the same problem &#8211; my identity is either in the hands of a public web service, or I have to pay to host a site.

Websites that implement their own registration are even worse. They usually rely on the registered email address, and may even revert back to an older email address even after you switch email addresses &#8211; so if your email is compromised, you are SOL.

Ultimate control needs to be firmly in the hands of the user &#8211; in the form of something that can be used to prove you the same person who created an identity, and replace that identity with another, whenever it proves necessary. The information, key, or token to do that needs to be safely in my hands, not with my identity provider.