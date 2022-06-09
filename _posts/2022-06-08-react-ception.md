---
layout: post
title: React-Ception
permalink: /react-ception/
date: 2022-06-08
---

Recently, my work as a consultant has involved an effort to re-architect our frontend website. Previously, the website was a static site, stored and served from an AWS S3 bucket, and it used React for its UI library. Nothing too fancy.

The new approach, by contrast, is a really cool combination of React techniques (especially w/ concern to React routing), low-level DOM API methods, and the [CustomEvent](https://developer.mozilla.org/en-US/docs/Web/API/CustomEvent/CustomEvent) interface. In a future post, I'll share a link to a proof of concept repository I toyed with while getting it all together.

In a phrase, the new approach could be summarized as "react-ception" - the practice of tying multiple, distinct React applications on the same web page together - including some that may be loaded over the network (similar to "runtime" or "dynamically-loaded" components, except these are entire React applications that co-exist after DOM injection).

The tech stack I used to achieve this includes

* React 17
* React Router (v5)
* TypeScript
