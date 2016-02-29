---
layout: page
title: "Deployment"
category: doc
date: 2016-02-27 15:01:06
order: 6
---

### Deployment

Heroku watches the `production` branches on `expandrew/track-frontend` and `expandrew/track-api` and triggers a deployment whenever changes are merged in.

- Make a pull request from `master` to `production` in either repository 
  - Title the pull request with the date and deployment number for that day (`20160227.1`)
  - enumerate the feature changes in description of the pull request
- Heroku detects the merged pull request and will trigger a build and deployment
  - Heroku detects Node.js and runs `npm install`
    - My `package.json` files have [postinstall scripts](https://docs.npmjs.com/misc/scripts) that trigger the build tasks (`bower install && gulp build`) - check out the `scripts: { ... }` sections of each `package.json` file to see what's happening
  - Repository/branch configuration lives in the Deploy tab on the app's Heroku Dashboard
  - Deployment progress is available on the app's Heroku Dashboard under the Activity Feed

#### Notes for me

- *setting up CircleCI to watch the branch and trigger deployment after a successful test is more trouble than it is worth*
  - when the time comes to set up testing with a CI service, use CircleCI (but don't use it to deploy to Heroku) then turn on Heroku's "Wait for CI to pass before deploy" feature on the Deploy tab in the Automatic Deploys section. 
  - Don't trigger the deployment from CircleCI (this was a pain in the ass and I spent all weekend trying to get it to work optimally, but I couldn't find a configuration that satisfied me)

### "Releases"

- Update submodule references in the `expandrew/track` repository and commit to `master`
- Make a [new release](https://github.com/expandrew/track/releases/new) with a tag like `v0.0.0` (use [Semantic Versioning](http://semver.org/))
