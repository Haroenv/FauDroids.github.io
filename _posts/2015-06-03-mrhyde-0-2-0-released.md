---
layout: post
title: MrHyde 0.2.0 released
author: philipp
comments: true
published: false
---

Today we are happy to announce the release of MrHyde 0.2.0, now with image support!

Previously MrHyde was all about text, and text only. While downloading images from a repo wasn't a problem, you could only view and edit the raw bytes, which is ... well, not so awesome. While image support is still very basic, it allows you do add new pictures to repositories (and then include those in posts ...) and preview the result like you normally do. 

Okay, great, what else?

Images were the primary focus of this release, but a number of other features also managed to sneak in. They are:

- Undo / redo operations in the editor
- Optional line numbers in the editor
- Better looking preview server error pages
- Files in repos can be renamed

Nice, what's next?

That depends. At the moment MrHyde is really just a GitHub client with this cool Jekyll preview function, but does not really know anything about Markdown, posts or Jekyll in general. Ideally we want to offer a UI that is very specific to Jekyll, which for example shows the users posts / drafts at one glance or supports common Markdown formatting tasks, instead of forcing users to manually go through the file structure each time. We'll definitely keep the file browser around for a backup because we don't want to limit the edit capabilities of MrHyde, but it's going to be behind a layer of Jekyll specific views.

At the same time we are open for suggests and are actively looking for feedback. So if you know a feature that you would be dying to get your hands on, let us know!