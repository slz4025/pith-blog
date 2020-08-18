---
title: "Clarifying Pith's Purpose"
date: "2020-08-09"
author: "Sydney Zheng"
summary: "We decided that Pith should be designed to solve the (more) specific problem of allowing large discussions to take place such that (1) every person's perspective is represented and (2) the discussion can eventually be condensed into a one-page summary that can then be used to review the main points or to make decisions."
---

We decided that Pith should be designed to solve the (more) specific problem of allowing large discussions to take place such that (1) every person's perspective is represented and (2) the discussion can eventually be condensed into a "one-page summary" that can then be used to review the main points or to make decisions. 

We want to design the basic framework for this purpose that can then be applied in numerous settings, such as for corporate, for open-source problem-solving, for more casual exploration of other people's experiences.

## Representing Perspectives

There are two key ideas to do this. 

1. How can we identify under-examined perspectives?
2. How can we help bridge perspectives that have not been in contact, especially if each perspective has something important to contribute to the other?

## Summarizing a Large Discussion

A summary makes a discussion more digestible to everyone. If a community agrees a decision should be made off a summary, then it should be clear to everyone through what justification people make their decisions.

The summary can better represent the distribution of perspectives because of the prior point.

## Design

We are experimenting with several ideas for achieving these main two objectives.

Here we explain the general architecture of the design so far.

- Just as before, we have small discussions with at most ten people.
- Each discussion can make a summary for the purpose of keeping of record of the discussion itself. The summary is composed of summary-blocks, which are transcluded from the discussion and edited in the summary if need be.
- The discussion members are encouraged to "summarize" the salient points of their discussion to the general community. They do this by creating a select few "super-blocks", each of which should represent a discrete idea.
- The super-blocks are semantically organized in a network with super-blocks from other discussions. Therefore, we see the semantic landscape of salient points throughout discussions. The exact method for how super-blocks are placed in semantic space is yet to be determined.
- Super-blocks are linked to the discussion summary, which is linked to all super blocks from the discussion. Sections of the summary can be treated as an extension of super-blocks. For example, a super-block can express something such as "whales are great", and the summary can argue why.
- In the network, super-blocks are connected if they came from the same discussion.
- Therefore, there are two types of bonds: a semantic one and a co-mentioned one.
- The platform automatically detects certain patterns, like which semantic spaces (topics) have not been co-mentioned much with which other topics, or not co-mentioned with other topics in general and are relatively isolated.
- Humans exploring the network, and with the help of the automated patterns, identify which topics are underrepresented or could be bridged with another topic.
- Topics that are underrepresented or can be bridged can be "pinned" on the board and prioritized as a starting point for the spawning of new discussions. The board can ultimately allow people to "meta-discuss" what needs attention,.
- When these new discussions are formed, they create a new kind of link that shows they are inspired or transcluded from the topics.
- Within a discussion, people can explore the network and use it to inspire their current discussion. If they want to reference particular super-blocks, that is also a transclusion.

Note there are several keys issues that need to be solved.

## Issues

- How are super-blocks semantically organized together?
- How are "topics" identified, if they should be identified in a coherent way?
- How can we help people search the network without getting overwhelmed?
    - If a discussion's creation was inspired from several super-blocks, it is likely helpful that people should explore super-blocks that are semantically similar to those inspirational super-blocks. If people transclude super-blocks during the conversation, these super-blocks are also gateways to more semantically super-blocks.
    - It may also be helpful if people explore the co-mention links from these super-blocks, to see in which context particular super-blocks could have come up in.
    - If people have general topics they want to explore, perhaps a keyword or traditional semantic search of the blocks can help them find a starting point in the network to search around.
- When people search the network, how is it visually presented?
    - Is it a list, like how a search engine could present results?
    - Is it a network, which may emphasis the links or the topology of the space more than the nodes (results)?