# Website

This repo contains the source to our homepage hosted at https://faudroids.github.io. 

## Writing posts and creating pages

The webpage uses [Jekyll](http://jekyllrb.com) combined with [Poole](http://getpoole.com) and the [Hyde](http://hyde.getpoole.com/) theme to render its content. 

To publish content simply commit and push the changes to this repository and GitHub takes care of actually hosting the site.

When writing new posts and setting the `author` variable in the front matter block, Jekyll will look for a matching author in the [\_config.yml](https://github.com/FauDroids/FauDroids.github.io/blob/master/_config.yml) to display the full author name below the post title. For example the post

```
---
layout: post
title: My first post
author: bob
---
```
would look for an author object called `bob` in the config file and get the corresponding full name.


## Adding team members 

The team site contains a generated list of all the team members that are currently working on one of the projects. New members can be added by editing the [\_data/members.yml](https://github.com/FauDroids/FauDroids.github.io/blob/master/_data/members.yml) file. The following options are available:

- `name` of member which will be displayed below posts and on the team page
- `gravatar` small profile image shown next to the name
- `role` short description of what the team member is doing (e.g. Software Developer, Testing, Marketing, ...)
- `message` custom text which is displayed on the team page
- `email`, `github` and `homepage` optional contact information
