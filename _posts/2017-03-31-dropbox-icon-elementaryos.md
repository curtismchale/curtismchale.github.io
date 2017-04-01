---
layout: post
title: Get Dropbox working on ElementaryOS
date: 2017-03-31 21:31:00 -0800
categories: ElementaryOS
---

Yes if you want to install Dropbox on ElementaryOS you can use the standard [Ubuntu .deb file](https://www.dropbox.com/install-linux). Of course it will work, but you won't have an icon that looks right. In fact, all you'll get is a black square with a red cross through it.

This is because Dropbox doesn't recognize the ElementaryOS theme so it's not pulling in the Unity icons.

While you can edit some files to make it work, there is a much faster way. Grab this [Elementary Dropbox installer from Github](https://github.com/zant95/elementary-dropbox). All you need to do is follow the instructions and you're going to have Dropbox working with the icon you expect.
