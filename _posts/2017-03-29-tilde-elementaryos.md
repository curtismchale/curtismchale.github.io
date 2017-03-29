---
layout: post
title: Getting your Tilde key back on your Mackbook Air 13" with ElementaryOS
date: 2017-03-29 07:00:00 -0800
categories: ElementaryOS, linux,
---

I'll write a bit more about why I'm switching to Linux in the future, but for today I'm going to solve a problem with the tilde (~) key in ElementaryOS.

Out of the box with the Dvorak keyboard when you press the ~ key you actually get > which is not what you want. It means I can't really type the root path to my Home directory easily.

It's just a pain in the butt.

Since ElementaryOS is based on Ubuntu you'll find a bunch of solutions out there. One that seems to work for many people, but not me is to use the following code in your `/etc/rc.local` file.

`echo 0 > /sys/module/hid_apple/parameters/iso_layout`

As I said, that didn't change anything for me in ElementaryOS. But there is still a solution.

You need to 'switch' keys 49 and 94 by setting the 'badmap' in the keyboard settings. Using the command below 'fixes' it but isn't persistent in my experience.

`setxkbmap -option apple:badmap`

To make it persistent edit `/etc/default/keyboard` and set `XKBOPTIONS="apple:badmap"`.

With this in hand on ElementaryOS or Ubuntu 16.04LTS you should be able to type your ~ key.

You can see the official bug [here](https://bugs.launchpad.net/ubuntu/+source/linux/+bug/1245081).
