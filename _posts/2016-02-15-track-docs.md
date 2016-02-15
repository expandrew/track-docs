---
layout: page
title: "Documentation Site"
category: doc
date: 2016-02-15 10:52:12
order: 4
---

[**track-docs**](http://github.com/expandrew/track-docs) is the documentation site for the **expandrew/track** project.

It runs on [Jekyll](http://jekyllrb.com) and is hosted with [GitHub Pages](http://pages.github.com) at [http://docs.expandrew.com](http://docs.expandrew.com).

### Run the documentation site locally

~~~bash
cd ~/Code/track/docs
gem install jekyll
jekyll serve
~~~

### Create a new page on the documentation site

Use the generator below to create new pages:

~~~bash
cd ~/Code/track/docs
ruby bin/jekyll-page "Some Page Title" ref
# "ref" is the "section" under which the post will be filed
cd _pages/ && ls -la
# the new page will be in this directory; open it in a text editor and begin editing
~~~

Page "sections" are defined in the `_config.yml` file.



