---
layout: post
title: Connecting Chassis to Sequel Pro
date: 2018-01-30 14:08:00 -0800
categories: chassis, vagrant, sequel-pro, mysql
---

Needed to connect Chassis to SequelPro this morning. Remembering jumping through
hoops to figure it out when I used VVV, but seems that Chassis has an [easy
SequelPro connector](https://github.com/Chassis/SequelPro).

Clone the respository above into your extensions directory. Make sure you
provision vagrant again with `vagrant provision`.

Type `vagrant sequel` and SequelPro will pop up with the connection set.

Off to the races.
