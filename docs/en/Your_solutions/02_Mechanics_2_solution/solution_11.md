<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 11 – Dynamics with a Time-Dependent Force

## Problem Statement

A particle of mass $m=3 \text{ kg}$ moves in a force field $\vec{F} = (15t, 3t-12, -6t^2) \text{ N}$.
Initial conditions: $\vec{r}_0 = (5, 2, -3) \text{ m}$, $\vec{v}_0 = (2, 0, 1) \text{ m/s}$. Find position and velocity.

## Step-by-Step Solution

### 1. Acceleration

$$
\vec{a}(t) = \frac{\vec{F}}{m} = (5t, t-4, -2t^2)
$$

### 2. Velocity

$$
\vec{v}(t) = \vec{v}_0 + \int_{0}^{t} \vec{a}(\tau) d\tau
$$

$$
v_x = 2 + \int 5t dt = 2.5t^2 + 2
$$
$$
v_y = 0 + \int (t-4) dt = 0.5t^2 - 4t
$$
$$
v_z = 1 + \int -2t^2 dt = -\frac{2}{3}t^3 + 1
$$

### 3. Position

$$
\vec{r}(t) = \vec{r}_0 + \int_{0}^{t} \vec{v}(\tau) d\tau
$$

$$
x(t) = 5 + \int (2.5t^2 + 2) dt = \frac{5}{6}t^3 + 2t + 5
$$
$$
y(t) = 2 + \int (0.5t^2 - 4t) dt = \frac{1}{6}t^3 - 2t^2 + 2
$$
$$
z(t) = -3 + \int (-\frac{2}{3}t^3 + 1) dt = -\frac{1}{6}t^4 + t - 3
$$

## Final Result

The trajectory is given by:

$$
\vec{r}(t) = \begin{pmatrix} \frac{5}{6}t^3 + 2t + 5 \\ \frac{1}{6}t^3 - 2t^2 + 2 \\ -\frac{1}{6}t^4 + t - 3 \end{pmatrix} \text{ m}
$$