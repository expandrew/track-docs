---
layout: default
title: "Home"
---

## track-docs

This is the public documentation site for the [**expandrew/track**](http://github.com/expandrew/track) project.

This page is primarily for my personal use. I am using this site to record the steps I have taken to set up my environment and application, in the case of needing to repeat these steps on other projects in the future.

Check out the [what]({{ site.baseurl }}/about/what.html) page for general project information.

### Development Shortcuts

#### Open the Sublime Project

~~~bash
cd ~/Code/track
subl track.sublime-project
~~~

#### Running Development Servers

**API**

~~~bash
# pwd ~/Code/track/api/
$ heroku local
# runs on http://localhost:5000
~~~

**Docs**

~~~bash
# pwd ~/Code/track/docs/
$ jekyll serve
# runs on http://localhost:4000
~~~

**Frond End**

~~~bash
# pwd ~/Code/track/frontend/angular/
$ gulp serve
# runs on http://localhost:3000/
~~~

### Setup Repositories

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
