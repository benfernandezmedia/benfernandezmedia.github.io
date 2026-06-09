---
title: v3.0 - Welcome to Version 3.0!
description: The website has been officially updated to version 3.0! This major update has major improvements and fixes to the overall website experience.
publishDate: 2026-06-08T20:41:00
authors:
  - name: Benjamin Fernandez
    link: https://instagram.com/benfernandezmedia
    image: https://github.com/benfernandezmedia.png
sidebar:
  hide: true
imageZoom: false
tags:
  - updates
  - website
  - major-release
---
![Update Banner](/images/updatebanners/updatebanner-v3.webp)

After a long development week or two to fix improvements in the overall website experience, it is my pleasure to announce that the website has been officially updated to **Version 3.0!** This update introduces some major changes to the site, including: a new ticker for {{< icon "mediaplay" >}}MediaPlay, improvements to some icons and dark mode, and an **updated layout for the home page!**

As I continue to work on the website to add new features and pages, this can eventually be populated with more content, especially for the MediaPlay newsletter, but for now, let's enjoy what we have in this major update and *see what's new on the official website of BFM!*

## New Features

### Redesigned Home Layout

{{< hextra/feature-grid cols="2" style="margin-top: 14px;" >}}
  {{< card image="/images/old_layout.webp" title="Before the redesign" >}}
  {{< card image="/images/new_layout.webp" title="After the redesign" >}}
{{< /hextra/feature-grid >}}

After doing some research using the {{< icon "code" >}} **Developer Tools** on Chrome, I paid close attention to the image classes that control how both light and dark versions of my logo are viewed when the theme is toggled or how the theme behaves based on how your system is configured for dark mode.

By using `hx:hidden hx:dark:block` for the dark logo and `hx:block hx:dark:hidden` for the light logo, the former text that represents the brand is now replaced with the logo to ensure that the brand is more recognizable! Plus, the icons for the Not By AI badge and the stuff I use to make the site and content have also been updated with their appropriate classes!

For the icons that displayed the skills I use to make the site, I performed some trial and error when programming the icons to switch from light to dark by adding an additional container for the light-themed icons and trying to hide them when the theme is toggled. However, it didn't work until **I found a solution.**

{{< hextra/feature-grid cols="2" style="margin-top: 14px;" >}}
  {{< card image="/images/before_icons.webp" title="Before the redesign" subtitle="Before programming, all of the icons belonging to Skillsicon had a URL to target only that specific icon of choice. When toggling themes, these icons are not 'dynamic'." >}}
  {{< card image="/images/after_icons.webp" title="After the redesign" subtitle="By adding another 'img src' tag into the existing link tag and the classes I used for the logo, when toggling between light or dark, the icons will change to their appropriate theme." >}}
{{< /hextra/feature-grid >}}

### Meet The New MediaPlay Ticker

Have you noticed something different on the ticker that you always see on the home page? Well, that's actually the MediaPlay ticker, where it displays all published articles from the newsletter, and guess what? **The ticker has been redesigned from the ground up!**

![MediaPlay Ticker](/images/new_ticker.webp "Meet MediaPlay Ticker 2.0!")

While the old version of the ticker is considered a prototype, there was an issue when the prototype of the ticker was used...**it was not responsive on smaller devices.** While facing some programming difficulty in retaining the size of the MediaPlay logo, some attempts were made to add a smaller version of the logo to ensure it's simplified, but it underwent unsuccessful attempts due to the complexity of the classes I tried to use for the assets.

For this new ticker, with an additional container to show the logo and its brand-new tagline, the logo functionality remains the same. Clicking on the logo will take you to the MediaPlay page on the website. Also, note that this new ticker is responsive now, and it has been tested with no issues whatsoever.

## Improvements and Fixes

**Version 3.0** introduces the following fixes and improvements, that are aside from the new features that were disclosed in this post, but not limited to the following:

- The {{< icon "rssicon" >}} RSS icon is now in the website's main navigation bar for instant access to our main site's RSS feed.
- The icon for the MediaPlay link on the navigation bar was fixed. Originally, in the previous build, when toggling light theme on, you basically see a straight-up play icon while the 'M' inside the play icon is still black. By redoing the logo design on Figma, this icon has been fixed with the 'M' as a cutout!
- Updated social links and added additional icons in the `icons.yaml` file that will eventually be used in the future.
- Updated the {{< icon "question-mark-circle" >}}**Help and Information** index page, replacing the image that was used on the homepage with the branding image that is used as our OpenGraph image.
- Updated the 404 page; it may be a visual upgrade to align with our main brand's tagline and theme.
- Added fixed time zone as `timeZone: 'America/New_York` to fix the date and time on each blog post that is published to the site, and also updated the `publishDate` on every post.

## Under The Code

When working on the idea to adapt the icons for both dark and light themes of the site, I discovered the classes that were part of the theme, as it uses Tailwind CSS as the prefix and utility classes. I originally thought those classes will apply to containers but it only works on images. Lesson learned!
