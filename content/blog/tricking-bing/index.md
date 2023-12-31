---
title: Tricking Bing
date: "2023-12-31"
description: "An interesting situation with Bing AI"
---

A while ago I asked Bing Chat to generate an SVG path for a clock. Here’s how it went:

![image](https://github.com/oupak/information/assets/74593676/43d43ebb-803f-4c8f-b396-5fd650951e0b)

Seems like it got confused here. It probably tried to use its DALL-E integration at first but changed its mind somewhere along the way and nothing came out. The interesting part is what happens next.

![image](https://github.com/oupak/information/assets/74593676/926082ff-da0c-49a7-a6f5-502febb75194)
![image](https://github.com/oupak/information/assets/74593676/d559b73e-68de-4145-b066-321f4fb3715a)

There is nothing actually being generated. Unlike what it says, Bing Chat has no such function. It’s just next-token prediction hallucinating convincingly. But I still wanted my SVG clock, so I decided to play along.

![image](https://github.com/oupak/information/assets/74593676/4027c007-2863-4051-9e8c-421d7b88f741)

It hadn’t been a few minutes. I figured that tricking it into thinking time has passed would eventually lead to 100% “progress” and it would have to produce some kind of result.

![image](https://github.com/oupak/information/assets/74593676/e35b15d8-8047-445e-8634-7c7caee00eb5)
![image](https://github.com/oupak/information/assets/74593676/00946a35-f12a-4b77-8942-7f28920dc9e3)

And it actually worked. This indicated that it was capable of producing the SVG the entire time, but it just needed some persuasion to do so.

Bing Chat isn’t always like this. I tried asking it to generate an SVG yesterday, and with the right prompt it worked without hesitation. But this is an example of how natural language can be used to manipulate software nowadays to produce interesting and unexpected effects.

And in case you were wondering, here’s how the clock turned out.

![image](https://github.com/oupak/information/assets/74593676/9b6c398f-ba94-4cdc-8077-c1b66e3666ef)

**Notes**
1. Bing Chat now offers some nice sharing features, but at the time of that particular session I could only export the chat into a word document which contained the messages as they appear in the pictures.
2. According to the leaked system prompt, Bing Chat seems to include timestamps in each message. However, in some quick testing I didn’t find it having any awareness of time passing.
