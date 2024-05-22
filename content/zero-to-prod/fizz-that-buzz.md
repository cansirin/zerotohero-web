+++
title = "It's Time to Fizz that Buzz"
date = "2021-05-28"

[taxonomies]
tags = ["zero-to-prod"]
+++

![It's Time to Fizz that Buzz](/zerotohero-dev/content/images/size/w1200/2024/03/Volkan_zelik_data_structures_and_algorithms_but_they_are_alive_c53953fa-c2af-4acf-8494-e5d209cc1029.png)

Technical interviews in the valley require a weird mindset. (generated by
Midjourney)

Introduction
------------

In the video at the end of this post, I'm talking about **FizzBuzz Pro**---a
sister project of **Zero to Hero**.

In the video, I'm outlining a high-level architecture of the login flow of the
project, how it integrates with the **Ghost** content publishing platform as a
membership provider, and how I'm going to proceed.

**FizzBuzz Pro** is a greenfield project, and as I continue developing and
productizing it, I will be sharing the entire process with y'all with more
videos and articles.

> The video that I'm sharing here is a ~30min **uncut** recording: It's as raw
> as it gets.
>
> I wanted to share it in its entirety, before post-production, where I usually
> relentlessly cut out at least two-third of the video to increase the
> signal-to-noise ratio of it and provide as much value for the time you spend as
> I possibly can.

The High Level Overview
-----------------------

Here's the high-level authentication and identity management architecture that
I'll be talking about (_you can open the image in another tab for a
higher-resolution version_):

![](https://www.zerotohero.dev/content/images/2021/05/fizzbuzz-pro-verification-flow-2.png)

FizzBuzz Pro authentication high-level overview.

Video Discussion
----------------

So, without further ado, here goes the video.

Here's a quick cut where I'm talking about **FizzBuzz Pro** in general:

A brief overview of FizzBuzz Pro.

And here's the entire raw **uncut** video for your viewing pleasure:

On Keeping Things Simple
------------------------

After recording the video, I've realized that maybe coupling **Zero to Hero** (
_ghost_) user accounts with the **FizzBuzz Pro** user accounts is not the best
way to proceed.

The architecture I outlined above complicates things without providing any real
business value. It's better (_and simpler, and easier to maintain_) to keep *
*FizzBuzz Pro** as a separate service, and maybe provide a discounted enrollment
option (_using a zero-to-hero-generated discount coupon_) to **FizzBuzz Pro**
for the **Zero to Hero** premium members. To do that, we can create a separate
premium-member-only page where they can copy a discount coupon.

I'll update the diagram accordingly, create a follow-up articles, and also
create another video that walks through the new login flow.

And until then, enjoy... And may the source be with you 🦄.