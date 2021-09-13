{% katexmm %}

By concept, the number $e$ or **Euler's number**, is a mathematical **constant** which is an [irrational number][wiki-euler] of

$$
e = 2.71828182845904523536028747135266249775724709369995\dots
$$

There are multiple approaches existed to explain the origin of this "unique" constant (just like how $\pi$ is the ratio between circumference and diameter of any circle). However, this note will limit the scope to two explanations (or characterization) of this special constant:

- $e$ as a **base rate** of **exponential growth** {%cite bex_e --file calculus%}
- **Area under the curve** of $\frac{1}{x}$ between $x=1$ and $x=e$ **is 1**.

### Rate of exponential growth

Suppose there is an exponential function

$$
f(x) = a^x, x\isin \mathbb{R}
$$

**The first look** into this function's instant rate of change is:

$$
\begin{aligned}
\frac{df}{dx} &= \lim_{\Delta{x}\to 0}{\frac{a^{x+\Delta{x}}-a^x}{\Delta{x}}}\\
              &= a^x\left(\lim_{t\to 0}{\frac{a^t-1}{t}}\right)\\
              &= a^x\left(f^\prime(0)\right) & (1)
\end{aligned}
$$

By observation, the instant change ratio of $f(x)$ at $x=x_0$ is a product of the $f(x_0)$ and **a constant** of $\lim_{t\to 0}{\frac{a^t-1}{t}}$ or $f^\prime(0)$

| Base ($a$) | $\lim_{t\to 0}{\frac{a^t-1}{t}}$ |
|------|-------------|
|2|0.69314720407|
|3|1.09861234998|
|4|1.38629445701|
|6|1.79176007364|
|$e$|1|

Due to the unique property of $e$ of having
$$
\begin{aligned}
\lim_{t\to 0}{\frac{e^t-1}{t}} &= \frac{d}{dx}\left(e^x\right)\big|_{x=0}\\
                               &= e^0 \\
                               &= 1 && (2)
\end{aligned}
$$

[This fact could be proved in a non-circular manner][paramanands-proof].

The property also makes the computation of derivative of $f(x) = a^x$ easier by just transforming every power function $a^t$ to $e^{t\ln{a}}$ and let $h = t\ln{a}$:

$$
\begin{aligned}
\lim_{t\to 0}{\frac{a^t-1}{t}} &= \ln{a}\cdot \lim_{t\ln{a}\to 0}{\left(\frac{e^{t\ln{a}}-1}{t\ln{a}}\right)}\\
                               &= \ln{a}\cdot \underbrace{\lim_{h\to 0}{\left(\frac{e^h-1}{h}\right)}}_{\text{Result =}1}\\[1.5em]
                               &= \ln{a} & (3)
\end{aligned}
$$

Thanks to $e$ and its special character at $(2)$, the expression $(1)$ could be computed
for all base of $a\isin\mathbb{R}$ by converting $b$ to a power function of base $e$

$$
a = \exp{(\ln{a})}
$$

---

**The second** picture on exponential growth: **Compound Growth**

Suppose the intial value is $V$ and the growth rate per period is $R$

| Period | Value Before | Value After |
|--------|--------------|-------------|
|1| $V$ | $V+VR = V(1+R)$|
|2| $V(1+R)$|$V(1+R) + R\cdot V(1+R) = V(1+R)^2$|
|...| | |
|n| $V(1+R)^{n-1}$ | $V(1+R)^n$|

Every period, the growth amount will grows at the same rate to contribute to the initial
value, hence the term **Compound growth**.

$$
\begin{aligned}
&& V_n &= V_0\cdot (1+R)^n & (1)\\
&\text{or} & V_n &= V_0\cdot (1 + \text{rate})^{\text{period}}
\end{aligned}
$$

In the right side of the equation $(1)$, suppose $R = \frac{1}{n}$ and $V_0 = 1$, then we have a special
expression of:

$$
f(n) = \left(1+\frac{1}{n}\right)^n
$$

$$
\rule{20em}{0.3pt}
$$

> Investigating the behavior of $f(n)$ expose a few interesting insights:
>
> 1. The higher $n$, the higher $f(n)$
> 2. $f(n)$ seems to approach a certain limit with larger $n$

$$
\rule{20em}{0.3pt}
$$

**Point #2** and the value of the limit mentioned a fact of:

$$
\lim_{n\to \infty}{\left(1+\frac{1}{n}\right)^n} = c \quad\quad c \text{ is a constant}
$$

**Hint**: $c = e$

**Solution**:

$$
\begin{aligned}
&&\ln{\left[\lim_{n\to\infty}{\left(1 + \frac{1}{n}\right)^n}\right]} &= n\cdot\lim_{n\to\infty}{\left[\ln{\left(1+\frac{1}{n}\right)}\right]}\\
&&&=\underbrace{\lim_{\frac{1}{n}\to 0}{\left[\frac{\ln{\left(1 + \frac{1}{n}\right)}}{\frac{1}{n}}\right]}}_{\text{Result = }\ 1}\\
&\iff & \lim_{n\to \infty}{\left(1+\frac{1}{n}\right)^n} = e
\end{aligned}
$$

### Area under the curve of $y = \frac{1}{x}$

![euler_number_proof](/assets/images/calculus/euler_number_2_0.png)
{: .flex-justify-around .d-flex}
*<b>Figure 1:</b> Area under the curve of $\frac{1}{x}$ {%cite exp_theory --file calculus%}*

### Applications
WIP
{: .label .label-yellow}

#### Compound interest

#### Bernoulli trials

#### Standard normal distribution

[wiki-euler]: https://en.wikipedia.org/wiki/E_(mathematical_constant)
[paramanands-proof]: https://paramanands.blogspot.com/2014/05/theories-of-exponential-and-logarithmic-functions-part-1.html#.YTrHC50zZPb

{% endkatexmm %}
