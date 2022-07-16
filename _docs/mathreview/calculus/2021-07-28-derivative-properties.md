---
layout: default
title: "Differentiation Rules"
parent: Calculus
grand_parent: "Math Review"
categories: calculus derivative
nav_order: 2
---

# Differentiation Rules

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Objectives
{: .no_toc}

> **The Basic Rules**
>
> - [x] List of basic rules
> - [ ] Examples
>
> **Chain Rule**
>
> - [ ] Definition
> - [ ] Applications
>
> **Higher deriviation**
>
> - [ ] Definition

{% katexmm %}

## Basic Rules

<dl>
  <dt>Constant law</dt>
  <dd>
    $$
    \left(cf(x)\right)^\prime=cf^\prime\left(x\right)
    $$
  </dd>
  <dd>
    $$
    \left(\lim_{x\to a}{cf(x)} = c\lim_{x\to a}{f(x)} \right)
    $$
  </dd>
  <dt>Sum/Diff law</dt>
  <dd>
    $$
    \left(f(x) \pm g(x)\right)^\prime=f^\prime\left(x\right)\pm g^\prime\left(x\right)
    $$
  </dd>
  <dd>
    $$
    \left(\lim_{x\to a}{\left[f(x)\pm g(x)\right]} = \lim_{x\to a}{f(x)}\pm\lim_{x\to a}{g(x)}\right)
    $$
  </dd>
  <dt>Power law</dt>
  <dd>
    $$
    \left(x^n\right)^\prime = nx^{n-1}
    $$
  </dd>
  <dd>
    $$
    \left(\lim_{x\to a}{\left[f(x)\right]^n} = \left[\lim_{x\to a}{f(x)}\right]^n\right)
    $$
  </dd>
  <dt>Product law</dt>
  <dd>
    $$
    \left(fg\right)^\prime=f^\prime g + g^\prime f
    $$
  </dd>
  <dd>
    $$
    \left(\lim_{x\to a}{\left[f(x)\cdot g(x)\right]} = \lim_{x\to a}{f(x)}\cdot\lim_{x\to a}{g(x)}\right)
    $$
  </dd>
  <dt>Quotient law</dt>
  <dd>
    $$
    \left(\frac{f}{g}\right) = \frac{f^\prime g - fg^\prime}{g^2}
    $$
  </dd>
  <dd>
    $$
    \left(\lim_{x\to a}{\left[\frac{f(x)}{g(x)}\right]} = \frac{\lim_{x\to a}{f(x)}}{\lim_{x\to a}{g(x)}}\right)
    $$
  </dd>
</dl>

## Chain Rule

Suppose there are two functions $f$ and $g$, both are differentiable:

1. If there is a function $h: h(x) = g(f(x))$, then $h$ is called a *composite* function
2. The composite function $h$ is denoted as: $$h=g\circ f \quad \text{or} \quad (g\circ f)(x) = g(f(x))$$
3. The derivative of the composite function: $$h^\prime(x) = g^\prime(f(x))f^\prime(x) \quad\text{or}\quad \frac{dh}{dx} = \frac{dh}{df}*\frac{df}{dx}$$

{% endkatexmm %}

## References

{% bibliography --file calculus --cited %}

[fig3_trig_function]: /assets/images/calculus/trig_functions.jpg "Trigometric functions"
[trig_review]: https://tutorial.math.lamar.edu/Classes/CalcI/TrigFcns.aspx
