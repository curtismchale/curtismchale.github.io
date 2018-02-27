---
layout: post
title: Setting Custom Database Prefix for WordPress in Chassis
date: 2018-02-27 10:30:00 -0800
categories: wordpress, vagrant, chassis
---

Yes you can do it in the root `config.php` file, but you'll run into issues when you try to provision with tools like the great [SequelPro Connector](https://curtismchale.github.io/chassis-sequel-pro/).

Instead create `config.local.yaml` in the root of your Chassis folder.

Then paste in this set of lines:

```yaml
# Database configuration
# (When overriding, include all values)
database:
    name: wordpress
    user: wordpress
    password: vagrantpassword
    prefix: custom_prefix_
```

The last line is your custom database prefix and you should be off to the races.
