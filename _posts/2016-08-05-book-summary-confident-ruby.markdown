---
layout: post
title:  "Book Summary- Confident Ruby: 32 Patterns for Joyful Coding"
date:   2016-08-05 11:35:38
categories: books
---

## The problem the book adresses:
The book addresses the question on how to write methods in a way that they tell a story instead of looking like spaghetti.

## Methodology used to address the problem
THere are four parts to a method:
1. Collecting Input
2. Performing work
3. Delivering results
4. Handling failure

Usually when we think of a method we only think of "performing work" part. Breaking
the methods into the above mentioned parts when we think of them lets us do the following:
1. Separate the method logic from implementation details which will let us
write a method like it tells a story.
2. Reduces the burden of checking the inputs because we get to think in terms
of transforming the inputs to suit us better.
3. Focussing on delivering results in a more DRYer code. This will let you
create possibilities for batch processing :).

The book gives micro design patterns for collecting input, delivering results and handling
failures.

When you handle "peforming work" part of the method. There are a few things you should
keep in mind:
1. Operate at the same level of abstraction
2. Think in terms of roles and messages rather than in terms of objects and methods

**yet to be written: Details about the patterns**
