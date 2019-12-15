---
layout: post
title: Neural Network #1 - Deep Neuron Net.
---

Due to ever-evolving of various data driven industries, tools and frameworks are adapting to become more and more powerful with more enjoyable learning curve for not only researchers and data scientist, but also engineers on some small-scale project. 

However, as the saying goes:

> The book is there for inspiration and as a foundation, the fundamentals on which to build. 
> - Thomas Keller

Understanding basics of Neural Network would help to reduces hours in the future to crack your brain seeing some silly logical errors on screen, or a *Yike!* result at the end.

# Concept
All who spent a certain amount of time on this subject knew that despite the catchy name, "Neural Network" was only a loosely inspired version of human **Neural** system. 

Its main usage includes classification problems such as Computer vision's Object Recognition or NLP's POS-tagging. But again, the name sure is sexy, so who cares?

Jokes aside, the idea behind the name is having a bunch of different functions chained together into a multiple layers structure. 

For example, suppose $f^{(1)}$ is the first layer, $f^{(2)}$ is the second, etc. By chaining these functions, $f(x) = f^{(2)(f^{(1)}(x)}$
