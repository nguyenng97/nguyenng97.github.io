---
layout: default
title: "Overview"
parent: "Calculus"
categories: calculus
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

## Concepts

> The branch of mathematics that deals with the finding and properties of derivatives
> and integrals of functions, by methods originally based on the summation of 
> infinitesimal differences.
>
> The two main types are differential calculus and integral calculus.
>
> —**Oxford Dict.**

### Limits

#### Definition

> Suppose $f(x)$ be a function defined on an interval that contains $x=a$:
> $$ \lim_{x\to a}{f(x)=L}$$
>
> (or $L$ is the limit of $f(x)$ as $x$ approaches $a$) iff
>
> $\exist \delta > 0 , \forall \varepsilon > 0 :$
> $$ \lvert f(x) - L\rvert < \varepsilon \quad where\quad 0 < \lvert x-a \rvert < \delta$$
>
> {%cite paulcalc --file calculus%}

***

To prove a limit of $f(x)$ at $x=a$ is $L$:

1. Verify if the limit of $f(x)$ at $x=a$ exists.
2. If `YES`:
   1. We need to prove: $$\forall \varepsilon > 0, \exists \delta > 0: \lvert f(x) - L\rvert < \varepsilon \quad where\quad 0 < \lvert x-a \rvert < \delta$$ One way to do this is to define a **process** to find a $\delta > 0$ for every $\varepsilon > 0$ that meets aforementioned requirement.
   2. With the **process** (i.e. $\delta=g(\varepsilon)$) found in <b>Step 2.1</b>, prove that: $$\lvert f(x) - L\rvert < \varepsilon \quad where\quad 0 < \lvert x-a \rvert < g(\varepsilon)$$
   3. Conclusion.
3. If `NO`:
   1. Conclusion (Limit DNE).

***

To reason how a limit of $f(x)$ does not exist, prove the negation of the [Limit's definition](#limits):
$$
\exists \varepsilon > 0, \forall \delta > 0: 0 < \lvert x-a\rvert < \delta \Rightarrow \lvert f(x) - L \rvert \geq \varepsilon
$$

***

**Example 1: Limit exists** Prove the following limit:

$$\lim_{x\to 2}{2x - 3} = 1$$

<details>
  <summary>Toggle solution</summary>
<br/>

Assume that the limit of $f(x) = 2x-3$ exists and $\forall \varepsilon > 0, \exist\delta > 0$:

$$
0 <\lvert x-2\rvert < \delta \implies \lvert f(x) - 1 \rvert < \varepsilon\qquad (*)
$$

From the *right* side of the inequation, we have:

$$
\begin{aligned}
 &\qquad& \lvert f(x)-1\rvert   &< \varepsilon\\
 \iff&&   \lvert (2x-3)-1\rvert  &< \varepsilon\\
 \iff&&   \lvert 2(x - 2)\rvert  &< \varepsilon\\
 \iff&&   \lvert x-2\rvert       &< \frac{\varepsilon}{2}\qquad (**)
\end{aligned}
$$

Also the *left* side of the inequation shows that:

$$
0 <\lvert x-2\rvert < \delta \qquad (***)
$$

In order for $(*)$ to be TRUE, the inequation below must be correct:

$$
0 <\lvert x-2\rvert < \delta\implies \lvert x-2\rvert <\frac{\varepsilon}{2}
$$

In other words, $0 < \lvert x-2\rvert < \delta \leq \frac{\varepsilon}{2}$. Choose $\delta = \frac{\varepsilon}{2}$, which is one of the solution of the inequation, as the $\delta$ solution for all $\varepsilon > 0$ of the inequation $(*)$.

<br/>

Finally, we must verify if the equation $(*)$ is correct for all $\varepsilon > 0$ with $\delta = \frac{\varepsilon}{2}$.

$$
\begin{aligned}
  \forall \varepsilon > 0,\delta = \frac{\varepsilon}{2} > 0, x\ne 2: &\quad& \\
      &\qquad&  &\quad& \lvert x-2 \rvert &< \frac{\varepsilon}{2} \\
  \iff&& 0  &< 2&\lvert x-2\rvert &< \frac{2\varepsilon}{2}\\
  \iff&& 0  &<  &\lvert 2(x - 3) - 1\rvert &< \varepsilon\\
  \iff&& 0  &<  &\lvert f(x)-1 \rvert &< \varepsilon
\end{aligned}
$$

</details>

![Figure 2](/assets/images/limits_files/limits_2_0.png)

*<b>Figure 1:</b> Prove $\lim_{x\to 2}{5x-4} = 6$ {%cite paulcalc --file calculus%}*

<details>
    <summary>Code for Fig. 1</summary>
    {% capture my_include %}{% include nb/limits.md %}{% endcapture %}
    {{ my_include | markdownify }}
</details>
***
> Intuitively, **Figure 1** of **Excercise 1**

### One-sided limits

<dl>
  <dt>Left-handed limit</dt>
  <dd>$\lim_{x\to a^-}{f(x)} = L$</dd>
  <dd>if $\forall \varepsilon > 0, \exist \delta > 0: \lvert f(x) - L\rvert <\varepsilon \quad where\quad 0 < x - a < \delta$</dd>
  <dt>Right-handed limit</dt>
  <dd>$\lim_{x\to a^+}{f(x)} = L$</dd>
  <dd>if $\forall \varepsilon > 0, \exist \delta > 0: \lvert f(x) - L\rvert <\varepsilon \quad where\quad 0 < a - x < \delta$</dd>
</dl>

### Limit laws

## Notation

{% endkatexmm %}

## References

{% bibliography --file calculus --cited %}