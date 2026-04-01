<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 01 – Gravitational Dependence

## Problem Statement

A simple pendulum has a period of $4$ seconds on Earth. What would its period be on the Moon, where the gravitational acceleration is about $1/6$th of Earth's?

What is the required length of a simple pendulum to have a period of exactly $1$ second on Earth?

## Theory

The motion of a simple pendulum for small angles is described by simple harmonic motion. The period $T$ of a simple pendulum depends only on its length $L$ and the local acceleration due to gravity $g$. The relationship is given by

$$
T = 2\pi\sqrt{\frac{L}{g}}
$$

From this equation, we can observe two key proportionality relationships:
1. The period is directly proportional to the square root of the length: $T \propto \sqrt{L}$.
2. The period is inversely proportional to the square root of the gravitational acceleration: $T \propto \frac{1}{\sqrt{g}}$.

## Step-by-Step Solution

### Part 1: Period on the Moon

Given:
* Period on Earth ($T_E$) = $4 \text{ s}$
* Gravitational acceleration on Earth ($g_E$) $\approx 9.81 \text{ m/s}^2$
* Gravitational acceleration on Moon ($g_M$) = $\frac{1}{6}g_E$

We set up the ratio between the Moon and Earth:

$$
T_M = T_E \sqrt{\frac{g_E}{g_M}}
$$

Substituting $g_M = \frac{g_E}{6}$:

$$
T_M = 4 \sqrt{\frac{g_E}{g_E/6}}
$$

$$
T_M = 4\sqrt{6} \approx 9.80 \text{ s}
$$

### Part 2: Required Length on Earth

We rearrange the period formula to solve for $L$:

$$
L = \frac{g T^2}{4\pi^2}
$$

Given $T = 1 \text{ s}$ and $g = 9.81 \text{ m/s}^2$:

$$
L = \frac{9.81 \times (1)^2}{4\pi^2} \approx 0.248 \text{ m}
$$

## Final Result

* The period of the pendulum on the Moon is **$9.80 \text{ s}$**.
* The required length for a $1 \text{ s}$ period on Earth is **$0.248 \text{ m}$**.

## Interpretation

The increase in period on the Moon demonstrates that in a weaker gravitational field, the restoring force is smaller. Consequently, the bob accelerates more slowly, resulting in a "slower" swing.