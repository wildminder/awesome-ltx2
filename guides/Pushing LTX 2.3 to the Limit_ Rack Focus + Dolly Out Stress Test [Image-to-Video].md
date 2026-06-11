---
title: "Pushing LTX 2.3 to the Limit: Rack Focus + Dolly Out Stress Test [Image-to-Video]"
source: "https://www.reddit.com/r/StableDiffusion/comments/1rqtz0f/pushing_ltx_23_to_the_limit_rack_focus_dolly_out/"
author:
  - "[[umutgklp]]"
published: 2026-03-11
created: 2026-05-29
description: "Hey everyone. Following up on my previous tests, I decided to throw a much harder curveball at LTX 2.3 using the built-in Image-to-Video wor"
tags:
  - "clippings"
---
Hey everyone. Following up on my previous tests, I decided to throw a much harder curveball at LTX 2.3 using the built-in Image-to-Video workflow in ComfyUI. The goal here wasn't to get a perfect, pristine output, but rather to see exactly where the model's structural integrity starts to break down under complex movement and focal shifts.

**The Rig (For speed baseline):**

- CPU: AMD Ryzen 9 9950X
- GPU: NVIDIA GeForce RTX 4090 (24GB VRAM)
- RAM: 64GB DDR5

**Performance Data:** Target was a standard 1920x1080, 7-second clip.

- Cold Start (First run): 412 seconds
- Warm Start (Cached): 284 seconds

Seeing that ~30% improvement on the second pass is consistent and welcome. The 4090 handles the heavy lifting, but temporal coherence at this resolution is still a massive compute sink.

**The Prompt:**

> "A cinematic slow Dolly Out shot using a vintage Cooke Anamorphic lens. Starts with a medium close-up of a highly detailed cyborg woman, her torso anchored in the center of the frame. She slowly extends her flawless, precise mechanical hands directly toward the camera. As the camera physically pulls back, a rapid and seamless rack focus shifts the focal plane from her face to her glossy synthetic fingers in the extreme foreground. Her face and the background instantly dissolve into heavy oval anamorphic bokeh. Soft daylight creates sharp specular highlights on her glossy ceramic-like surfaces, maintaining rigid, solid mechanical structural integrity throughout the movement."

**The Result:** While the initial image was sharp, the video generation quickly fell apart. First off, it completely ignored my 'cinematic slow Dolly Out' prompt—there was zero physical camera pullback, just the arms extending. But the real dealbreaker was the structural collapse. As those mechanical hands pushed into the extreme foreground, that rigid ceramic geometry just melted back into the familiar pixel soup. Oh, and the Cooke lens anamorphic bokeh I asked for? Completely lost in translation, it just gave me standard digital circular blur.

LTX 2.3 is great for static or subtle movements (like my previous test), but when you combine forward motion with extreme depth-of-field changes, the temporal coherence shatters. Has anyone managed to keep intricate mechanical details solid during extreme foreground movement in LTX 2.3? Would love to hear your approaches.

---

## Comments

> **skyrimer3d** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9vd5ke/) · 4 points
> 
> Really, really impressive, i never thought this camera shifts were possible with a local video model, great find.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9vdq8h/) · 2 points
> > 
> > Thank you bro. I'll try more camera movements and share with you all. The results are not always satisfying but at least it's free to retry again and again :))

> **fauni-7** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9us5qg/) · 6 points
> 
> Would.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9usawi/) · 2 points
> > 
> > [
> > 
> > ](https://external-preview.redd.it/sR8wmwydcu3Ivy4inLctZ0BARU98Ttba-0EDxqXujWw.gif?auto=webp&s=c1e607cb026a0af76ff2e6801a26f1dc4af8eda6)

> **berlinbaer** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9vzz2f/) · 2 points
> 
> they do have those specialized camera controls loras, no idea if you've tried them.
> 
> overall i am also a bit annoyed at how sometimes instructions will get totally ignored in regards to framing. always wonder if there is some magic word or combo that we are all just missing. maybe it's not trained on "dolly out" but "pull out" instead or something who knows.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9w31mp/) · 1 points
> > 
> > You are right not all of them work properly. I'm trying so many variations in my end and I'm willing to share decent results with you all. And I hope others share too.

> **\[deleted\]** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9w1u53/) · 2 points
> 
> Save it dude. Thanks
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9w3dnf/) · 1 points
> > 
> > You're welcome bro. I'm glad to be of help.

> **jefharris** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9we13o/) · 2 points
> 
> Tagged with Workflow included?
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9wf0y2/) · 2 points
> > 
> > Ohh sorry never thought I should also add the comfyui built-in template here too. Please read the post.
> > 
> > > **jefharris** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9y2lup/) · 2 points
> > > 
> > > Thanks!
> > > 
> > > > **umutgklp** · [2026-03-12](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9z1tjj/) · 1 points
> > > > 
> > > > You're welcome bro, glad to be of help.

> **Cubey42** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9wfbhl/) · 2 points
> 
> I think pushing ltx2 i2v would be getting good dynamic motion with a complex narrative imo
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9wpu8c/) · 1 points
> > 
> > Like what? Can you share your experience with us?

> **Odd-Scarl-7308** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9xbz1h/) · 2 points
> 
> How much electricity did that clip cost
> 
> > **umutgklp** · [2026-03-12](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9z0r0b/) · 1 points
> > 
> > Never tried to calculate that but not much. I'll share if I calculate.

> **ih8ithear** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9y22o5/) · 2 points
> 
> That is so sick! Any advice how to achieve something like this?
> 
> > **umutgklp** · [2026-03-12](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9z1gkt/) · 2 points
> > 
> > Thank you, glad you liked it. Actually I shared all the details..... This may sound cliche:)) Use detailed images and focus on the prompt.

> **James\_Reeb** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9uxxej/) · 1 points
> 
> Great ! Workflow pleaz 😽
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9v07i0/) · 2 points
> > 
> > Thank you bro. I've used the LTX 2.3 built-in Image-to-Video workflow in ComfyUI. If you can't see it try to update your ComfyUI to the latest.

> **\[deleted\]** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9v9i0x/) · 1 points
> 
> i would love a workflow if possible? im trying to gather what everyone has done and ship my caption tool with it  
> people dont realise sometimes the 7 second clip tht took 412 seconds actually takes 9 hours of testing different things lol
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9vabc4/) · 1 points
> > 
> > You are absolutely right bro, before that 412 seconds yes hours of testing, especially engineering the prompt is not an easy task. For the workflow; I'm using the latest ComyUI's built-in template and didn't change any nodes, I just added the prompt and I shared the prompt exactly as it is.
> > 
> > > **Phuckers6** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9vnqgm/) · 4 points
> > > 
> > > Could speed things up by adding an image preview node after the first low resolution part of the workflow. Then, if the preview images look off, you can just cancel the generation and update the prompt.
> > > 
> > > > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9w1g8e/) · 1 points
> > > > 
> > > > You are right but in my results the problem mostly occurs in the end of the video.
> > > > 
> > > > > **Phuckers6** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9wptgr/) · 2 points
> > > > > 
> > > > > The way the image preview works, it outputs all the frames as images. You can click on an image and then use arrow keys to scroll through them to see the full animation.
> > > > > 
> > > > > What you would be previewing is the whole video at lower resolution. What's added later in the upscale stage is the fine details. So you can at least check that the overall animation came out right.
> > > > > 
> > > > > > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9wq6hb/) · 2 points
> > > > > > 
> > > > > > I should try this. Thank you for the tip.
> > > > > > 
> > > > > > > **Phuckers6** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9wr2s6/) · 2 points
> > > > > > > 
> > > > > > > It's especially useful if you're doing longer clips. Would be better to find out about any issues early on. And the second high resolution stage should be the slower part anyway, because, well... it's generating at double the resolution.

> **Aware-Swordfish-9055** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9w7wkk/) · 1 points
> 
> Clickbait, that no rack focus.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9wahpv/) · 1 points
> > 
> > 😂🤣 no rack no focus 🤣😂🤣😂

> **\[deleted\]** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9utnwk/) · 7 points
> 
>  Target was a standard 1920x1080, 7-second clip. Hope you manage to get the result you want.
> 
> > **umutgklp** · [2026-03-11](https://reddit.com/r/StableDiffusion/comments/1rqtz0f/comment/o9uul17/) · 2 points
> > 
> >  Target was a standard 1920x1080, 7-second clip. Hope you manage to get the result you want.