---
title: "Outlining Phase II of Prototyping"
date: "2020-07-06"
author: "Christian Broms"
summary: "Having built a working prototype of the core chat functionality in Pith, we're moving on to the next phase of development in which we will address issues raised with the prototype so far and introduce summarization."
---

Having built a working prototype of the core chat functionality in Pith, we're moving on to the next phase of development in which we will address issues raised with the prototype so far and introduce summarization. Last week we posted [a list of changes](/posts/testing-phase-1) that we'd like to make to the existing prototype given some of the testing we'd done. This week, we're expanding that list to include new features we're developing. Here are the main points that we'll be working through, generally in order:

## Fixing chat bugs

There were a number of bugs and usability issues uncovered from the first round of testing and we'd like to get them taken care of as soon as possible. In particular:

-   Keeping the scroll bar from returning to the bottom of the chat every time a new post is added. Create an alert (as Discord and Signal do) indicating that there are new posts.
-   Preventing a few edge cases where empty blocks could be posted.
-   Giving only the author of a tag the ability to delete it, not anyone in the chat.
-   Tweaking the UI to reduce visual clutter and changing the font to a serif font (we're using Freight Text Pro for all materials related to Pith.)

## Adding replies

The ability to reply to a post directly without having to search for it was a need identified during testing. We're adding the ability to click a "reply to" button on any given block and automatically populate a transcluded block in the post editor.

## Improving contextual search

Currently, searching through content just includes previous posts and blocks, not other contextual metainformation such as tags and time. In this next phase, we will be introducing multiple ways to search. Someone can identity how they'd like to search (by block content, by tags...) and perform a keyword search in the same way as before. A new widget will be designed that facilitates this new kind of interaction.

## Implementing discussion abstraction

In our first prototype, the Pith chat was an isolated piece of the UI independent from the other components of the platform. In reality the chat will serve as one part of the larger ecosystem of the site, where authors might move between discussions in a space we're tentatively calling a _board_, and contribute to summarizing any given discussion in a _summary_ alongside the chat, to be used to make decisions, defer decisions, generate ideas, reduce a problem space, raise new points, and so on.

We'll be implementing discussions that can be created by individuals and can have specific _goals_. A discussion should be a stepping stone in getting to some desired future state and therefore must passively direct participants towards contributing to that state through a predefined goal or desired outcome. Why are we having this discussion? Well, we want to decide on a set of topics for the next meeting. We want to choose a movie. We want to better understand why people disagree on the best way enact societal change. Whatever the topic may be, productive discussions are often _goal oriented_, so this will be a part of their digital versions on Pith.

## Introducing identity

We initially developed the Pith chat having deferred the topic of identity for later. Having done some testing, it's clear that we should not have done this—people were quick to point out the many issues with the anonymity on the platform—so our next phase will address this question.

Our proposed design for identity is to have both a global and local identity. Individuals will create an account to the platform to establish a _global_ identity. This will be used to keep track of the discussions they are participating in, their saved posts, and so on. However, within a discussion a different identity is used—the _local_ identity. Individuals create a nickname that they use to interact with others in the discussion that's somewhat independent of their global identity. Users in a discussion know which posts were created by the same individuals, but not who those individuals really are. We will be exploring the reasons for this choice alongside its benefits and drawbacks in a forthcoming blog post.

## Implementing summarization

There's much too much to discuss about this topic, so we'll be addressing it specifically in a future post. Phase II will introduce summarization to the core functionality.
