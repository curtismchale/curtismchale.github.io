---
layout: post
title: ElementaryOS no apt-add-repository command
date: 2017-03-30 09:46:00 -0800
categories: ElementaryOS
---

While ElementaryOS is a derivative of Ubuntu, that doesn't always mean it functions exactly the same out of the box.

While trying to install [Zotero](https://www.zotero.org/download/) I found that the `apt` package manager didn't have the command needed to add a ppa so I could install Zotero.

To add the `apt-add-repository` command to ElementaryOS you need to run this command in your terminal.

```
sudo apt-get install software-properties-common
```

Once you have the common properties installed you can happily go ahead and add new ppa's to your ElementaryOS system.
