---
layout: post
title: Neural Network #1 - Deep Neural Net.
edited: false
---

Due to ever-evolving of various data driven industries, tools and frameworks are adapting to become more and more powerful with more enjoyable learning curve for not only researchers and data scientist, but also engineers on some small-scale project. 

However, as the saying goes:

> The book is there for inspiration and as a foundation, the fundamentals on which to build. -Thomas Keller

Understanding basics of Neural Network would help to reduces hours in the future to crack your brain seeing some silly logical errors on screen, or a *Yike!* result at the end.

# Concept
## What is Neural Net?
Neural Network is well-known for classification problems such as Computer vision's Object Recognition or NLP's POS-tagging, etc.

All who spent a certain amount of time on this subject knew that despite the catchy name, "Neural Network" was only a loosely inspired version of human **Neural** system. But again, the name sure is sexy, so who cares?

Jokes aside, the idea behind the name is having a bunch of different functions chained together into a multiple layers structure. 

For example, suppose $f^{(1)}$ is the first layer, $f^{(2)}$ is the second, etc. By chaining these functions, $f(x) = f^{(2)}(f^{(1)}(x)$ - the output of this layer became input for the next.
<p align="center">
  <img src="https://i.ibb.co/DDnV50L/1200px-Colored-neural-network-svg.png" width="500">
</p>
The rest is not that different from other ML models, we got a function $y = f(x, \theta)$ (where **x** is an input vector and **y** is a category) with a bunch of parameters (the weights of the edges between every two nodes in two adjacent layers in the networks) $\theta$ to optimize based on the training set.

After the process, the initial ***f*** would, hopefully, approximate to ___f*___ - which is the true classification function for the problem.

With each training data point (a row of training data), the signal was fired through the network and the algorithm would magically do the optimization on $\theta$ - the weights (or the params). Then TADAA!! Problem solved after a few cups of coffee.

## What makes Neural Net better?



# References:
- [Neural Networks for beginners - Jay Shah](https://blog.statsbot.co/neural-networks-for-beginners-d99f2235efca)
- [Deep learning book - Ian Goodfellow et al.](http://www.deeplearningbook.org/)
