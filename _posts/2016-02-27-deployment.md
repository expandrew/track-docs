---
layout: page
title: "Deployment"
category: doc
date: 2016-02-27 15:01:06
order: 6
---

### Deployment

CircleCI watches the `production` branches on `expandrew/track-frontend` and `expandrew/track-api` and triggers a deployment whenever changes are merged in.

- Make a pull request from `master` to `production` in either repository 
  - Title the pull request with the date and deployment number for that day (`20160227.1`)
  - enumerate the feature changes in description of the pull request
- CircleCI detects the merged pull request and will trigger a build, test, and deployment to Heroku according to the `circle.yml` file in the repo

### "Releases"

- Update submodule references in the `expandrew/track` repository and commit to `master`
- Make a [new release](https://github.com/expandrew/track/releases/new) with a tag like `v0.0.0` (use [Semantic Versioning](http://semver.org/))
