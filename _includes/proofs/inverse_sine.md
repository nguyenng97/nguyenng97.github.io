{% katexmm %}

<b> Inverse of Sine Proof</b>

> Suppose that $$y=\sin^{-1}{x}$$
>
> We have:

$$
\begin{aligned}
    &&          f(f^-1(x)) &= x\\
    &\implies & f^\prime\left(f^{-1}(x)\right)\left(f^{-1}(x)\right)^\prime &= 1\\
    &\implies & \left(f^{-1}(x)\right)^\prime &= \frac{1}{f^\prime\left(f^{-1}(x)\right)}
    \end{aligned}
$$

> Let $f(x)=\sin{x}$ then:

$$
\left(\sin^{-1}{x}\right)^\prime = \frac{1}{\cos\left(\sin^{-1}{x}\right)}\quad (*)
$$

> Secondly, we also have

$$
\begin{aligned}
y = \sin^{-1}(x) &\implies \sin{y} &&= x , \quad \frac{-\pi}{2} \leq y \leq \frac{\pi}{2}\\
                 &\implies \cos{y} &&= \sqrt{1-x^2}\\
                 &\iff     \cos{\left(\sin^{-1}(x)\right)} &&= \sqrt{1-x^2}\quad (**)
\end{aligned}
$$

> From $(*),(**)$ we could conclude that:

$$
\left(\sin^{-1}{x}\right)^\prime = \frac{1}{\sqrt{1-x^2}}
$$

{% endkatexmm %}
