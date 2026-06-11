---
title: "LTX 2.3 Rack Focus Test | ComfyUI Built-in Template [Prompt Included]"
source: "https://www.reddit.com/r/StableDiffusion/comments/1rqoweu/ltx_23_rack_focus_test_comfyui_builtin_template/"
author:
  - "[[umutgklp]]"
published: 2026-03-11
created: 2026-05-29
description: "Hey everyone. I just wrapped up some testing with the new LTX 2.3 using the built-in ComfyUI template. My main goal was to see how well the"
tags:
  - "clippings"
---
Hey everyone. I just wrapped up some testing with the new LTX 2.3 using the built-in ComfyUI template. My main goal was to see how well the model handles complex depth of field transitions specifically, whether it can hold structural integrity on high-detail subjects without melting.

**The Rig (For speed baseline):**

- **CPU:** AMD Ryzen 9 9950X
- **GPU:** NVIDIA GeForce RTX 4090 (24GB VRAM)
- **RAM:** 64GB DDR5

**Performance Data:** Target was a 1920x1088 (Yeah, LTX and its weird 8-pixel obsession), 7-second clip.

- **Cold Start (First run):** 413 seconds
- **Warm Start (Cached):** 289 seconds

Seeing that ~30% drop in generation time once the model weights actually settle into VRAM is great. The 4090 chews through it nicely, but LTX definitely still demands a lot of compute if you're pushing for high-res temporal consistency.

**The Prompt:**

> "A rack focus shot starting with a sharp, clear focus on the white and gold female android in the foreground, then slowly shifting the focus to the desert landscape and the large planet visible through the circular window in the background, making the android become blurred while the distant scenery becomes sharp."

**My Observations:** Honestly, the rack focus turned out surprisingly fluid. What stood out to me is how the mechanical details on the android’s ear and neck maintain their solid structure even as they get pushed into the bokeh zone. I didn't notice any of the usual temporal shimmering or pixel soup during the focal shift. Finally, no more melting ears when pulling focus.

**EDIT: Forgot to add the prompt....**

---

## Comments

> **skyrimer3d** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9tt0jc/) · 6 points
> 
> Now this is the kind of posts i love to see, i wish more people shared useful prompts like this with camera tricks and more.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9tt5ru/) · 3 points
> > 
> > I'm glad I could be of help.

> **Spara-Extreme** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9tuzse/) · 3 points
> 
> I’m realllly digging LTX2.3 right now.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9tvgh1/) · 1 points
> > 
> > Dig deeper bro! Good luck 🤘

> **luciferianism666** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9vlt94/) · 3 points
> 
> "rack" focus 👀
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9vlxpq/) · 1 points
> > 
> > 😂

> **Enshitification** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9tqmvc/) · 2 points
> 
> Nice, if it's controllable. The prompt section seems a bit empty though.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9tqv0p/) · 2 points
> > 
> > sorry I forgot to add the prompt....
> > 
> > **The Prompt:**
> > 
> > > "A rack focus shot starting with a sharp, clear focus on the white and gold female android in the foreground, then slowly shifting the focus to the desert landscape and the large planet visible through the circular window in the background, making the android become blurred while the distant scenery becomes sharp."
> > 
> > > **Enshitification** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9tr4xr/) · 2 points
> > > 
> > > Yes, that's better.
> > > 
> > > > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9tr7ib/) · 2 points
> > > > 
> > > > Thank you bro, now I understand why I got downvoted :)))

> **mugxyz** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9v4px0/) · 2 points
> 
> This is very nice. Fluid, smooth and artful. Great work.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9v5byz/) · 1 points
> > 
> > Thank you. Glad you liked it.

> **Pleasant\_Candy9103** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9v6ac9/) · 2 points
> 
> [u/umutgklp](https://www.reddit.com/user/umutgklp/) What exactly do you mean with "LTX 2.3 using the built-in ComfyUI template"? What advantage is there when you use in LTX2.3 the built in ComfyUI template? Can you elaborate on it? Do you use any additional Lora?
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9v8551/) · 1 points
> > 
> > I'm not sure if I have any advantage or not, I'm just using the comyui right out of the box. Mostly complex workflows give me headaches bunch of custom nodes and in the end I get muddy results. But the built-in templates give better results for me. I'm not using any additional Loras. When I find time I'll try and test Lord Kijai's version \[ [https://huggingface.co/Kijai/LTX2.3\_comfy](https://huggingface.co/Kijai/LTX2.3_comfy) \] .

> **roculus** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9vhzyf/) · 2 points
> 
> Did you edit out sound or was it completely silent? Nice to see the model didn't insert some random C3PO mechanical noises or voice.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9viuyt/) · 1 points
> > 
> > 😂😂😂 Sound was an annoying ambient drone music therefore I mute the sound.
> > 
> > > **roculus** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9vlk0d/) · 2 points
> > > 
> > > Doh! hehe. you could try starting prompt off with, "In a quiet room". That sometimes works :)
> > > 
> > > > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9vlsrx/) · 1 points
> > > > 
> > > > Interesting...ok I'll try next time...thanks for the tip...

> **Choice\_Sympathy9652** · [2026-03-12](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/oa3ch1i/) · 2 points
> 
> No matter how hard I try - characters from images always change to some muddy monsters, text generated characters are ugly from the beginning. I tried various LTX 2.3 models - normal, distilled - nothing seems to work. I thought I am not detailed enough with prompts - but here people use just short prompts and get great results. Can HW be blamed? 3090 24g, 64g system. But I dont believe 3090 calculates things differently than 4090 ...
> 
> > **umutgklp** · [2026-03-13](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/oa5y6mf/) · 1 points
> > 
> > True, when they start to talk they immediately turn into a crackhead 😂😂😂 I'm on the same boat too. Don't know but maybe Lord Kijai fixed this? Have you tried his workflows? About graphics cards calculating differently, well actually yes but no. I mean even with the same workflow and even with the same seed number we can get slightly different results but this doesn't mean that characters should turn into muddy crackheads. the others, as you can see, mostly generate cartoons and this doesn't force the model, trying with real human skins (+teeth+facial expressions) is an issue for this model. As my guess buying a 5090 would not change the results. I suggest you to experiment with the nodes' settings and seeds.

> **\[deleted\]** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9twc44/) · 4 points
> 
> I'm sure 2.5 will be better.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqoweu/comment/o9txoj5/) · 3 points
> > 
> > I'm sure 2.5 will be better.