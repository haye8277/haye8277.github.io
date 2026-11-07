---
layout: post
title: "Getting Reviews Where They Belong"
date: 2026-11-07
---

This one started with a problem that had been bugging me for a while, and honestly, it came together a lot faster than I expected.

## The problem

When you run a few online stores selling a lot of the same products, the reviews end up scattered. Someone leaves a great review on one site, and shoppers on the others never see it. BigCommerce keeps each store's reviews to itself, so the only way to share them was copying them over by hand, one at a time. That gets old quickly.

## What I built

So I built a small app to do it for me. It runs on my own computer, matches up the same products across the stores, pulls every review into one place, and works out what each store is missing. Then it adds them, original dates and all.

## The tricky bits

It sounds simple, but a few parts turned out to be more interesting than I expected:

- **Spotting copies.** Some reviews had already been copied over by hand at some point, sometimes with small edits. The app needed to recognize those as the same review, so nothing got posted twice.
- **Sanitizing names.** Names get tidied up before they're shared, so it's a first name and last initial, and never an email address. Anything with an inappropriate reference, or that just doesn't read like a real name, gets held back so I can check it first, and each store can have its own rules for that.
- **Never doubling up.** If a store doesn't clearly confirm a review went through, the app checks before trying again instead of risking a duplicate. It also keeps track of everything it adds, so it can cleanly undo its own work.
- **Products listed differently.** Products aren't always set up the same way across platforms, and the same item can have a completely different product identifier in each store. So the app has to work out what's actually the same product before it shares anything, and in a few cases the reviews only flow one way.
