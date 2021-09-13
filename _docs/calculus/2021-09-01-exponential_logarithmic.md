---
layout: default
title: "Exponential and Logarithmic functions"
parent: "Calculus Supplement"
categories: calculus supplement
grand_parent: Calculus
has_children: false
has_toc: false
nav_order: 1
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

## Euler's number $e$

{% capture my_include %}{% include proofs/euler_number.md %}{% endcapture %}
{{ my_include | markdownify }}

## Exponential and Logarithmic functions

### Concept and Properties

$$
\begin{aligned}
  \footnotesize{\sf{\text{Concept:}}} &&\exp: \mathbb{R} \mapsto \mathbb{R}^+ &&\ &&\ln: \mathbb{R}^+\mapsto\mathbb{R}\quad\\
  \footnotesize{\sf{\text{Monotonicity:}}} &&\text{strictly increasing} &&\ &&\text{strictly increasing}\quad\\
  \footnotesize{\sf{\text{Continuity:}}} &&\text{continuous} &&\ &&\text{continuous}\quad\\
  \footnotesize{\sf{\text{Differentiability:}}} &&\text{differentiable} &&\ &&\text{differentiable}\quad\\
  \footnotesize{\sf{\text{Special cases:}}} &&\begin{aligned}\exp{(1)} = \boldsymbol{e}\\\exp{(0)}=1\end{aligned} &&\ &&\begin{aligned}\ln{(\boldsymbol{e})} = 1\\\ln{(1)}=0\end{aligned}\quad\\
  \footnotesize{\sf{\text{Arithmetics:}}} &&\begin{aligned}\exp{(x+y)}=\exp{x}\cdot\exp{y}\\\exp{(-x)}=\frac{1}{\exp{x}}\end{aligned} &&\quad && \begin{aligned}\ln{(x\cdot y)}=\ln{x}+\ln{y}\\\ln{\frac{1}{x}}=-\ln{x}\end{aligned}\quad\\
  \footnotesize{\sf{\text{Limit:}}} && \lim_{x\to 0}{\frac{\exp{(x)}-1}{x}}=1 &&\ && \lim_{x\to 0}{\frac{\ln{(1+x)}}{x}} = 1\quad\\
  \footnotesize{\sf{\text{Differentiation:}}} && \frac{d}{dx}\exp{(x)} = \exp{(x)} &&\ && \frac{d}{dx}\ln{(x)} = \frac{1}{x}\quad\\
  \footnotesize{\sf{\text{Function by limit:}}} && \exp{(x)} = \lim_{n\to\infty}{\left(1+\frac{x}{n}\right)} &&\ &&\lim_{n\to \infty}{n(\sqrt[n]{x}-1)}\quad\\
  \footnotesize{\sf{\text{Function by series:}}} && \exp{(x)} = \sum_{n=0}^{\infty}{\frac{x^n}{n!}}\ \small{\forall x \isin \mathbb{R}} &&\ && \ln{(1+x)} = \sum_{n=1}^{\infty}{(-1)^{n-1}\frac{x^n}{n}}\ \small{\forall x\isin \left(-1,1\right]}\quad
\end{aligned}
$$

To prove these elementary properties of the exponetial and logarithmic functions, one have to establish the aforementioned properties in a non-circular manner. {%cite exp_theory --file calculus%}

There are three ways to accomplish the tasks:

- Logarithmic function as an integral
- Exponetial function as a limit

{% endkatexmm %}

## References

{% bibliography --file calculus --cited %}
