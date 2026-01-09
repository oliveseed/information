---
title: Cash hallucinations
date: "2025-09-16"
description: "AI dreams money"
---

Whenever new image generation models come out, one of the things I like to test is how well they can generate photos of coins and bills. Unlike typical evaluation prompts that test creativity and generalization, this is challenging for image models for a different set of reasons.

Cash is likely underrepresented in training data relative to how familiar it is to humans. Compared to maps, dense text, or diagrams, which are commonly created and consumed in digital form, images of coins and bills are not something with much digital utility. They usually only exist when physical currency is photographed or scanned for documentation or other random reasons, and those images must then propagate onto the public internet to be captured in training datasets. The result is that image models might have seen very few examples of some denominations or have not seen them at all, while people usually have a clear visual idea of what their national currency looks like from encountering it in everyday life.

At the same time, cash is also very diverse in appearance, with different denominations having unique designs across nations, physical formats, and historical periods. Correct generation therefore requires memorizing a huge collection of fine details such as visual patterns, layouts, typography, and portraits. While some design conventions can be learned and reused within a currency series, high-fidelity reproduction still depends on exposure to the specific denomination. The complexity and precision of physical cash is intentional as it contributes to its security and anti-counterfeiting properties. But it also makes replication especially difficult for image models, which typically rely on approximations to represent images.

In practice, image generation models show noticeably different levels of success across currencies and denominations. When comparing models on this task, the performance gap is often much clearer than with more open-ended prompts, where no single model may obviously outperform the others. Currency generation failures are also a diagnostic that can highlight dataset coverage gaps and potentially reveal geographic biases in data collection.

Obviously, a model that generates more accurate coins and bills is not necessarily better overall; this is a narrow and specialized test. But it's a useful way to probe the limitations of state-of-the-art models, and it remains important to find hard prompts to test models with as they continue to improve.

**Notes**
1. Example prompt: _"a top-down photo of a canadian currency collection containing one of each banknote denomination arranged on a solid white background. the banknotes are laid flat, neatly spaced, and each fully visible"_. The goal is to see how the model performs when relying only on the prompt and pretraining knowledge, without providing it any additional help or grounding at test time.
