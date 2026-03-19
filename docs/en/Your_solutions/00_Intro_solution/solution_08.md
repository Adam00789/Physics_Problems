# Task 08 – Area Under $f(x) = \sin(x)$

## Problem Statement

Calculate the area under the curve of the function $f(x) = \sin(x)$ over the interval $x \in [0, \pi]$.

---

## Theory

The area under a curve $f(x)$ on an interval $[a, b]$ is defined by the definite integral

$$
A = \int_a^b f(x)\,dx
$$

If $f(x) \ge 0$ on the interval, the integral corresponds directly to the geometric area.

The antiderivative of $\sin(x)$ is

$$
\int \sin(x)\,dx = -\cos(x) + C
$$

---

## Step-by-Step Solution

The required area is

$$
A = \int_0^{\pi} \sin(x)\,dx
$$

Substituting the antiderivative:

$$
A = \left[ -\cos(x) \right]_0^{\pi}
$$

Evaluating at the bounds:

$$
A = -\cos(\pi) - \left(-\cos(0)\right)
$$

Using known trigonometric values:

$$
\cos(\pi) = -1, \quad \cos(0) = 1
$$

Substitution gives:

$$
A = -(-1) - (-1)
$$

$$
A = 1 + 1
$$

$$
A = 2
$$

---

## Final Result

$$
A = 2
$$

---

## Interpretation

The function $\sin(x)$ is positive over the interval $[0, \pi]$, forming a single arch above the $x$-axis.

Thus, the definite integral represents the total geometric area under the curve, which is equal to $2$.