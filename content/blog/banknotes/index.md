---
title: Banknotes
date: "2025-09-16"
description: "What AI probably won't be able to generate"
---

A few weeks ago, Google gave us a new toy called Nano Banana (Gemini 2.5 Flash), which had significantly upgraded image generation capabilities compared to the previous 2.0 model. With the standards continuing to rise, text-to-image gets better and better. Things that models used to struggle with, like faces, [hands](https://www.reddit.com/r/StableDiffusion/comments/12c44g7/why_ai_art_struggles_with_hands/), and [historically accurate WWII German soldiers](https://www.nytimes.com/2024/02/22/technology/google-gemini-german-uniforms.html) are pretty much solved by now.

There are still plenty of tricky prompts that frontier models struggle with. But I think there is a specific kind of thing that will continue to be especially difficult for models to generate images of: **banknotes**. 

For example, here’s what some of today’s best image models think [Canadian banknotes](https://en.wikipedia.org/wiki/Banknotes_of_the_Canadian_dollar) look like:

<img width="1408" height="384" alt="banknotes" src="https://github.com/user-attachments/assets/32ca0453-9b5c-4e57-a367-5f0d614ba613" />

> Prompt: _“a top-down photo of a canadian currency collection containing one of each banknote denomination arranged on a solid white background. the banknotes are laid flat, neatly spaced, and each fully visible”_. **Left to right:** imagen-4.0, gpt-image-1, nano-banana, seedream-4

In this very limited experiment, all tested models except for gpt-image-1 failed to generate somewhat accurate looking Canadian banknotes. It worked a bit better with US banknotes, and there’s more clarity when prompted to generate a single banknote rather than a collection. But even when the banknote is overall correct, details are still blurry and text is often misspelled or scrambled. If time and usage limits allow, it would be interesting to try more currencies, especially less-traded ones.

Banknotes are purposely designed to be maximally difficult to copy. They have different materials, textures, and fine details which make them complicated and also give many ways to verify their authenticity. The combination of visual elements like face identities, tiny text, and intricate patterns also happen to perfectly strike at the weaknesses of today’s image models, which rely on aggressive compression techniques for learning.

So if you need a way to prove your photo or video isn’t AI, maybe try waving around some cash.
