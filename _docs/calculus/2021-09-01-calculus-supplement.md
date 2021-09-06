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

## Exponential and Logarithmic functions

### Concept and Properties

$$
\begin{aligned}
  \footnotesize{\sf{\text{Concept:}}} &&\exp: \mathbb{R} \mapsto \mathbb{R}^+ &&\quad &&\ln: \mathbb{R}^+\mapsto\mathbb{R}\\
  \footnotesize{\sf{\text{Monotonicity:}}} &&\text{strictly increasing} &&\quad &&\text{strictly increasing}\\
  \footnotesize{\sf{\text{Continuity:}}} &&\text{continuous} &&\quad &&\text{continuous}\\
  \footnotesize{\sf{\text{Differentiability:}}} &&\text{differentiable} &&\quad &&\text{differentiable}\\
  \footnotesize{\sf{\text{Special cases:}}} &&\begin{aligned}\exp{(1)} = \boldsymbol{e}\\\exp{(0)}=1\end{aligned} &&\quad &&\begin{aligned}\ln{(\boldsymbol{e})} = 1\\\ln{(1)}=0\end{aligned}\\
  \footnotesize{\sf{\text{Arithmetics:}}} &&\begin{aligned}\exp{(x+y)}=\exp{x}\cdot\exp{y}\\\exp{(-x)}=\frac{1}{\exp{x}}\end{aligned} &&\quad && \begin{aligned}\ln{(x\cdot y)}=\ln{x}+\ln{y}\\\ln{\frac{1}{x}}=-\ln{x}\end{aligned}\\
  \footnotesize{\sf{\text{Limit:}}} && \lim_{x\to 0}{\frac{\exp{(x)}-1}{x}}=1 &&\quad && \lim_{x\to 0}{\frac{\ln{(1+x)}}{x}} = 1\\
  \footnotesize{\sf{\text{Differentiation:}}} && \frac{d}{dx}\exp{(x)} = \exp{(x)} &&\quad && \frac{d}{dx}\ln{(x)} = \frac{1}{x}\\
  \footnotesize{\sf{\text{Function by limit:}}} && \exp{(x)} = \lim_{n\to\infty}{\left(1+\frac{x}{n}\right)} &&\quad &&\lim_{n\to \infty}{n(\sqrt[n]{x}-1)}\\
  \footnotesize{\sf{\text{Function by series:}}} && \exp{(x)} = \sum_{n=0}^{\infty}{\frac{x^n}{n!}}\ \small{\forall x \isin \mathbb{R}} &&\quad && \ln{(1+x)} = \sum_{n=1}^{\infty}{(-1)^{n-1}\frac{x^n}{n}}\ \small{\forall x\isin \left(-1,1\right]}
\end{aligned}
$$

To define a logarithmic function and prove its properties, the **Euler number** $e$ have to be defined and be used to establish the function's properties in a non-circular manner. {%cite exp_theory --file calculus%}

{% capture my_include %}{% include proofs/euler_number.md %}{% endcapture %}
{{ my_include | markdownify }}

{% endkatexmm %}

## References

{% bibliography --file calculus --cited %}
