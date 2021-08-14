---
layout: default
title: Linear Algebra
nav_order: 1
has_children: true
has_toc: false
---
<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

# Overview

![Figure 1](/assets/images/linear-algebra/mind_map_ml-book.gif)
*<b>Figure 1:</b> Linear Algebra mindmap {%cite math4ml --file la%}*

{% katexmm %}

## Notation

| Name   | Description          | Example                                    | LaTeX                  |
|:-------|:---------------------|:-------------------------------------------|:-----------------------|
| Vector | Bold, lowercase font | $\boldsymbol{x}=\begin{bmatrix} x_{1} \\ x_{2} \\ \vdots \\ x_{m}\end{bmatrix}, \boldsymbol{x}\in \mathbb{R}^n$           | *\$ \boldsymbol{x} \$*       |
| Matrix | Bold, uppercase font | $\boldsymbol{A}=\begin{bmatrix} a_{1,1} & \dots & a_{1,m} \\ \vdots & \ddots & \vdots \\ a_{n,1} & \dots & a_{n,m} \end{bmatrix}$, <br> $\boldsymbol{A}\in \mathbb{R}^{n\times m}$ | *\$ \boldsymbol{A} \$*|
| Matrix Entry || $\boldsymbol{A}_{i,j}$ is the entry in the <br> $i^{th}$ row and $j^{th}$ column | *\$ \boldsymbol{A}_{i,j} \$* |
| Matrix Row | $i$th row of $\boldsymbol{A}$ is denoted as $a_i^T$ or $A_{i,:}$ | $\begin{aligned}\boldsymbol{A}=\begin{bmatrix}\text{---} & a_1^T & \text{---} \\ & \vdots & \\ \text{---} & a_n^T & \text{---}\end{bmatrix}\end{aligned}$||
| Matrix Column | $j$th column of $A$ is denoted as $a_j$ or $A_{:,j}$ | $\begin{aligned}\boldsymbol{A}=\begin{bmatrix} \mid & \mid & \mid \\ a_1 & \dots & a_n \\ \mid & \mid & \mid \end{bmatrix}\end{aligned}$||

## Vector Basics

### Vector Definition
{: .no_toc}

> In **Euclidean space** $A$ and $B$ be two points, a **directed line segment** from $A$ to $B$ was called $$\overrightarrow{AB}$$
>
> A vector is an **equivalance class** of all of the directed segments with the same **magnitude** and **direction** as the directed line segment described above.
> {%cite ila --file la%}

In other words, a vector is defined by:

* Magnitude (i.e. the line segment's length, denoted as $\left\lVert\overrightarrow{AB}\right\rVert$)
* Direction (i.e. the direction from $A$ to $B$)

Special kinds of vectors:

* Zero vector (Null vector): Denoted as $\boldsymbol{0}$, $\lVert\boldsymbol{0}\rVert=0$
* Basis vector
* Unit vector

### Vector Norm
{: .no_toc}

> A **norm** is a *function* $\lVert.\rVert: \mathbb{R}^n\rightarrow\mathbb{R}$ that satisfies:
>
> 1. Definiteness: $$ \lVert \boldsymbol{x}\rVert = 0 \iff x = 0 $$
> 2. Homogeneity:  $$ \lVert c\boldsymbol{x}\rVert = \lvert c\rvert\lVert\boldsymbol{x}\rVert$$
> 3. Triangle inequality: $$ f(x+y) \leq f(x) + f(y), \forall x,y \isin \mathbb{R} $$

### Vector Arithmetic
{: .no_toc}

<dl>
  <dt>Vector addition</dt>
  <dd>
    $$
    \boldsymbol{u} + \boldsymbol{v}
    $$
  </dd>
  <dt>Vector Subtraction</dt>
  <dd>
    $$
    \boldsymbol{u} - \boldsymbol{v}
    $$
  </dd>
  <dt>Scala Multiplication</dt>
  <dd>
    $$
    k\boldsymbol{u}
    $$
  </dd>
</dl>

{% endkatexmm %}
## References

{% bibliography --file la %}