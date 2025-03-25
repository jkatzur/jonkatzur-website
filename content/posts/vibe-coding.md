---
title: "So, I vibe coded"
date: 2025-03-24T11:48:24-04:00
draft: false
---

Continuing my exploration of llm assistance in coding, I decided to try to fully build an app end to end only via vibe-coding in natural language, no actual code. 

I did this mostly through the `composer` feature in cursor. I had a lot of fun! In particular, it collapsed the time I took from idea to working app from ~20 hours to ~2 hours. 

You can check out the app I built here: [Why are stocks up?](https://whyarestocksuptoday.com/) which is a question friends have asked me for years (don't worry, I also have whyarestocksdown.com). 

A few lessons in vibe-coding this:
* It's a lot more like management than coding. You need to communicate clearly, define requirements, and make decisions
* The LLMs understand examples quite well. I wanted my app to have the look/feel of fivethirtyeight and it understood how to replicate the style well
* The LLM does better when you clearly suggest it ask questions before writing code
* This is a fantastic way to... rack up a bunch of technical debt, but I also noticed the LLM is surprisingly good at refactoring, even large-scale refactors
* Every single software engineer should be using llms to write code like this. While it has some limitations and oddities in the way it writes code and potential technical debt, at minimum for prototyping and hacking it's remarkably fast
* This has to change how companies think about long-term software development systems. I expect companies that adopt high quality tooling, including re-usable components, will be able to combine AI with these lego blocks to move extremely quickly while maintaining code quality. 

More to digest over time. Beyond that, here was my opening prompt as an example of what I've seen work well:

```
I'd like to work together to define a feature for a project that I want to build. Let's work together to finalize and define the spec before we code it. The app will be called 'Market Pulse' or market-pulse. 

The app is going to be have three components:
1. A header in H1 that reads "Why are stocks up/down/flat today?" which will either say up, down, or flat depending on the actual stock market results of the day. 
2. A section in paragraph, ultimately written by an LLM that explains why the market is up/down/flat for the day. 
3. A set of three charts, one each for Nasdaq, SP500 and Dow that is a static chart that shows how stocks did that day. This should be a chart, show the % day change, and show todays level. 

Let's work together to finalize the requirements and then we can begin coding
```

We then went through functional and non-functional requirements, it asked questions to clarify, and eventually we jumped into coding. 