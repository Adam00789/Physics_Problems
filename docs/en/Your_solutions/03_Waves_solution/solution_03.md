<h1 style="color:#4fc3f7">Task 03 – Superposition Principle</h1>

<h2 style="color:#81d4fa">Problem Statement</h2>

Two waves are described by:

$$
y_1(x, t) = A \sin(kx - \omega t)
$$

$$
y_2(x, t) = A \sin(kx + \omega t)
$$

Find the equation of the resulting standing wave and identify the positions of the nodes.

---

<h2 style="color:#81d4fa">Theory</h2>

The **superposition principle** states that the resultant displacement of a medium subject to two or more waves is the algebraic sum of the individual displacements:

$$
y(x, t) = y_1(x, t) + y_2(x, t)
$$

The two waves above have the same amplitude $A$, wave number $k$, and angular frequency $\omega$, but travel in opposite directions along the $x$-axis. Their superposition produces a **standing wave** — a pattern that oscillates in time but does not propagate in space.

The derivation uses the sum-to-product identity:

$$
\sin(\alpha) + \sin(\beta) = 2 \sin\!\left(\frac{\alpha+\beta}{2}\right) \cos\!\left(\frac{\alpha-\beta}{2}\right)
$$

---

<h2 style="color:#81d4fa">Step-by-Step Solution</h2>

<h3 style="color:#b3e5fc">Step 1 — Apply the Superposition Principle</h3>

$$
y(x,t) = A\sin(kx - \omega t) + A\sin(kx + \omega t)
$$

<h3 style="color:#b3e5fc">Step 2 — Apply the Sum-to-Product Identity</h3>

Set $\alpha = kx - \omega t$ and $\beta = kx + \omega t$:

$$
\begin{align}
\frac{\alpha + \beta}{2} &= \frac{(kx - \omega t) + (kx + \omega t)}{2} = kx \\
\frac{\alpha - \beta}{2} &= \frac{(kx - \omega t) - (kx + \omega t)}{2} = -\omega t
\end{align}
$$

Therefore:

$$
y(x,t) = 2A \sin(kx) \cos(-\omega t)
$$

Since $\cos(-\omega t) = \cos(\omega t)$:

$$
y(x, t) = 2A \sin(kx) \cos(\omega t)
$$

<h3 style="color:#b3e5fc">Step 3 — Identify the Nodes</h3>

Nodes are positions where the displacement is zero for all time. This requires:

$$
\sin(kx) = 0
$$

$$
kx = n\pi, \quad n = 0, \pm 1, \pm 2, \ldots
$$

Since $k = \dfrac{2\pi}{\lambda}$:

$$
\frac{2\pi}{\lambda} x = n\pi
$$

$$
x_n = \frac{n\lambda}{2}, \quad n = 0, \pm 1, \pm 2, \ldots
$$

---

<h2 style="color:#81d4fa">Final Result</h2>

**Standing wave equation:**

$$
y(x, t) = 2A \sin(kx) \cos(\omega t)
$$

**Node positions:**

$$
x_n = \frac{n\lambda}{2}, \quad n = 0, \pm 1, \pm 2, \ldots
$$

---

<h2 style="color:#81d4fa">Interpretation</h2>

The result $y(x,t) = 2A\sin(kx)\cos(\omega t)$ separates into a spatial factor $\sin(kx)$ and a temporal factor $\cos(\omega t)$. Every point on the string oscillates in phase (or exactly out of phase) with every other point, but with an amplitude that depends on position. Nodes — points of permanent zero displacement — are spaced $\lambda/2$ apart. Antinodes, where the amplitude is maximal ($2A$), occur midway between nodes at $x = (2n+1)\lambda/4$.