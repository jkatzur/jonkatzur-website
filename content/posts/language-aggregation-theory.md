---
title: "Are Typescript and Python the last languages?"
date: 2025-02-21T11:48:24-04:00
draft: false
---

I host this blog on AWS with S3 and cloudfront. It's built using [Hugo](https://gohugo.io/) a fun open-source static site generator. I picked this setup originally after reading reddit threads recommending various static site generators, like this [one](https://www.reddit.com/r/webdev/comments/1c8z739/what_is_your_favorite_static_site_generator/?rdt=63331). It was an excuse to learn some new tech, but I also wanted to pick something that was simple to learn and easy to deploy. 

For the past few months I've been using Cursor for my side projects. It completely changes the experience of writing code. Instead of the OODA loop of googling, reading docs, writing code, testing, reading reddit, checking stackoverflow, googling again, you ask an AI. You live in the IDE. And you notice that Cursor, using LLMs, is much better at writing code in popular languages and frameworks. I assume this is because the models are trained on open-source code and documentation, and the more that exists the better the LLMs are. 

While Hugo itself is much simpler framework than React, it has less documentation and fewer developers. When I hit a hugo bug in Cursor and work through the chat, it needs more help to find the answer, anad more trial and error than I want. I sometimes end up spending time in the same OODA loop even, gasp, googling!

Meanwhile, when coding more popular languages/frameworks Cursor gets it right more often by default and can fix bugs faster. 

This got me thinking about [aggregation theory](https://stratechery.com/aggregation-theory/) in the Ben Thompson strategy sense. In writing about internet companies his insight is that unlike tradition industries, companies that control demand (often time/attention), by creating better user experiences, end up controlling supply (content) and thus the value (eventually advertisers) enabling more investment in better user experiences.

Similarly, it seems that whichever languages have the most demand (developers using them) will end up controlling supply relevant to LLMs (code/docs), thus making developers more productive in these languages. This is a turning point where instead of new languages being created with improved syntax and features, we'll see existing languages and frameworks become more popular, ever easier to write in, with better abstractions as you actually converse with your AI to write the code. 

By the way, SQL will win because of this too, but it was too sad a realization to include in the title. 