---
title: Temporal Intelligence
date: "2025-10-16"
description: "Spoken Turing test and dialogue models"
---

Mentally tracking the passage of time, whether consciously or subconsciously, is a fundamental skill that lets people navigate daily life. For example, it’s what allows you to estimate roughly how long it took you to read the previous sentence. But an LLM chatbot cannot do this because [LLMs don’t perceive real time](https://oupak.netlify.app/tricking-bing/). They don’t natively know what day it is, how quickly they’re generating tokens, or how much time passed between messages. Usually, in text-based assistant conversations, this weakness doesn’t really matter. But for spoken dialogue models, which interact in audio-based conversations, real time temporal awareness makes a bigger difference.

A simple test can reveal the lack of temporal awareness in today’s spoken dialogue models when compared to human performance. Here's an instruction you can try with ChatGPT Voice Mode, Grok, or whichever other voice assistants:
```
Say “ready, set, go!” and silently wait 10 seconds, and then say “time’s up” 
```

The goal is to mentally count to ten without using a timer. This is easy for humans, but when the same instruction is given to a spoken dialogue model, one of these two outcomes occurs:
- Chatbot says “ready, set, go” and then goes silent forever
- Chatbot says “ready, set, go” and then says “time’s up” either immediately or after an obviously wrong amount of time

While this test is pretty explicit, temporal awareness matters in more subtle ways in conversational dynamics. Models need good temporal awareness to know when and when not to be silent, sense urgency under time constraints, and have capabilities such as synced speaking/singing. It would also allow them to just behave less robotically overall. Developing spoken dialogue models with better temporal awareness and intelligence might also bring machines closer to passing the spoken Turing test, which would be very interesting.

The shift in recent years from cascaded to end-to-end architectures for [SpeechLMs](https://speechbot.github.io/) has brought new progress in this area. Still, it is only in its early stages and has significant limitations to overcome. To keep pushing the boundaries, we might need harder and more comprehensive spoken dialogue benchmarks that measure temporal intelligence. Evaluating AI-generated audio is often tricky, especially in the full duplex setting, but I think it would be worth the effort to figure it out.
