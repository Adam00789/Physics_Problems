# Task 06 – Variable Velocity

## Problem Statement

Given $v(t) = t^2 + 2t - 5$, with $x(0)=4$, find position and acceleration at $t=3$.

---

## Theory

Position:

$$
x(t) = \int v(t)\,dt
$$

Acceleration:

$$
a(t) = \frac{dv}{dt}
$$

---

## Step-by-Step Solution

Integrate:

$$
x(t) = \frac{t^3}{3} + t^2 - 5t + C
$$

At $t=0$, $x=4$:

$$
C = 4
$$

$$
x(3) = 9 + 9 - 15 + 4 = 7
$$

Acceleration:

$$
a(t) = 2t + 2
$$

$$
a(3) = 8
$$

---

## Final Result

$$
x(3) = 7, \quad a(3) = 8
$$

---

## Interpretation

Motion is non-uniform with increasing acceleration.