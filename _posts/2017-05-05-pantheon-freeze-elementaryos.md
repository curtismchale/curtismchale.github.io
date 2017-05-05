---
layout: post
title: Vim freezes in Pantheon Terminal on Elementary OS
date: 2017-03-29 10:30:00 -0800
categories: vim, pantheon, elemantaryos
---

Here I am writing in Vim and my terminal freezes. Like many people I'm at least
partially programmed to press `Ctrl + S` to save a file. Seems in Pantheon (and
many other terminal applications) this actually stops the screen output of the
terminal.

So there you sit looking at a terminal with nothing responding. You thought you
were saving...but nope.

Turns out there is an eazy fix. Press `Ctrl + Q` and you're good to go. The
terminal session will start working again and you're off to the races.

