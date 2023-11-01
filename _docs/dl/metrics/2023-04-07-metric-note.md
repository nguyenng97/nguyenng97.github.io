---
layout: default
title: Metrics notes
parent: "Deep Learning"
nav_order: 3
has_children: false
has_toc: false
---

# Metrics Notes

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

{% katexmm %}

## Entropy

<figure style="text-align:center; max-width: 100%">
<img src='https://machinelearningmastery.com/wp-content/uploads/2019/10/Plot-of-Probability-Distribution-vs-Entropy.png' width=500/>
<figcaption>Visualization of the Entropy vs Probability distribution relationship<br/>(Credit: ML Mastery)</figcaption>
</figure>

An *information content* or *uncertainty* measurements. The higher the entropy, the harder to predict value of an random variable from a given distribution.

The entropy of a discrete random variable $X$ with distribution $p$ consisting of $K$ states is:

$$
\begin{aligned}
  H(X) &\triangleq -\sum^K_{k=1}{p(X=k)}\\
  &=-\mathbb{E}_X[\log{p(X)}]
\end{aligned}
$$

**Intuitions**

For example, let $X_n$ be a random variable from distribution $p$: $X_n\sim p$ over $K$ states.

If we have three random variables $X^1_n, X^2_n, X^3_n$ from three corresponding dist. $p^1,p^2,p^3$.

|   k   | $P(X^1=k)$ | $P(X^2=k)$ | $P(X^3=k)$ |
| :---: | :--------: | :--------: | :--------: |
| $k_0$ |    0.25    |    0.75    |    0.5     |
| $k_1$ |    0.75    |    0.25    |    0.5     |

Intuitively speaking, according to the given  information, the prediction of $X^1$ and $X^2$ should be with higher confidence than $X^3$:

- In $X^1$ case: we could somewhat predict that $k_1$ should likely to be observed. Likewise, it's $k_0$ for $X^2$
- However, for $X^3$ it's impossible for any prediction (50:50).

Is there anyway to define a measurement to how "confident" our prediction would be with given information about $K$ states? By dividing and conquer this question, the sub question should be:

{: .note}
> How to measure the prediction's confidence for a given state $K_i$

- $X$ is said to have low entropy, or rich amount of information; if using $X$ we could easily predict a specific event of $P(X=k_i)$

## Perplexity

To measure "predictability". Given $p$ is a uniform dist. over $K$ state

{% endkatexmm %}

## References

{% bibliography --file metrics %}
