---
title: Cash hallucinations
date: "2025-09-16"
description: "AI struggles to remember what different currencies look like"
---

Whenever new image/video generation models come out, one of the things I like to test is whether they can accurately depict different kinds of coins and bills. Unlike typical evaluation prompts that test creativity and generalization, this is challenging for AI for different reasons.

The first challenge is that cash is likely underrepresented in training data to begin with. Compared to maps, dense text, or diagrams, which are commonly created and consumed in digital form, images and videos of coins and bills are not something with much digital utility. They usually only exist when physical currency is photographed or scanned for documentation or other random reasons, and that media must then propagate onto the public internet to be captured in training datasets. Naturally, image and video models might end up seeing zero or very few examples of some nations' currencies during training.

Even having seen it, it's hard to remember what it looks like. Cash is very diverse in appearance, with different denominations having unique designs across nations, physical formats, and historical periods. Correctly generating them therefore requires having memorized lots of fine visual patterns, typography, and portraits, and where they all belong. While some design conventions can be learned and reused within a currency series, there is minimal benefit to be gained from trying to generalize without actual exposure to each specific denomination. The high complexity and precision of physical cash is intentional as it contributes to its security and anti-counterfeiting properties, but it also happens to make replication especially difficult for AI models which typically rely on extreme compression to approximate visual information.

In practice, image and video models show noticeably different levels of success across currencies and denominations. When comparing models on this task, correctness is easy to evaluate compared to open-ended/creative prompts, where no single model may obviously outperform the others. Currency generation failures are also a diagnostic that can highlight dataset coverage gaps and potentially reveal geographic biases in data collection. Obviously, a model that generates more accurate coins and bills is not necessarily better overall; this is a narrow and specialized test. But it's a useful way to probe the limitations of state-of-the-art models, and it remains important to find hard prompts to test models with as they continue to improve.

**Notes**
1. Example prompt: _"a top-down photo of a canadian currency collection containing one of each banknote denomination arranged on a solid white background. the banknotes are laid flat, neatly spaced, and each fully visible"_. The goal is to see how the model performs when relying only on the prompt and pretraining knowledge, without providing it any additional help or grounding at test time.
