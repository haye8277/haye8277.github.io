---
layout: post
title: "A Better Way to Run Store-Wide Sales"
date: 2026-05-18
---

Back in February I said I had some other things in the works. The first one is finally far enough along to talk about: a sale manager app.

## The problem

Most ecommerce platforms come with their own promotions built in: buy one get one free, spend a certain amount and save, that kind of thing. The catch is they all work at the cart level. The discount only shows up once something's been added to the cart, or once a customer meets some condition like buying a certain number of items.

What they don't handle well is a proper store-wide sale. Setting a specific discount across hundreds of products, having it show right on the product page where customers actually see it, and having it start and stop on a schedule. For a long time that meant a spreadsheet, a lot of clicking, and an alarm on my phone to switch everything back.

## What I built

So I built a tool to do it for me. I can set up a sale using:

- **A percentage off**, like 20% off everything in a collection
- **A set amount off**, like $10 off each product
- **A specific sale price** for each product

It all works in bulk, including straight from a CSV file, so a sale across hundreds of products is as easy as one. Every sale gets a start and end time, and the app takes care of applying it and putting prices back when it's over.

It's not flashy, but it has already saved me hours and removed a whole category of "did I remember to turn that off?" worries.

## Building it

I leaned heavily on modern development tools to build this. I like the practical side of new technology more than the hype, and this was a good example. Something that would have taken me months on my own came together in weeks, and I learned a lot along the way.
