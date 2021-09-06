---
layout: default
title: "Calculus Supplement"
parent: "Calculus"
categories: calculus derivative
has_children: false
has_toc: false
nav_order: 3
---
<details open markdown="block">
  <summary> 
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

{% katexmm %}

## Objectives
{: .no_toc}

> **Exponential and Logarithmic Functions**
>
> - [ ] Definition
> - [ ] Properties

## Preprequisites

### Exponentiation operation

**Exponentiation**, involving two components: the **base** ($b$) and the **power** ($n$) defined as
$$
b^n = \underbrace{b\times \dots \times b}_{n\ \text{times}}
$$

Properties of the exponentiation consists of:

- $a^{p+q} = a^p \cdot a^q$
- $(a\cdot b)^q = a^q \cdot b^q$
- $\left(\frac{a}{b}\right)^q = \frac{a^q}{b^q}$
- $\left(a^p\right)^q = a^{pq}$

Suppose $n \isin \mathbb{Q}$, the concept of exponentiation and its properties could also be expanded to $n \isin \mathbb{R}$ by using the limit theory.

### Power function

$$
  f(x) = cx^n
$$

| Relation | Name | Shape |
|----------|------|:-----:|
| $x\mapsto x$ | Identity, Linear | <img src='/assets/images/calculus/linear_func.png' width=150 height=150> |
| $x\mapsto x^2$ | Quadratic |  <img src='/assets/images/calculus/parabolic_func.png' width=150 height=150> |
| $x\mapsto x^{\frac{1}{2}}$ | Square root | <img src='/assets/images/calculus/square_root_func.png' width=150 height=150>|
| $x\mapsto x^{-1}$ | Reciprocal | <img src='/assets/images/calculus/hyperbolic_func.png' width=150 height=150>|

## Logarithmic function

To define a logarithmic function and prove its properties, the **Euler number** $e$ have to be defined and be used to establish the function's properties in a non-circular manner. {%cite exp_theory --file calculus%}

{% capture my_include %}{% include proofs/euler_number.md %}{% endcapture %}
{{ my_include | markdownify }}

{% endkatexmm %}

## References

{% bibliography --file calculus --cited %}
