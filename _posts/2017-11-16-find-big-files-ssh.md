---
layout: post
title: Find Big Files or Folders via SSH
date: 2017-11-16 14:30:00 -0800
categories: ssh, ssh-agent
---

Needed to clean up a client server recently that had 10GB of 'stuff' somewhere on the server. Since I had SSH access this was actually super easy. Use:

`du -a -h /home | sort -n -r | head -n 10`

Change `/home` to whatever directory on the server you want to start from and you'll get a list of the 10 biggest files ordered by size.

Then go delete them.

You can find more options [here](https://thomas.vanhoutte.be/miniblog/biggest-file-folder-linux/).
