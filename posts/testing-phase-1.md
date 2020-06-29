---
title: "Feedback from Testing Phase I"
date: "2020-06-28"
author: "Sydney Zheng"
summary: "We tested the prototype website chat with a group of people informally. We gave them some time to chat among themselves and explore the features organically. People were able to pick up how to use multiple blocks in a post and tags fairly quickly."
---

We tested the prototype website chat with a group of people informally. We gave them some time to chat among themselves and explore the features organically. People were able to pick up how to use multiple blocks in a post and tags fairly quickly. About five minutes in, we began dropping hints of how to use other features—the search and transclusion ability. The conversation lasted for about twenty minutes. Afterward, we asked them for their formal feedback.

## Feedback

-   _Tags._ Tags were popular. People used it like a reply to a post, in addition to a place to "react" to post. Here's an example of someone trying to react with an emoji: ![](/images/emojis.png) A search via tags was also requested. Another issue revealed was that anyone can delete a tag. We should change this so only the creator of the tag can delete it.

-   _Replies._ People wanted the ability to reply directly to a post; without this functionality they used tags as a space for replies. Here's an example of a reply to a tag using transclusion: ![](/images/reply.png) Note that the original response to the post was placed in a tag, and then the author replied with a transclusion.

-   _Blocks._ People sometimes used multiple blocks in a post, especially to make lists.

-   _Identity._ We need some notion of identity within the chat as well as some notion of how many people are in the chat. This helps people feel like they are talking to each other in a more natural way.

-   _Search._ Our current method of search, by typing backspace followed by the query and then a space, was confusing to people. We should consider changing this. We might also add an FAQ to help people know basic features.

-   _Rich content._ People would like a spell checker, rich text editor, and the ability to send media or have special formats (like for code or Latex).

-   _Chat feed._ We should change the way people receive new posts. By default, people should automatically see new responses at the bottom of the chat screen. If they are higher up in the chat, viewing history per say, we can give them an arrow when new chats are created to let them "fly" to the bottom to view them. This is what Signal and Discord do.

-   _Accessibility._ We need to consider how to make the website accessible to more browsers, such as Edge. For now, our main focus was Firefox.

-   _UI._ We should include a dark mode in addition to updating the UI so that it uses our serif font.

-   _Resolution._ We should consider nesting text within a post, such as transclusions, and giving users the option to hide them.

## Next Steps

We will address these changes as well as some bugs that were pointed out. Soon after, we will develop Phase II—giving people the ability to summarize their conversation. More about this will be included in future updates.
