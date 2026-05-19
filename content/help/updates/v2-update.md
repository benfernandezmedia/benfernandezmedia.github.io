---
title: The official website has got the 2.0 upgrade!
date: 2026-05-04
authors:
  - name: Benjamin Fernandez
    link: https://instagram.com/benfernandezmedia
    image: https://github.com/benfernandezmedia.png
sidebar:
  hide: true
tags:
 - updates
---

![Update](/images/help_index/recentchanges.webp)

Our website has been improved, fixed, and of course upgraded to version 2.0! I have been doing a lot of hard work to ensure that everything doesn't break during the publishing process but the good thing is that everything you see has no errors! *Yare yare daze...*

<!--more-->

## New Features (and also some pages)

### New Pages: Help and Information and of course...a changelog

In the previous version of the site, you had only the {{< icon "question-mark-circle" >}}**Questions and Answers** page where I answers some questions that some people might ask me, but now on version 2.0, a new help index has been added where it leads you to the new additional pages and one of those pages is the brand new **Recent Changes** blogset where all posts related to website updates **including this update post** will be shown from there!

### OpenGraph Implemented

When the site was published initially, it had no social link previews as if the links to my site was shared. In this new upgrade, OpenGraph was finally implemented! Now, as you share a link from the website, you will properly see a preview image from the website, although some pages may have different preview images based on page contents.

Here are some examples:

{{< cards cols="2">}}
  {{< card image="/images/social_preview.png" title="Generic Preview Image" subtitle="This will be used globally throughout the website!" >}}
  {{< card image="/images/help_index/qna_social_preview.png" title="Help Preview Image" subtitle="Some help pages will have its own preview image." >}}
{{< /cards >}}

By properly adding a description in the page's markdown file, it will be translated into metadata for the social preview or SEO to read.

```{filename="metadata.md"}
---
title: Example
description: This is just an example description.
images:
  - /path/to/social_preview.png
---
```

*Personally, in the future, I need to create dyanimic social preview images by doing some generation programming using the assets folder in my site workspace. It's not AI work, but it has to do with manipulating with some image files and data from a blog post and reuse them dynamically. **But it's gonna be very hard to do so!***

### The Characters Have Joined As Authors

*Before I had this idea of using my characters as authors for the website, this was based off the time I used my mascot as a Discord webhook to treat it a hostess of a concepted newsletter that pushes an embed to a channel in a Discord server. Now, I decided to use all of the characters and give them specific roles as authors!*

**NOTE:** Since Madeline is still new, although she has appeared twice as herself and in her Spooky Girl persona, she will not appear as an author but she will have the chance in the future.

The following characters who will appear as authors on the site has a role tied for them:

| Icon | Character Name | Role |
| ----------------------------------- | -------------- | ---- |
| ![Amira](/images/authors/amira.png) | Amira Fernandez | You may seen her everywhere along with the other two characters. Amira shares updates regarding what's going on for new content that I'm posting on my socials. |
| ![Rachel](/images/authors/rachel.png) | Rachel Jordan | Rachel sometimes posts extra content if I have extra or unused content. |
| ![Crystal](/images/authors/crystal.png) | Crystal Ashiro | For the first time, Crystal will be the hostess of a new thing on the website called MediaPlay! An exclusive way to share insights of what's going on in the world of online entertainment such as indie animations, gaming, and much more! |

## Fixes and Improvements

- Fixed and added some icons that was not included with the Hextra theme. This includes icons that were needed in parts of the Navigation Bar.
- The homepage, which is the first page you enter the site with, has been revamped from the ground up, added new visual improvements alongside!
- Favicons has been replaced to ensure that our branding is updated to be par with the system theme.
- RSS support has been fixed! You can now add the site to your RSS feeder of choice.

## Under The Code

- While working on some parts of the pages like the Questions and Answers and Recent Changes pages, I had to modified the layouts for both list and single pages to display the appropiate banners, it was tough but the modification was successful.
