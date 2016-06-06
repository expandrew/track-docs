---
layout: page
title: "Front End"
category: doc
date: 2016-02-15 11:21:38
order: 1
---

[**track-frontend**](http://github.com/expandrew/track-frontend) is the front end layer for the **expandrew/track** project.

### Setup

The first iteration is bootstrapped from the Yeoman [gulp-angular generator](https://github.com/Swiip/generator-gulp-angular):

~~~bash
# pwd is ~/Code/track/frontend
$ npm install -g yo gulp bower
$ npm install -g generator-gulp-angular
$ mkdir angular && cd $_
$ yo gulp-angular
~~~

### Local Development

Run the server with the following:

~~~bash
# pwd is ~/Code/track/frontend/angular
$ gulp serve
~~~

### Reference Articles

#### Authentication

- [Where to Store your JWTs – Cookies vs HTML5 Web Storage](https://stormpath.com/blog/where-to-store-your-jwts-cookies-vs-html5-web-storage)
- [Opinionated AngularJS - Techniques for authentication in AngularJS applications](https://medium.com/opinionated-angularjs/techniques-for-authentication-in-angularjs-applications-7bbf0346acec#.j42u7pss8)
