---
title: Understanding the formulae of network effects
slug: understanding-the-formulae-of-network-effects
date_published: 2019-09-09T00:00:00.000Z
date_updated: 2019-09-09T00:00:00.000Z
---

A16Z describes three different network effect formulae in their deck.
![](/assets/images/Understanding-the-formulae-of-network-effects/1-G_w-0hf2MoBL_KZGJ6FfUA.png)https://a16z.com/2016/03/07/all-about-network-effects/
Ever wondered how the formulae came to be without looking it up? It’s actually simple.

Well, the value formula is a way of quantitatively assessing how many connections can be formed within the network.

### In Yahoo

If there are n users, they all connect to Yahoo and have no connections to each other. So value is proportional to number of users. *V ∝ n*.

### In Facebook

Users are connected to each other. How many connections can you form between 2 users from a pool of n users?

> nC2 = n*(n-1)/2

So that’s like roughly saying *V ∝ n²*.

### In WhatsApp

Users can form many groups and share unique connections within the groups too.

How many groups can we form with n users?

> nC2 + nC3 + .. + … nCn

Guess what that equates to?

> = 2^n-nC1- nC0

We are subtracting *nC1 = n* because a group requires 2 people.

We are subtracting *nC0 = 1* is because groups cannot have 0 people.

But yeah, for brevity *V ∝ 2^n*.

### But why should value be measured in connections at all?

Because, as a company, you want to have as many ways to reach a particular user as possible to deliver your product.

### And the graph
![](/assets/images/Understanding-the-formulae-of-network-effects/1-geiBFImHupRt7x2KnJVYLQ.jpeg)https://redcatco.com/communication/metcalfes-law-really-useful-not/
