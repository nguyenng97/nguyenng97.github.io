---
layout: default
title: "Overview"
parent: "Linear Algebra"
categories: linear_algebra
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

## Notation

| Name   | Description          | Example                                    | LaTeX                  |
|:-------|:---------------------|:-------------------------------------------|:-----------------------|
| Vector | Bold, lowercase font | $\boldsymbol{x}=\begin{bmatrix} x_{1} \\ x_{2} \\ \vdots \\ x_{m}\end{bmatrix}, \boldsymbol{x}\in \mathbb{R}^n$           | *\$ \boldsymbol{x} \$*       |
| Matrix | Bold, uppercase font | $\boldsymbol{A}=\begin{bmatrix} x_{1,1} & \dots & x_{1,m} \\ \vdots & \ddots & \vdots \\ x_{n,1} & \dots & x_{n,m} \end{bmatrix}$, <br> $\boldsymbol{A}\in \mathbb{R}^{n\times m}$ | *\$ \boldsymbol{A} \$*|
| Matrix Entry || $\boldsymbol{A}_{i,j}$ is the entry in the <br> $i^{th}$ row and $j^{th}$ column | *\$ \boldsymbol{A}_{i,j} \$* |

## Concepts

![Figure 1](/assets/images/linear-algebra/mind_map_ml-book.gif)
*<b>Figure 1:</b> Linear Algebra mindmap {%cite math4ml --file la%}*

### Vector

### Matrix

$$
\begin{aligned}
y &=  \begin{bmatrix}
        x_{1} \\
        x_{2} \\
        \vdots \\
        x_{m}
      \end{bmatrix}
      \begin{bmatrix}
        x_{1} \\
        x_{2} \\
        \vdots \\
        x_{m}
      \end{bmatrix}
\end{aligned}
$$

{% endkatexmm %}

## References

{% bibliography --file la --cited %}
