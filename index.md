---
layout: default
title: "Home"
---

## track-docs

This is the documentation site for the **expandrew/track** project.

Check out the [what]({{ site.baseurl }}/about/what.html) page for general project information.

### Get started

Clone the main project repo ([`expandrew/track`](http://github.com/expandrew/track)) then update the submodules.

~~~bash
cd ~/Code
git clone git@github.com:expandrew/track
cd track
git submodule init
git submodule update
~~~

Alternatively, you can specify `--recursive` when you clone, and the submodules will be automatically updated.

~~~bash
git clone --recursive git@github.com:expandrew/track
~~~