<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 12 – Work and Energy with a Constant Force

## Problem Statement

A constant force acts on $m = 2 \text{ kg}$: $\vec{F} = (6, 2) \text{ N}$.
Initial: $\vec{v}_0 = (1, -1) \text{ m/s}$, $\vec{r}_0 = (0, 0) \text{ m}$.
Calculate work at $t=3 \text{ s}$ and verify the work-energy theorem.

## Step-by-Step Solution

### 1. Kinematics

$$
\vec{a} = \frac{\vec{F}}{m} = (3, 1) \text{ m/s}^2
$$
$$
\vec{v}(t) = (3t+1, t-1) \implies \vec{v}(3) = (10, 2)
$$
$$
\vec{r}(t) = (1.5t^2 + t, 0.5t^2 - t) \implies \vec{r}(3) = (16.5, 1.5)
$$

### 2. Work Calculation

$$
W = \vec{F} \cdot \Delta \vec{r} = (6)(16.5) + (2)(1.5) = 99 + 3 = 102 \text{ J}
$$

### 3. Work-Energy Theorem

$$
KE_i = \frac{1}{2}(2)(1^2 + (-1)^2) = 2 \text{ J}
$$
$$
KE_f = \frac{1}{2}(2)(10^2 + 2^2) = 104 \text{ J}
$$
$$
\Delta KE = 104 - 2 = 102 \text{ J}
$$

## Final Result

The work done is **$102 \text{ J}$**, which exactly matches the change in kinetic energy.