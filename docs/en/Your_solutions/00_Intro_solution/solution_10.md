# Task 10 – Infinite Series and Final Position of an Ant

## Problem Statement

An ant starts at the origin and moves in the following pattern:

- $1$ m east  
- $\frac{1}{2}$ m north  
- $\frac{1}{3}$ m west  
- $\frac{1}{4}$ m south  
- $\frac{1}{5}$ m east  
- ...

Determine the final position of the ant.

---

## Theory

The motion can be decomposed into horizontal and vertical components.

- East-West motion contributes to the $x$-coordinate.
- North-South motion contributes to the $y$-coordinate.

The movements alternate directions and form two separate infinite series:

- Horizontal displacement: alternating series
- Vertical displacement: alternating series

A key known result is the alternating harmonic series:

$$
\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n} = \ln(2)
$$

---

## Step-by-Step Solution

### Horizontal Displacement

The horizontal movements are:

- $+\frac{1}{1}$ (east)
- $-\frac{1}{3}$ (west)
- $+\frac{1}{5}$ (east)
- $-\frac{1}{7}$ (west)
- ...

This forms the series:

$$
x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots
$$

This is a known series:

$$
\sum_{k=0}^{\infty} \frac{(-1)^k}{2k+1} = \frac{\pi}{4}
$$

Thus,

$$
x = \frac{\pi}{4}
$$

---

### Vertical Displacement

The vertical movements are:

- $+\frac{1}{2}$ (north)
- $-\frac{1}{4}$ (south)
- $+\frac{1}{6}$ (north)
- $-\frac{1}{8}$ (south)
- ...

This gives:

$$
y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \cdots
$$

Factor out $\frac{1}{2}$:

$$
y = \frac{1}{2} \left(1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots \right)
$$

Recognize the alternating harmonic series:

$$
\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n} = \ln(2)
$$

Thus,

$$
y = \frac{1}{2} \ln(2)
$$

---

## Final Result

The final position of the ant is:

$$
\left( \frac{\pi}{4}, \frac{1}{2} \ln(2) \right)
$$

---

## Interpretation

The motion consists of infinitely many steps with decreasing magnitude. Although the total distance traveled diverges, the position converges due to alternating directions.

- The horizontal motion converges to $\frac{\pi}{4}$.
- The vertical motion converges to $\frac{1}{2}\ln(2)$.

Thus, the ant approaches a fixed point in the plane.