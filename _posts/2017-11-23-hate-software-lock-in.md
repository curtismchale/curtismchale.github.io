---
layout: post
title: I hate software lock in
date: 2017-11-30 14:28:00 -0800
categories: macOS, OSX, Linux, Windows
---

At one point this year I spent 6 months on Linux and the biggest problem was
software lock in. Not Linux software lock in, but macOS lock in.

I love Ulysses and Scrivener, but if I want to change my OS to Ubuntu I'm out of
luck with either of those tools.

If I want to change to Windows, Ulysses goes by the wayside.

This sucks. It feels like it's not the way it should be. I know that Scrivener
gave Linux a go, and abandoned the application. It clearly wasn't viable
financially.

This has me thinking, what about building a crossplatform editor? Something that
takes markdown like Ulysses, but has some more power like Scrivener?

Something where I can embed a web page in my 'research' like Scrivener, but it
gets out of the way like Ulysses when I'm working on a project that's not as
complex.

Could it be done? Could I do it?

The first stop is choosing a programming interface. I'd rather go for
crossplatform compatibility instead of native OS perfection so that leaves me
with a few options, but [Electron](https://electronjs.org/) looks like the best
option so far.

No I don't want to hear your whining about Electron and processor usage. If you
want a crossplatform application, there is something that needs to get given up.

So yes, I'll be investigating Electron and what it's going to take to build
myself a writing tool that fits in with what I want. To start, we'll aim for a
markdown editor only. Then we'll introduce folders like Ulysses has so it can be
synced in Dropbox easily.
