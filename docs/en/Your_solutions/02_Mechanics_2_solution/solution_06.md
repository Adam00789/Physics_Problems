<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 06 – Energy Dissipation

## Problem Statement

A tennis ball is dropped from a height of $2.0 \text{ m}$. After each bounce, it loses $30\%$ of its mechanical energy. To what height does it rise after the second bounce?

## Theory

The mechanical energy of the ball at its maximum height $h$ is purely gravitational potential energy:

$$
E = mgh
$$

If the ball loses $30\%$ of its energy, it retains $70\%$ (or a factor of $0.7$) of its energy after each impact. Since $E \propto h$, the height reached after a bounce is directly proportional to the energy remaining:

$$
h_{n} = e \cdot h_{n-1}
$$

Where $e$ is the energy retention coefficient ($0.7$ in this case).

## Step-by-Step Solution

### 1. Energy after First Bounce

The energy after the first bounce ($E_1$) is $70\%$ of the initial energy ($E_0$):

$$
E_1 = 0.7 E_0 \implies h_1 = 0.7 h_0
$$

### 2. Energy after Second Bounce

The energy after the second bounce ($E_2$) is $70\%$ of the energy after the first bounce:

$$
E_2 = 0.7 E_1 = 0.7(0.7 E_0) = 0.49 E_0
$$

### 3. Final Height Calculation

Using $h_0 = 2.0 \text{ m}$:

$$
h_2 = 0.49 \times 2.0
$$

$$
h_2 = 0.98 \text{ m}
$$

## Final Result

The ball rises to a height of **$0.98 \text{ m}$** after the second bounce.

## Interpretation

Each bounce represents a non-conservative interaction where energy is dissipated through the deformation of the ball and the surface, as well as sound. Because height scales linearly with potential energy, the height follows a geometric progression $h_n = h_0 (0.7)^n$.