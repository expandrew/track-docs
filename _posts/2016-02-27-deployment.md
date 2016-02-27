---
layout: page
title: "Deployment"
category: doc
date: 2016-02-27 15:01:06
order: 6
---

### To deploy

- Commit changes to repositories
- Push each repository to origin
- Update submodule references in the `expandrew/track` repository and commit to `master`
- Push updated `expandrew/track` repository to origin
- Make a pull request from `master` to `production` in the `expandrew/track` repository 
  - Title the pull request with the date and deployment number for that day (`20160227.1`)
  - enumerate the feature changes in description of the pull request
- (CircleCI watches the `expandrew/track/production` branch and runs deploy scripts automatically)
- When things are stable on the production environment, make a [new release](https://github.com/expandrew/track/releases/new) with a tag like `v0.0.0` (use [Semantic Versioning](http://semver.org/))