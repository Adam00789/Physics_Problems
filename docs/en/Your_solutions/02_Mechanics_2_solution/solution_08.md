<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 08 – Work of a Variable Force

## Problem Statement

Given a one-dimensional force $F(x) = -kx$:
1. Write down the equation of motion and solve it.
2. Calculate the work done during the displacement from $0$ to $x_0$.
3. Interpret the result as potential energy.
4. Verify the relationship $F = -\frac{dU}{dx}$.
5. Draw the graph of $F(x)$ and $U(x)$.

## Theory

A force proportional to displacement and directed toward the equilibrium point is a restoring force, leading to Simple Harmonic Motion (SHM). Work done by a variable force is the integral of the force over the displacement:

$$
W = \int_{x_i}^{x_f} F(x) dx
$$

## Step-by-Step Solution

### 1. Equation of Motion

Applying Newton's Second Law:

$$
m \frac{d^2 x}{dt^2} = -kx \implies \ddot{x} + \frac{k}{m}x = 0
$$

This is a second-order linear homogeneous differential equation. The solution is:

$$
x(t) = A \cos(\omega t + \phi), \quad \omega = \sqrt{\frac{k}{m}}
$$

### 2. Work Done

$$
W = \int_{0}^{x_0} (-kx) dx = \left[ -\frac{1}{2} k x^2 \right]_{0}^{x_0} = -\frac{1}{2} k x_0^2
$$

### 3. Interpretation as Potential Energy

The work done **by the field** is negative, meaning the field opposes the displacement. The potential energy $U(x)$ is defined as the work done by an **external agent** to move the particle from $0$ to $x_0$ without change in kinetic energy:

$$
U(x) = -W = \frac{1}{2} k x^2
$$

### 4. Verification

$$
-\frac{dU}{dx} = -\frac{d}{dx} \left( \frac{1}{2} k x^2 \right) = - \left( \frac{1}{2} k \cdot 2x \right) = -kx
$$

Since $-kx = F(x)$, the relationship is verified.

## Final Result

* **Equation:** $x(t) = A \cos(\omega t + \phi)$.
* **Work:** $W = -\frac{1}{2} k x_0^2$.
* **Potential Energy:** $U(x) = \frac{1}{2} k x^2$.

## Interpretation



The force $F(x)$ is a linear function with a negative slope, indicating it always pulls the object back to $x=0$. The potential energy $U(x)$ is a parabola, showing that energy increases quadratically as the particle moves away from equilibrium in either direction.