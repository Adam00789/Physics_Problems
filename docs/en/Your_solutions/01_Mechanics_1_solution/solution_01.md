# Problem Set 01 – Solutions

---

# Task 01 – Projectile Motion

## Problem Statement

A projectile is launched from the ground with an initial velocity of $100 \text{ m/s}$ at an angle of $37^\circ$ above the horizontal. Air resistance is neglected.

Determine:

- The differential equations of motion
- The time of flight
- The maximum height
- The range

---

## Theory

Projectile motion under constant gravitational acceleration is described by Newton’s second law.

- Horizontal acceleration: $a_x = 0$
- Vertical acceleration: $a_y = -g$

where $g \approx 9.8 \text{ m/s}^2$.

The initial velocity components are:

$$
v_{0x} = v_0 \cos\theta
$$

$$
v_{0y} = v_0 \sin\theta
$$

---

## Step-by-Step Solution

### Differential Equations of Motion

From Newton’s second law:

$$
\frac{d^2 x}{dt^2} = 0
$$

$$
\frac{d^2 y}{dt^2} = -g
$$

Integrating once:

$$
\frac{dx}{dt} = v_{0x}
$$

$$
\frac{dy}{dt} = v_{0y} - gt
$$

Integrating again:

$$
x(t) = v_{0x} t
$$

$$
y(t) = v_{0y} t - \frac{1}{2} g t^2
$$

---

### Initial Velocity Components

Given $v_0 = 100$ m/s and $\theta = 37^\circ$:

$$
v_{0x} = 100 \cos(37^\circ)
$$

$$
v_{0y} = 100 \sin(37^\circ)
$$

Using approximations:

$$
\cos(37^\circ) \approx 0.8, \quad \sin(37^\circ) \approx 0.6
$$

$$
v_{0x} \approx 80 \text{ m/s}, \quad v_{0y} \approx 60 \text{ m/s}
$$

---

### Time of Flight

The projectile returns to the ground when $y(t) = 0$:

$$
0 = v_{0y} t - \frac{1}{2} g t^2
$$

Factor:

$$
t \left(v_{0y} - \frac{1}{2} g t \right) = 0
$$

Non-zero solution:

$$
t = \frac{2 v_{0y}}{g}
$$

Substitute:

$$
t = \frac{2 \cdot 60}{9.8}
$$

$$
t \approx 12.24 \text{ s}
$$

---

### Maximum Height

At maximum height, vertical velocity is zero:

$$
v_y = v_{0y} - gt = 0
$$

Solve for time:

$$
t = \frac{v_{0y}}{g}
$$

Height:

$$
H = v_{0y} t - \frac{1}{2} g t^2
$$

Substitute:

$$
H = \frac{v_{0y}^2}{2g}
$$

$$
H = \frac{60^2}{2 \cdot 9.8}
$$

$$
H \approx 183.7 \text{ m}
$$

---

### Range

Range is horizontal distance at total flight time:

$$
R = v_{0x} \cdot t
$$

$$
R = 80 \cdot 12.24
$$

$$
R \approx 979.2 \text{ m}
$$

---

## Final Result

- Differential equations:

$$
\frac{d^2 x}{dt^2} = 0, \quad \frac{d^2 y}{dt^2} = -g
$$

- Time of flight:

$$
t \approx 12.24 \text{ s}
$$

- Maximum height:

$$
H \approx 183.7 \text{ m}
$$

- Range:

$$
R \approx 979.2 \text{ m}
$$

---

## Interpretation

The motion is a combination of uniform motion in the horizontal direction and uniformly accelerated motion in the vertical direction.

The trajectory is parabolic, and the symmetry of motion ensures that the ascent and descent times are equal.

Neglecting air resistance results in an idealized trajectory with maximum range determined solely by the initial velocity and launch angle.