<h1 style="color:#4fc3f7">Task 08 – Travelling Wave Identification</h1>

<h2 style="color:#81d4fa">Problem Statement</h2>

Determine which of the following functions can describe a travelling wave by checking whether each satisfies the wave equation:

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}
$$

Candidates:

- a) $y(x,t) = A \cos(kx^2 - \omega t)$
- b) $y(x,t) = A(x - vt)^2$
- c) $y(x,t) = A \log(x + vt)$

---

<h2 style="color:#81d4fa">Theory</h2>

The **wave equation** is a second-order linear PDE. Any function $f(x,t)$ that can be written in the form $f(x \pm vt)$ satisfies the wave equation with speed $v$, provided $f$ is twice differentiable. Conversely, if the ratio $\partial^2 y / \partial x^2$ to $\partial^2 y / \partial t^2$ equals $1/v^2$ everywhere, the function is a valid travelling wave.

The approach is to compute both second derivatives and check whether their ratio is constant and equal to $1/v^2$.

---

<h2 style="color:#81d4fa">Step-by-Step Solution</h2>

<h3 style="color:#b3e5fc">a) $y = A\cos(kx^2 - \omega t)$</h3>

**First spatial derivative:**

$$
\frac{\partial y}{\partial x} = -A \sin(kx^2 - \omega t) \cdot 2kx
$$

**Second spatial derivative:**

$$
\frac{\partial^2 y}{\partial x^2} = -2Ak\sin(kx^2 - \omega t) - 4Ak^2 x^2 \cos(kx^2 - \omega t)
$$

**Second time derivative:**

$$
\frac{\partial^2 y}{\partial t^2} = -A\omega^2 \cos(kx^2 - \omega t)
$$

For the wave equation to hold, the ratio $\partial^2 y/\partial x^2$ to $\partial^2 y/\partial t^2$ must equal $1/v^2$ — a constant. The spatial second derivative contains both $\sin$ and $\cos$ terms while the time second derivative contains only $\cos$. There is no constant $v$ for which the equation is satisfied for all $x$ and $t$.

**Conclusion: does NOT satisfy the wave equation.**

---

<h3 style="color:#b3e5fc">b) $y = A(x - vt)^2$</h3>

This function has the form $f(x - vt)$ with $f(u) = Au^2$.

**Second spatial derivative:**

$$
\frac{\partial y}{\partial x} = 2A(x-vt), \qquad \frac{\partial^2 y}{\partial x^2} = 2A
$$

**Second time derivative:**

$$
\frac{\partial y}{\partial t} = -2Av(x-vt), \qquad \frac{\partial^2 y}{\partial t^2} = 2Av^2
$$

**Check:**

$$
\frac{\partial^2 y}{\partial x^2} = 2A, \qquad \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2} = \frac{2Av^2}{v^2} = 2A
$$

The wave equation is satisfied:

$$
2A = 2A \quad \checkmark
$$

**Conclusion: satisfies the wave equation with speed $v$.**

Note: While mathematically valid, this function is not periodic and represents a single broad pulse travelling in the $+x$ direction.

---

<h3 style="color:#b3e5fc">c) $y = A\log(x + vt)$</h3>

This function has the form $f(x + vt)$ with $f(u) = A\log(u)$.

**Second spatial derivative:**

$$
\frac{\partial y}{\partial x} = \frac{A}{x+vt}, \qquad \frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x+vt)^2}
$$

**Second time derivative:**

$$
\frac{\partial y}{\partial t} = \frac{Av}{x+vt}, \qquad \frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{(x+vt)^2}
$$

**Check:**

$$
\frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x+vt)^2}, \qquad \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{v^2(x+vt)^2} = -\frac{A}{(x+vt)^2}
$$

The wave equation is satisfied:

$$
-\frac{A}{(x+vt)^2} = -\frac{A}{(x+vt)^2} \quad \checkmark
$$

**Conclusion: satisfies the wave equation with speed $v$ (travelling in the $-x$ direction), valid for $x + vt > 0$.**

---

<h2 style="color:#81d4fa">Final Result</h2>

| Function | Satisfies Wave Equation? | Notes |
|---|---|---|
| $A\cos(kx^2 - \omega t)$ | No | Mixed $\sin/\cos$ terms; no constant $v$ exists |
| $A(x-vt)^2$ | Yes | Non-periodic pulse, travels in $+x$ direction |
| $A\log(x+vt)$ | Yes | Non-periodic, travels in $-x$ direction; requires $x+vt > 0$ |

---

<h2 style="color:#81d4fa">Interpretation</h2>

Any function of the form $f(x \pm vt)$ — provided it is twice differentiable — satisfies the wave equation. The argument $x - vt$ describes rightward travel; $x + vt$ describes leftward travel. The argument of function (a), $kx^2 - \omega t$, is not of this form (the $x^2$ term prevents it from being written as a function of $x \pm vt$), which is why it fails. Functions (b) and (c) are valid waves despite being non-sinusoidal and non-periodic.