---
layout: default
title: "Differentiation Formulas"
parent: Derivatives
grand_parent: Calculus
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

> **Differentiation Formulas**
>
> - [ ] Trig functions
> - [ ] Exponential functions
> - [ ] Logarithm functions
> - [ ] Hyperbolic functions

{% katexmm %}

## Differentiation Formulas

### Trig Functions

WIP
{: .label .label-yellow }

Below are popular six trig functions:

$$
\begin{aligned}
\cos{x}                           & \quad&&     \sin{x}& \\
\tan{x} &=\frac{\sin{x}}{\cos{x}}   \quad&&     \cot{x}&=\frac{\cos{x}}{\sin{x}} \\
\sec{x} &=\frac{1}{\cos{x}}         \quad&&     \csc{x}&=\frac{1}{\sin{x}}
\end{aligned}
$$

More reviews could be found [here][trig_review]

![trig_functions][fig3_trig_function]
{: .flex-justify-around .d-flex}
*<b>Figure 3:</b> Trigonometric functions {%cite wiki_trigo --file calculus%}*

|    | Function $f$ | Derivative $f^\prime$ |
|:--:|--------------|----------------|
|sin |$f(x) = sin(x)$|$f^\prime(x)=cos(x)$|
|cos |$f(x) = cos(x)$|$f^\prime(x)=-sin(x)$|
|tan |$f(x) = tan(x)$|$f^\prime(x)=\frac{1}{cos^2(x)}=sec^2(x)$|
|cot |$f(x) = cot(x)$|$f^\prime(x)=-\frac{1}{sin^2(x)}=-csc^2(x)$|

{% endkatexmm %}

### Exponential functions

WIP
{: .label .label-yellow}


## References

{% bibliography --file calculus --cited %}

[fig3_trig_function]: /assets/images/calculus/trig_functions.jpg "Trigometric functions"
[trig_review]: https://tutorial.math.lamar.edu/Classes/CalcI/TrigFcns.aspx
