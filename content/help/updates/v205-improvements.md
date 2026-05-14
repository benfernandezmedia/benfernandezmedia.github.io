---
title: v2.0.5 - Improvements and Fixes
description: Small improvements and overall fixes for the website.
images:
  - /images/help_index/social_preview.png
date: 2026-05-14
authors:
  - name: Benjamin Fernandez
    link: https://instagram.com/benfernandezmedia
    image: https://github.com/benfernandezmedia.png
sidebar:
  hide: true
tags:
 - Updates
---

![Update](/images/help_index/recentchanges.webp)

*Small improvements and overall fixes for the website, mainly focused on file cleanup and RSS feed fixes.*

<!--more-->

## New Features

*No new features for this changelog.*

## Fixes and Improvements

- Fixed RSS feed outputs for the main website, and updates posts.
- Decluttered folders that holds the tags for every posts, keeping it at a small digital footprint.
- Version 2.0.5 introduces overall improvements of website experience and stability.

## Under The Code

When observing my site code, I discovered that most of the tags that were placed in the public folder, had a lot of index.xml files for the RSS feed. In order to declutter, I had to add some outputs for specific pages that it can only focus for articles that appears in the RSS channels.
