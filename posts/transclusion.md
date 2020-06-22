---
title: "Adding Transclusion"
date: "2020-06-21"
author: "Christian Broms"
summary: "We've recently been working on adding a kind of hyperlinking functionality to the Pith prototype, called transclusion. Often, authors will want to quote a previous post and will cut out a section of it as a reference"
---

We've recently been working on adding a kind of hyperlinking functionality to the Pith prototype, called [transclusion](https://en.wikipedia.org/wiki/Transclusion). Often, authors will want to quote a previous post and will cut out a section of it as a reference. This is a behavior we'd like to encourage in Pith, so we're making it easy with a search that's built into the editor.

![](/images/transclusion.gif)

Transclusion is different than a typical reference in that it includes the original block in the post, rather than a copy of it.

A search happens after a user types a "\" and then a query into the editor:

![](/images/transclusion1.png)

Selecting the suggested block will create a transclusion, where the unique id of the block is included along with a preview of the content:

![](/images/transclusion2.png)

This can create a conversation with many references between blocks:

![](/images/transclusionAll.png)
