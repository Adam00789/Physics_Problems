<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 09 – Vertical Throw with Drag

## Problem Statement

We have the equation of motion for a particle of mass $m$ thrown vertically:

$$
m\frac{dv}{dt} = -mg - kv
$$

with initial conditions $v(0)=v_0$ and $x(0)=10$.
* Solve the equation by analytical methods.
* Determine the maximum height.
* Compare with the case without drag.
* Perform a numerical simulation using Python.

## Theory

When an object moves through a fluid, it experiences a drag force $F_d = -kv$ (linear drag). This force always opposes the velocity. During the upward motion, both gravity and drag act downward. 

The terminal velocity $v_t$ is reached when the drag force equals the weight:

$$
mg = kv_t \implies v_t = \frac{mg}{k}
$$

## Step-by-Step Solution

### 1. Analytical Solution for Velocity

We rewrite the differential equation:

$$
\frac{dv}{dt} = -g - \frac{k}{m}v = -\frac{k}{m}\left( \frac{mg}{k} + v \right)
$$

Let $\gamma = \frac{k}{m}$ and $v_t = \frac{g}{\gamma}$. Then:

$$
\frac{dv}{v + v_t} = -\gamma dt
$$

Integrating both sides:

$$
\ln(v + v_t) = -\gamma t + C
$$

At $t=0$, $v=v_0$, so $C = \ln(v_0 + v_t)$.

$$
v(t) = (v_0 + v_t)e^{-\frac{k}{m}t} - v_t
$$

### 2. Maximum Height

Maximum height $H$ occurs when $v(t_{max}) = 0$.

$$
(v_0 + v_t)e^{-\gamma t_{max}} = v_t \implies t_{max} = \frac{1}{\gamma} \ln\left( 1 + \frac{v_0}{v_t} \right)
$$

Integrating $v(t)$ to find $x(t)$:

$$
x(t) = x_0 + \int_{0}^{t} \left[ (v_0 + v_t)e^{-\gamma \tau} - v_t \right] d\tau
$$

$$
x(t) = 10 + \frac{v_0 + v_t}{\gamma}(1 - e^{-\gamma t}) - v_t t
$$

Substitute $t_{max}$ to find $x_{max}$.

## Numerical Simulation (Python)

```python
import numpy as np

def simulate_throw(v0, m, k, g=9.81, dt=0.01):
    t, x, v = 0, 10, v0
    while v > 0:
        a = -g - (k/m)*v
        v += a * dt
        x += v * dt
        t += dt
    return x # Max height