<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 03 – Conservation of Energy

## Problem Statement

A pendulum with a length of $1.0$ meter is released from an initial angle of $15^\circ$. What is the speed of the pendulum bob at the bottom of its swing?

## Theory

According to the Law of Conservation of Energy, the total mechanical energy (Potential + Kinetic) remains constant if non-conservative forces like air resistance are neglected:

$$
E_{top} = E_{bottom}
$$

At the release point (height $h$), the energy is purely potential ($mgh$). At the bottom ($h=0$), the energy is purely kinetic ($\frac{1}{2}mv^2$). 

The height $h$ can be determined via trigonometry:

$$
h = L - L\cos\theta = L(1 - \cos\theta)
$$

## Step-by-Step Solution

### 1. Energy Equality

$$
mgh = \frac{1}{2}mv^2
$$

Solving for $v$:

$$
v = \sqrt{2gh}
$$

### 2. Height Calculation

Given $L = 1.0 \text{ m}$ and $\theta = 15^\circ$:

$$
h = 1.0 \times (1 - \cos(15^\circ))
$$

$$
h \approx 1.0 \times (1 - 0.9659) = 0.0341 \text{ m}
$$

### 3. Velocity Calculation

$$
v = \sqrt{2 \times 9.81 \times 0.0341}
$$

$$
v = \sqrt{0.669} \approx 0.818 \text{ m/s}
$$

## Final Result

The speed of the pendulum bob at the bottom of the swing is **$0.818 \text{ m/s}$**.

## Interpretation

The velocity at the bottom is independent of the mass of the bob. This is because both the gravitational potential energy and the kinetic energy are proportional to mass, so it cancels out during the derivation.