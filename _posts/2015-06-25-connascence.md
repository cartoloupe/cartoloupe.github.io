---
layout: post
title: connascence
---

## what does this mean?:
> Connascence between two software components A and B means either 1) that you can postulate some change to A that would require B to be changed (or at least carefully checked) in order to preserve overall correctness, or 2) that you can postulate some change that would require both A and B to be changed together in order to preserve overall correctness.
  - `Meilir Page-Jones, What Every Programmer Should Know About Object-Oriented Design`

- it seems like connascence is a good thing from this definition...
- but:

> When one Ruby method has to know the correct order of another method’s positional arguments, we end up with connascence of position.

- ^ now it has a not so good connotation


### references
- [thoughtbot keyword arguments](https://robots.thoughtbot.com/ruby-2-keyword-arguments)

