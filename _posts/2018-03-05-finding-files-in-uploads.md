---
layout: post
title: Finding PHP files in uploads
date: 2018-02-05 10:30:00 -0800
categories: wordpress hack, terminal
---

Been dealing with a persistent hack thing on a few sites I manage. I think I
keep getting closer to a full solution when things happen. Here are a few steps
I've taken to try and get this sorted.

## 1. Install iThemes Security

Specifically turn on the System Tweaks in [iThemes
Security](https://ithemes.com/security/) (not the Pro version). Turn on all the
settings.

I've also made iThemes Security notify me of all the files changes everywhere so
I can track things down.

This does mean I get notified when people upload images, but I've found other
files there as well.

## 2. Find PHP files in uploads

Shouldn't be any of these at all. Using SSH and terminal on my server I was able
to search it for all instances of php files in the uploads directory easily.

`find ./ -type f -name ".php"`

`./` means current directory so make sure you're at the current directory.

`-type f` makes it search through the directory tree.

`-name "*.php"` tells it to return php files. So change that for whatever you're
looking for.

Hopefully we've got things under control now.
