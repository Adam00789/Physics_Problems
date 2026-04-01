<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 02 – Harmonic Motion

## Problem Statement

A $10 \text{ kg}$ mass is attached to a spring and oscillates according to the equation $x(t) = 0.2 \cos(10\pi t)$ (in meters). What is the spring constant $k$? What is the total mechanical energy of the system?

## Theory

For a mass $m$ on a spring, the displacement $x(t)$ follows:

$$
x(t) = A \cos(\omega t + \phi)
$$

The angular frequency is related to the spring constant $k$ and mass $m$ by:

$$
\omega = \sqrt{\frac{k}{m}}
$$

The total mechanical energy $E$ is:

$$
E = \frac{1}{2} k A^2
$$

## Step-by-Step Solution

### 1. Determining the Spring Constant

From $x(t) = 0.2 \cos(10\pi t)$:
* $A = 0.2 \text{ m}$
* $\omega = 10\pi \text{ rad/s}$
* $m = 10 \text{ kg}$

$$
k = m \omega^2 = 10 \times (10\pi)^2 = 1000\pi^2 \approx 9870 \text{ N/m}
$$

### 2. Determining Total Mechanical Energy

$$
E = \frac{1}{2} k A^2 = \frac{1}{2} (1000\pi^2) (0.2)^2 = 20\pi^2 \approx 197.4 \text{ J}
$$

## Final Result

* The spring constant $k$ is **$1000\pi^2 \text{ N/m}$**.
* The total mechanical energy $E$ is **$20\pi^2 \text{ J}$**.

## Interpretation

The high spring constant indicates a very stiff system, leading to a high oscillation frequency despite the $10 \text{ kg}$ mass.