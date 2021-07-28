---
layout: default
title: "Derivative"
parent: "Calculus"
categories: calculus derivative
nav_order: 2
---
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

> **1. Derivative**
>
> - [ ] Definition
> - [ ] Interpretation
>
> **2. Derivative Formulas**
>
> - [ ] Trig functions
> - [ ] Exponential and Logarithm functions
> - [ ] Hyperbolic functions
>
> **3. Laws of Derivation**
>
> - [ ] Deriviation laws
> - [ ] Chain rule

{% katexmm %}

## Derivative

> The **derivative** of $f(x)$ with respect to x is the function $f^\prime(x)$:
>
> $$ f^\prime(x) = \lim_{h\to 0}{\frac{f(x+h) - f(x)}{h}} $$
> $$ (f^\prime \text{called 'f prime of x'}) $$

There are 2 major interpretations for a derivative of a function:

- Rate of change
- Slope of tangent line

***

![line_kinds](/assets/images/calculus/secant.png)
*<b>Figure 1:</b> Common lines and line segments on a circle {%cite wiki_sec --file calculus%}*

To understand a tangent line, the secant line concept has to come first.

***

> A secant is a line that intersects a curve at a minimum of two distinct points.
>
> {%cite wiki_sec --file calculus%}

***

If we draw a secant line at $\left(a, f(a)\right)$, the slope of this line is:
$$m_{sec} = Q = \frac{f(x) - f(a)}{x - a}$$

This equation forms a *difference quotient*. Suppose $\forall h\ne 0: x = a + h$, the aforementioned equation can also be expressed as:
$$Q = \frac{f(a + h) - f(a)}{h}$$

***

> A tangent line is a line that intersects a curve at two infinitely close points
>
> ― **Gottfried Wilhelm Leibniz**

***

According to the above properties, one could infer the slope $m_{tangent}$ of the tangent line of $f(x)$ at $x=a$ is:

$$
\begin{aligned}
m_{tangent} = f^\prime(a) &= \lim_{x\to a}{\frac{f(x) - f(a)}{x - a}} \\
&= \lim_{\Delta{x}\to 0}{\frac{\Delta{f(x)}}{\Delta{x}}}
\end{aligned}
$$

***

To summary,

$$
\begin{aligned}
\text{Secant line} &= \frac{\Delta{f(x)}}{\Delta{x}} & &= \text{Average rate of change} \\
\text{Tangent line} &= \lim_{\Delta{x}\to 0}{\frac{\Delta{f(x)}}{\Delta{x}}} & &= \text{Instantaneous rate of change}
\end{aligned}
$$

{% endkatexmm %}

## References

{% bibliography --file calculus --cited %}
