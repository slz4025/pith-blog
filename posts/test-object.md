---
title: "Designing a First Test Object"
date: "2020-06-07"
author: "Christian Broms & Sydney Zheng"
summary: "To begin to test out some of the features we've designed, we're creating a small protoype of the discussion interface. This test suite will serve as a way of evaluating the following design choices and features."
---

## Test Object

To begin to test out some of [the features we've designed](/posts/conversational-design), we're creating a small protoype of the discussion interface. This test suite will serve as a way of evaluating the following design choices and features:

### External Link Design

- Options
    - Citation could be included in a block's metadata. A property on the block.
    - Could be a higher-level organizer that links multiple blocks  (i.e. all these three blocks refer to the same source, so I include one link that's relevant to all three)
- Questions
    - How often do people use external citations?
    - When do people use external citations?
    - Are there cases when a citation seems warranted yet a person does not use one?  Should we encourage them to offer a citation?

### Internal Link Design

- Options
    - Have an icon next to each block that gives permalink.
    - Have an icon next to the head of each post that gives permalink.
    - Drag the block from the library to the post.
    - Search for the block within the post to add to the post.
- Questions
    - Will people actually find this feature useful in normal conversation?
    - How do people find and add a block to a post?
    - Are there cases when a citation seems warranted yet a person does not use one?  Should we encourage them to offer a citation?

### Saving Blocks/Posts

- Options
    - Have an icon next to each block that saves it to a library.
    - Have an icon next to the head of each post that saves it to a library.
    - The library of saved blocks/posts can be filtered by type (block/post) among other things like query.
- Questions
    - What kind of blocks will people save?
    - Will they use these blocks to refer to later on in the future?
    - Will they use these blocks to put them into summaries?

### Tagging a Contribution

- Options
    - Offer some pre-existing options: Action, Personal Story, Analysis.
    - Let people choose from tags made by other participants.
    - Maybe allow new tags to be generated based on which ones seem to be popular (future).
- Questions:
    - How often do people use pre-existing tags?
    - What kinds of options do people add?   Based on this, can evaluate set of pre-existing tags.
    - How will people actually end up using this feature?
    - How will they respond to the use of this feature?

## Take a Look

*Server-side*: [https://github.com/rainflame/pith-api](https://github.com/rainflame/pith-api)

*Front-end*: [https://github.com/rainflame/pith-frontend](https://github.com/rainflame/pith-frontend)