---
title: 'Build error at "Setup Ruby" stage of Build and Deploy on Actions'
author: Richard Koranteng
date: 2025-02-28 15:00:00 -0600
description: I got this error while 
categories: [Agile Transformation]
tags: [agile]
img_path: /assets/screenshots/agile-transformation
image:
  path: cover.jpg
  width: 100%
  height: 100%
  alt: Agile Transformation Series
---

## Issue

I recently tried to push updates to my GitHub Pages hosted site and got the following error at the 'Build' stage.
```
Run ruby/setup-ruby@8575951200e472d5f2d95c625da0c7bec8217c42
  with:
    ruby-version: 3.1
    bundler-cache: true
    cache-version: 0
Error: The current runner (ubuntu-24.04-x64) was detected as self-hosted because the platform does not match a GitHub-hosted runner image (or that image is deprecated and no longer supported).
In such a case, you should install Ruby in the $RUNNER_TOOL_CACHE yourself, for example using https://github.com/rbenv/ruby-build
You can take inspiration from this workflow for more details: https://github.com/ruby/ruby-builder/blob/master/.github/workflows/build.yml
$ ruby-build 3.1.4 /opt/hostedtoolcache/Ruby/3.1.4/x64
Once that completes successfully, mark it as complete with:
$ touch /opt/hostedtoolcache/Ruby/3.1.4/x64.complete
It is your responsibility to ensure installing Ruby like that is not done in parallel.
```