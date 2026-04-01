<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 10 – Force Field and Power

## Problem Statement

In a certain force field, the equations of motion of a particle with mass $m=0.5 \text{ kg}$ are:

$$
x = 5t^2 - t, \quad y = 2t^3, \quad z = -3t + 2
$$

Find the time dependence of: velocity, momentum, acceleration, force, and power.

## Theory

The kinematic variables are related by time derivatives of the position vector $\vec{r}(t)$:
* Velocity: $\vec{v} = \frac{d\vec{r}}{dt}$
* Acceleration: $\vec{a} = \frac{d\vec{v}}{dt}$
* Momentum: $\vec{p} = m\vec{v}$
* Force: $\vec{F} = m\vec{a}$
* Power: $P = \vec{F} \cdot \vec{v}$

## Step-by-Step Solution

### 1. Velocity ($\vec{v}$)

$$
v_x = \frac{d}{dt}(5t^2 - t) = 10t - 1
$$
$$
v_y = \frac{d}{dt}(2t^3) = 6t^2
$$
$$
v_z = \frac{d}{dt}(-3t + 2) = -3
$$
$$
\vec{v}(t) = (10t - 1, 6t^2, -3) \text{ m/s}
$$

### 2. Momentum ($\vec{p}$)

$$
\vec{p} = 0.5 \times (10t - 1, 6t^2, -3) = (5t - 0.5, 3t^2, -1.5) \text{ kg}\cdot\text{m/s}
$$

### 3. Acceleration ($\vec{a}$)

$$
\vec{a} = \frac{d\vec{v}}{dt} = (10, 12t, 0) \text{ m/s}^2
$$

### 4. Force ($\vec{F}$)

$$
\vec{F} = m\vec{a} = 0.5 \times (10, 12t, 0) = (5, 6t, 0) \text{ N}
$$

### 5. Power ($P$)

$$
P = \vec{F} \cdot \vec{v} = 5(10t - 1) + 6t(6t^2) + 0(-3)
$$
$$
P(t) = 36t^3 + 50t - 5 \text{ W}
$$

## Final Result

The time-dependent power is **$P(t) = 36t^3 + 50t - 5$ Watts**.

## Interpretation

The power is positive for $t > 0.1 \text{ s}$, meaning the field is doing work on the particle, increasing its kinetic energy.