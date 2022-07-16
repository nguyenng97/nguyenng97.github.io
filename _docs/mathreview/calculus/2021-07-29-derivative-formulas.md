---
layout: default
title: "Differentiation Formulas"
parent: Calculus
grand_parent: "Math Review"
categories: calculus derivative
nav_order: 3
---

# Differentiation Formulas

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

## Trig Functions

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

![trig_functions][fig1_trig_function]
{: .flex-justify-around .d-flex}
*<b>Figure 3:</b> Trigonometric functions {%cite wiki_trigo --file calculus%}*

|    | Function $f$ | Derivative $f^\prime$ |
|:--:|--------------|----------------|
|sin |$f(x) = sin(x)$|$f^\prime(x)=cos(x)$|
|cos |$f(x) = cos(x)$|$f^\prime(x)=-sin(x)$|
|tan |$f(x) = tan(x)$|$f^\prime(x)=\frac{1}{cos^2(x)}=sec^2(x)$|
|cot |$f(x) = cot(x)$|$f^\prime(x)=-\frac{1}{sin^2(x)}=-csc^2(x)$|

## Exponential functions

### Number e

WIP
{: .label .label-yellow}

The number $e$ is an important mathematical constant, approximately equal to $2.71828...$.

> Three general definitions of $e$ are:
>
> - $$e = \lim_{n\to \infin}{(1+\frac{1}{n})^n}$$
> - $$\lim_{h\to 0}{\frac{e^h-1}{h}} = 1$$
> - $$e = \sum_{n=0}^{\infin}{\frac{1}{n!}}$$

#### Eucler's Number: Intuitions
{: .no_toc}



<details>
    <summary>Code for Fig. 2</summary>
    {% capture my_include %}{% include nb/trig_functions.md %}{% endcapture %}
    {{ my_include | markdownify }}
</details>

![trig_functions][fig2_exp_function]
{: .flex-justify-around .d-flex}

<details>
    <summary>Code for Fig. 2</summary>
    {% capture my_include %}{% include nb/trig_functions.md %}{% endcapture %}
    {{ my_include | markdownify }}
</details>

$$
\begin{aligned}
&\frac{d}{dx}(e^x)=e^x & &\quad & &\frac{d}{dx}(a^x)=a^x \ln{a}\\
&\frac{d}{dx}(\ln{x}) = \frac{1}{x} & &\quad & &\frac{d}{dx}(\log_a{x})=\frac{1}{x\ln{a}}
\end{aligned}
$$

## Inverse of Trig functions

### Inverse Sine

$$
\begin{aligned}
y &= \sin^{-1}{x}\\
\frac{dy}{dx} &= \frac{1}{\sqrt{1-x^2}}
\end{aligned}
$$

<details>
    <summary>View proof</summary>
    {% capture my_include %}{% include proofs/inverse_sine.md %}{% endcapture %}
    {{ my_include | markdownify }}
</details>

### Summary: Inverse trig functions

$$
\begin{aligned}
\frac{d}{dx}\left(\sin^{-1}{x}\right) &= \frac{1}{\sqrt{1-x^2}}  &  \frac{d}{dx}\left(\cos^{1}{x}\right) &= -\frac{1}{\sqrt{1-x^2}}\\
\frac{d}{dx}\left(\tan^{-1}{x}\right) &= \frac{1}{1+x^2} & \frac{d}{dx}\left(\cot^{-1}{x}\right) &= -\frac{1}{1+x^2}\\
\frac{d}{dx}\left(\sec^{-1}{x}\right) &= \frac{1}{\lvert x\rvert \sqrt{x^2-1}} & \frac{d}{dx}\left(\csc^{-1}{x}\right) &= -\frac{1}{\lvert x\rvert\sqrt{x^2-1}}
\end{aligned}
$$

{% endkatexmm %}

## References

{% bibliography --file calculus --cited %}

[fig1_trig_function]: /assets/images/calculus/trig_functions.jpg "Trigometric functions"
[fig2_exp_function]: /assets/images/calculus/e_func.gif "Trigometric functions"
[trig_review]: https://tutorial.math.lamar.edu/Classes/CalcI/TrigFcns.aspx
