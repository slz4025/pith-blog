---
title: "Adding Basic Functionality to the Test Object"
date: "2020-06-14"
author: "Christian Broms"
summary: "We've begun to integrate some of the functionality from last week's post into the test object. At the moment the goal is to keep the development focused on getting the essential features roughly implemented, and then coming back later and adding a minimum amount of styling to increase the functionality of the prototype as an object to be evaluated by our testers."
---

We've begun to integrate some of the functionality from [last week's post](/posts/test-object) into the test object. At the moment the goal is to keep the development focused on getting the essential features roughly implemented, and then coming back later and adding a minimum amount of styling to increase the functionality of the prototype as an object to be evaluated by our testers. Be warned, the aesthetics are _very_ rough at this stage—we have yet to consider the UI much at all.

# Functionality

## Creating a new post

![](/images/basic.png)

[As we've previously discussed](/posts/conversational-design), blocks are the most atomic elements in Pith. They're what every post is comprised of, and they're what's transcluded between posts. When creating a new post, the editor allows the user to create multiple blocks. The operation for creating a new block is a newline, and the operation for deleting one is hitting delete with the cursor at the beginning of the block. There are other operations available such as splitting a block's content in the center with a newline and creating two separate blocks. Here's what that process looks like:

![](/images/basic-1.gif)

Once posted, posts appear in the discussion sequence, with the latest posts appearing at the bottom. We currently don't have any notion of a "user" other than the client's IP address, so the only information that is shown on a post is its content.

## Tagging blocks

Each block can be tagged by anyone once it's posted. Here's what that looks like:

![](/images/basic-2.gif)

These changes are reflected immediately across everyone's discussion views.

## Saving blocks

Each block can be saved to a user's library. We're still exploring what this means; read more about this in [Considering Searching](/posts/considering-seraching).

# How it's built

We're using React for the client and a python server for the backend. We're using [socket.io](http://socket.io) to interface between the two. This allows for some very nice near-real time updates between clients—here are two separate clients side-by-side showing the immediate changes when a post is created or tag is added:

![](/images/basic-3.gif)

The latest progress can be found in the [client repository](https://github.com/rainflame/pith-client) and the [server repository](https://github.com/rainflame/pith-api).
