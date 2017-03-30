---
layout: post
title: Install Zotero Standalone on ElementaryOS
date: 2017-03-30 09:51:00 -0800
categories: ElementaryOS
---

While I loved Evernote for years I have continually felt that they were focusing on features that were of no use to me or to their core market at all. Then when they started heading down a road of looking in to my notes, I was gone.

I was also fully invested in OSX then so I tried and loved [DevonThink Pro](http://www.devontechnologies.com/products/devonthink/overview.html). Unfortunately there is no version of DevonThink that runs on Linux so as I've made the switch to ElementaryOS I've had to look for something new.

The closest thing so far has been [Zotero](https://www.zotero.org/download/).

You won't find Zotero in the AppCenter for ElementaryOS so you'll need to install it from the command line. To get started [read my previous post](https://curtismchale.github.io/no-apt-add-repository-elementaryos/) to make sure you have the `apt-add-repository` command available.

With that command available you can use the following three commands to install Zotero from the ppa source.

```
sudo add-apt-repository ppa:smathot/cogscinl
sudo apt-get update
sudo apt-get install zotero-standalone
```

Now enjoy Zotero for storing your research.
