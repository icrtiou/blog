---
title: Free my annotation
description: A way to annotate web page and get the data out.
author: "Lucas Shen"
image: assets/2020-03-21-free-my-annotation/cover.png
comments: true
toc: true
layout: post
categories: [w3c, linked-data, web-annotation, knowledge-graph]
---

## Context

Recently, I've been reading ferociously like this

![](https://media.giphy.com/media/4K55PfPOhIrIY/giphy.gif)

I enter this state every once in a while to upgrade myself. However, **this time is different**. I am constantly overloading my mental pipeline which does ETL[^1] to convert info into knowledge for me.

Heuristically, I categorize info into **3 buckets** to decide if some materials need further processing.

1. **Ideas I knew by heart**.
   - It may be presented differently but I got it. Good to reinforce what I knew.
2. **Ideas help construct new connection of existing knowledge**.
   - It's a trigger to help realizing the possibility to connect existing dots differently. Sense of enlightenment, but nothing radical.
3. **Ideas introduce whole new perspective**.
   - Like cartesian coordinates to polar coordinates. Not only see things differently, existing internal knowledge structure is transforming along with it. The effect has two fold:
     - fast: Immediate brain dead. I'll just freeze for a while. No repulsive rejection. I knew I hit something big, positive, but can't react.
     - slow: The beauty is here. My brain's physical structure is literally changing. It will take a while for new perspective to break, reorg and merge with whatever I have in my brain. This is gold[^2], and where annotations come to play an important role.

![](/assets/2020-03-21-free-my-annotation/iq.png)

My recent reads mostly land in category 3, hence the kernel panic. Could be the world is changing exponentially but I'm not. Regardless the reason, I have to seize the opportunity to internalize as much as possible so that new ideas won't be just words I read before, but concrete framework in my brain helping me making better decision in the future.

## Purpose of annotation

I can brute force through materials in category 1 and 2. For cat 1, could just forget it. Cat 2, write it down few times, compose a quick learning note or write a prototype program to connect dots should be enough. Cat 3 is in whole new level. Opportunity like this need cares. I need to create an environment to nurture new perspectives.

In this book, [How to read a book](https://www.amazon.com/How-Read-Book-Classic-Intelligent/dp/0671212095), it introduces the idea of highest level of reading: **syntopical reading**[^9]. Basically compare and contrast a set of ideas to understand the shape and interconnection of them, which forms the conceptual framework of the subject.

In order to compare and contrast the elements and relationships of new perspective, I need a group of people analyzing, discussing, question and answering and find references over a period of time, typical research process. However, it's hard to find a group of people to tackle something of my interest at the right space time. So usually I have to simulate a group of imaginary personas working on the same problem with me.

Simulation is important because I need various attack angles to dissect the subject. Idealist, pragmatist, technologist, politician and businessman will see things differently. By resolving initially convoluted logical relationships and finding the right incentive to unite different personas, I have a chance to get the complete picture of new perspective. For me, a new perspective is how things could work differently. Burn chaotic init states through clash of personas is my process of making sense of complexities.

Back to annotation. It serves two purposes to facilitate the process:

1. Keep records of interaction.
2. Provide decent data representation to facilitate further interaction and final interpretation.

There will be a period of time I need to stay as close as possible to original reading materials to comment, highlight and take notes, repeatedly[^10]. To track how my understandings evolve over time and cultivate each persona's unique voice, I need to comment on my comments and notes too. A tool helps me talking to myself. Decent UI/UX to make sense of all annotations as a whole over a period of time. I call this kind of annotation **evergreen notes**[^3]

Tools I knew could achieve these goals but couldn't stop wondering if there's better process.

## Insufficient toolbox

I have been using PDF reader, MS Word, MS OneNote, MindMap and [draw.io](draw.io) to track my continuous conversation with materials. It's ok. Few problems though:

- They are designed to be used by human only. Each one of them have proprietary data format. In this setting, machines can't help a lot in the process. I need to do all the works to copy, combine and transform[^4] materials.
- Data are siloed. Not trivial to extract annotations in Word doc and combine with those in PDF and EPUB.

Having been working on data projects for few years, I grow appreciation on the synergy of machine and human to generate useful insight from digital footprints. Even though ultimately it's human's responsibility to interpret and understand, machine definitely can do more to help during the process. The power of google search[^5] is not human curation, but to leverage the inherent interconnections of HTML via hyperlinks.

Then, I found this: [Hypothes.is](https://web.hypothes.is/).

> a non-profit using w3c standards to annotate the web with anyone, anywhere.

## [Hypothes.is](https://web.hypothes.is/)

I was exporting web page as PDF to annotate. With hypothes.is, I could easily annotate web page directly. Few other great features:

- Non-profit using open web standards[^6].
  - I'm not another product served to advertisers directly.
  - Able to use that open web standard to interpret data.
- API. Even has a WebSocket based realtime API[^7] 👍
- Able to create private group.
- Support PDF and EPUB.
- Open source. 🤩

With this, I don't need to export PDF anymore. Just annotate web page, save URL and revisit. Option to see public annotations and maybe join the conversation.

Reddit, Facebook, HackerNews and countless forums can all facilitate open conversations. But fine grained annotation directly on web page to everyone is way more powerful in my opinion.

What really excites me is that, with this tool and open web standards, I could build a personal knowledge graph[^8] programatically.

## Potential

Imagine a world:

- I could have comprehensive view of all readings. Flashcards are generated automatically to easily review key quote and comment.
- Follow the breadcrumbs of HTMLs to expand the width or depth of the research.
- Relationships of materials.
  - The graph could be serialize on time dimension to see how I'm influenced by what, when, and laid out briefings of each article.
  - Able to explore the interconnections of materials and track the progress of exploration into unknown area.
  - Could even use ML generated summary to help me decide which direction is more interesting to dig deeper.

I won't dream too far to say this could be the foundation of personal Jarvis but this is way better than siloed PDF and Word files scatter all over my PC.

![](https://media.giphy.com/media/K0gPNKBiSYjG8/giphy.gif)

Will definitely use the service for a little longer and see if I could build something useful. Annotation on voice and video sounds useful to me, considering all those podcasts and youtube videos.

---

[^1]: [Extract, transform, load](https://en.wikipedia.org/wiki/Extract,_transform,_load)
[^2]: [Perspective is gold](https://youtu.be/1e8VZlPBx_0?t=94)
[^3]: [Evergreen notes are written and organized to evolve, contribute, and accumulate over time, across projects..](https://notes.andymatuschak.org/My_morning_writing_practice?stackedNotes=Evergreen_notes)
[^4]: [Everything is a Remix](https://vimeo.com/139094998)
[^5]: [Pagerank](https://en.wikipedia.org/wiki/PageRank)
[^6]: [Web Annotation Data Model](https://www.w3.org/TR/annotation-model/)
[^7]: [Real Time API](https://h.readthedocs.io/en/latest/api/realtime/)
[^8]: [Knowledge Graphs](https://arxiv.org/abs/2003.02320)
[^9]: [How to Read a Book: The Ultimate Guide by Mortimer Adler](https://fs.blog/how-to-read-a-book/)
[^10]: [Spaced Repetition for Efficient Learning](https://www.gwern.net/Spaced-repetition)
