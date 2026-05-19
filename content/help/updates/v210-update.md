---
title: v2.1.0 - MediaPlay Update
description: This version introduces the new functionality related to our new MediaPlay newsletter which is the brand new homepage ticker and RSS feed, with the addition of improvements to the website.
date: 2026-05-18
images:
  - /images/help_index/social_preview.png
authors:
  - name: Benjamin Fernandez
    link: https://instagram.com/benfernandezmedia
    image: https://github.com/benfernandezmedia.png
sidebar:
  hide: true
imageZoom: false
tags:
  - updates
  - mediaplay
---

![Update](/images/help_index/recentchanges.webp)

*This version introduces the new functionality related to our new MediaPlay newsletter which is the brand new homepage ticker and RSS feed, with the addition of improvements to the website.*

<!--more-->

## New Features

### Introducing the MediaPlay news ticker

![MediaPlay Logo](/images/logo.png)

During last weekend, a lot of hard work has been done on the website to intergrate the new MediaPlay newsletter idea and it has been successfully done by creating a brand new ticker that will display all content related MediaPlay on our homepage for easy access!

When working on the new ticker, that hard work consists of using Chrome's Inspect Element and development tools to shape the look and feel of the ticker and it will be the first thing you will see on the homepage.

Although, this is the first time a long-time HTML tag called `<marquee>` is used, Hugo's code and functionality to display the article title were added so you can access the articles instantly. But for now, since we are writing down the first issue of MediaPlay, you will see Crystal's message that is currently showing on the ticker. As soon as all articles for MediaPlay are populated, **you won't see her message on the ticker any longer.**

In addition to the ticker, the RSS feed for MediaPlay, is now available and we have updated the RSS subscription guide to add the new link to that feed.

## Fixes and Improvements

v2.1.0 introduces the following fixes and improvements to the main website experience:

- Added the {{< icon "mediaplay" >}}**MediaPlay** link to the navigation bar to access the blogset.
- Updated the {{< icon "question-mark-circle" >}}**Help and Information** index to add a card link to the RSS feed guide.
- Fixed some tags on some blog posts everywhere on the site to declutter the folders that have been generated in the site public folder.
- To properly add some credit on source verification based on the media content that is being reviewed on MediaPlay, a new author called **The MediaPlay Team** will be added in the issues that are published on the site.

## Under The Code

When working on the new ticker for MediaPlay, it started off with an idea on Figma, I basically concepted a mockup consisting a bar with the MediaPlay logo on it as the link to the blogset. The trickiest part was designing the bar itself as the bar consists of creating containers to add the logo and the marquee to add the information from the blogset.

Plus, in order to lay it all out to shape the ticker, I used the `background-color` CSS element for the the two container so I can adjust the `max-width` for each container to add the logo and marquee.

While using Visual Studio Code to program the ticker, with some help and assistance of using GitHub Copilot, and proper testing to verify, the ticker was finally working and it will display up to five articles on the feed.