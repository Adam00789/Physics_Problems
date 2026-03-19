# Task 02 – Range Optimization

## Problem Statement

Show analytically that the range

$$
R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}
$$

is maximized at a launch angle of $45^\circ$.

---

## Theory

To maximize a function, compute its derivative and find critical points where

$$
\frac{dR}{d\theta} = 0
$$

The sine function satisfies:

- Maximum value: $\sin(x) = 1$
- Occurs when $x = \frac{\pi}{2}$

---

## Step-by-Step Solution

Differentiate:

$$
R(\theta) = \frac{v_0^2}{g} \sin(2\theta)
$$

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta)
$$

Set derivative to zero:

$$
2\cos(2\theta) = 0
$$

$$
\cos(2\theta) = 0
$$

$$
2\theta = \frac{\pi}{2}
$$

$$
\theta = \frac{\pi}{4}
$$

---

## Final Result

$$
\theta = 45^\circ
$$

---

## Interpretation

Maximum range occurs when $\sin(2\theta)$ is maximized. This happens at $2\theta = 90^\circ$, giving $\theta = 45^\circ$.