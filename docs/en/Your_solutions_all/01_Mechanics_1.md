FILE: problem_set_01_solutions.md

```markdown
# Problem Set 01 – Solutions

# Task 01 – Projectile Motion

## Problem Statement

A projectile is fired from the ground with an initial velocity of $100 \text{ m/s}$ at an angle of $37^\circ$ above the horizontal. Assume no air resistance. Derive the differential equations of motion, and determine the time of flight, maximum height, and range.



## Theory

Projectile motion is a form of two-dimensional motion under constant acceleration due to gravity. By separating the motion into horizontal ($x$) and vertical ($y$) components, the physical behavior can be described by Newton's second law.

## Step-by-Step Solution

The initial velocity components are given by

$$
v_{0x} = v_0 \cos(\theta)
$$

$$
v_{0y} = v_0 \sin(\theta)
$$

Given $v_0 = 100 \text{ m/s}$ and $\theta = 37^\circ$, these evaluate to

$$
v_{0x} = 100 \cos(37^\circ) \approx 79.86 \text{ m/s}
$$

$$
v_{0y} = 100 \sin(37^\circ) \approx 60.18 \text{ m/s}
$$

The differential equations of motion are derived from the fact that acceleration is purely vertical.

$$
\begin{align}
\frac{d^2x}{dt^2} &= 0 \\
\frac{d^2y}{dt^2} &= -g
\end{align}
$$

Integrating these equations with respect to time yields the velocity and position functions.

$$
\begin{align}
v_x(t) &= v_{0x} \\
v_y(t) &= v_{0y} - gt \\
x(t) &= v_{0x}t \\
y(t) &= v_{0y}t - \frac{1}{2}gt^2
\end{align}
$$

The time of flight $T$ occurs when the projectile returns to the ground, $y(T) = 0$.

$$
0 = v_{0y}T - \frac{1}{2}gT^2
$$

Assuming $T \neq 0$,

$$
T = \frac{2v_{0y}}{g}
$$

$$
T = \frac{2(60.18)}{9.81} \approx 12.27 \text{ s}
$$

The maximum height $H$ is reached when the vertical velocity is zero, $v_y(t) = 0$. The time to reach this height is $t_h = T / 2 \approx 6.13 \text{ s}$.

$$
H = y(t_h) = v_{0y}\left(\frac{v_{0y}}{g}\right) - \frac{1}{2}g\left(\frac{v_{0y}}{g}\right)^2
$$

$$
H = \frac{v_{0y}^2}{2g} = \frac{(60.18)^2}{2(9.81)} \approx 184.5 \text{ m}
$$

The range $R$ is the horizontal distance traveled during the time of flight.

$$
R = x(T) = v_{0x}T = 79.86(12.27) \approx 980 \text{ m}
$$

## Final Result

- Time of flight: $12.27 \text{ s}$
- Maximum height: $184.5 \text{ m}$
- Range: $980 \text{ m}$

## Interpretation

The decoupling of horizontal and vertical axes allows for independent solutions. The horizontal motion proceeds at a constant velocity, while the vertical motion is subject to uniform gravitational acceleration.

---

# Task 02 – Range Optimization

## Problem Statement

Show analytically that the maximum range $R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$ for a given initial velocity is achieved at a launch angle of $45^\circ$.

## Theory

The maximum of a continuous, differentiable function over an interval can be found by taking the first derivative with respect to the variable of interest and setting it to zero.

## Step-by-Step Solution

The range function depends on the launch angle $\theta$.

$$
R(\theta) = \frac{v_0^2}{g} \sin(2\theta)
$$

To find the angle that maximizes $R$, the derivative of $R$ with respect to $\theta$ is calculated.

$$
\frac{dR}{d\theta} = \frac{d}{d\theta} \left[ \frac{v_0^2}{g} \sin(2\theta) \right]
$$

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \cos(2\theta) \cdot 2
$$

Set the derivative equal to zero to identify critical points.

$$
\frac{2v_0^2}{g} \cos(2\theta) = 0
$$

Since the physical launch angle must lie in the interval $[0, \frac{\pi}{2}]$,

$$
\cos(2\theta) = 0
$$

$$
2\theta = \frac{\pi}{2}
$$

$$
\theta = \frac{\pi}{4} = 45^\circ
$$

To verify this is a maximum, the second derivative is evaluated.

$$
\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g} \sin(2\theta)
$$

For $\theta = 45^\circ$, the second derivative is negative, confirming a maximum.

## Final Result

The maximum range is achieved at $\theta = 45^\circ$.

## Interpretation

A $45^\circ$ angle provides the optimal trade-off between the time the projectile remains in the air (which favors higher angles) and the horizontal speed at which it travels (which favors lower angles).

---

# Task 03 – Path Intersection

## Problem Statement

Alice moves along $A(t) = (2+t, 8-3t)$ and Bob moves along $B(t) = (2t-1, 2t+2)$. Determine if their paths intersect. If yes, determine when and where they collide. If not, determine the minimum distance between them and when it occurs.



## Theory

Intersection of paths means the trajectories share a spatial coordinate, though not necessarily at the same time. Collision requires both the same spatial coordinate and the same time parameter. Distance between two points in a Cartesian plane is found via the Euclidean distance formula.

## Step-by-Step Solution

First, determine if the paths intersect in space. For Alice's path, isolating $t$ yields

$$
t = x_A - 2
$$

$$
y_A = 8 - 3(x_A - 2) = 14 - 3x_A
$$

For Bob's path, isolating $t$ yields

$$
t = \frac{x_B + 1}{2}
$$

$$
y_B = 2\left(\frac{x_B + 1}{2}\right) + 2 = x_B + 3
$$

Equating the spatial trajectories $y_A = y_B$ to find an intersection point

$$
14 - 3x = x + 3
$$

$$
4x = 11
$$

$$
x = 2.75
$$

The paths cross at $x = 2.75$ and $y = 5.75$. Next, check if a collision occurs by checking the times at this intersection.

For Alice,

$$
2 + t_A = 2.75 \implies t_A = 0.75 \text{ s}
$$

For Bob,

$$
2t_B - 1 = 2.75 \implies t_B = 1.875 \text{ s}
$$

Since $t_A \neq t_B$, they do not collide. To find the minimum distance, define the squared distance function $D^2(t)$.

$$
D^2(t) = (x_B(t) - x_A(t))^2 + (y_B(t) - y_A(t))^2
$$

$$
D^2(t) = ((2t - 1) - (2 + t))^2 + ((2t + 2) - (8 - 3t))^2
$$

$$
D^2(t) = (t - 3)^2 + (5t - 6)^2
$$

Minimize $D^2(t)$ by differentiating with respect to $t$.

$$
\frac{d(D^2)}{dt} = 2(t - 3) + 2(5t - 6)(5)
$$

$$
\frac{d(D^2)}{dt} = 2t - 6 + 50t - 60 = 52t - 66
$$

Set to zero to find the critical time.

$$
52t - 66 = 0
$$

$$
t = \frac{66}{52} \approx 1.27 \text{ s}
$$

Substitute this back into $D^2(t)$ to find the minimal distance.

$$
D^2(1.27) = \left(\frac{66}{52} - \frac{156}{52}\right)^2 + \left(5\left(\frac{66}{52}\right) - \frac{312}{52}\right)^2
$$

$$
D^2(1.27) = \left(-\frac{90}{52}\right)^2 + \left(\frac{18}{52}\right)^2 = \frac{8100 + 324}{2704} \approx 3.115 \text{ m}^2
$$

$$
D = \sqrt{3.115} \approx 1.76 \text{ m}
$$

## Final Result

The paths intersect spatially, but there is no collision. The minimum distance is $1.76 \text{ m}$ at time $t = 1.27 \text{ s}$.

## Interpretation

While the linear trajectories cross in space, the differing velocities and starting positions mean the objects pass through the intersection point at different times. 

---

# Task 04 – Vector Calculus

## Problem Statement

The position of an object is given by $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$. Find the object's velocity and acceleration vectors as a function of time.

## Theory

Velocity is the first derivative of the position vector with respect to time. Acceleration is the second time derivative.

## Step-by-Step Solution

The position vector is

$$
\vec{r}(t) =
\begin{pmatrix}
3t^2 \\
5t - 8t^2
\end{pmatrix}
$$

Differentiating with respect to time yields the velocity vector $\vec{v}(t)$.

$$
\begin{align}
\vec{v}(t) &= \frac{d\vec{r}}{dt} \\
           &= \begin{pmatrix} \frac{d}{dt}(3t^2) \\ \frac{d}{dt}(5t - 8t^2) \end{pmatrix} \\
           &= \begin{pmatrix} 6t \\ 5 - 16t \end{pmatrix}
\end{align}
$$

Differentiating velocity with respect to time yields the acceleration vector $\vec{a}(t)$.

$$
\begin{align}
\vec{a}(t) &= \frac{d\vec{v}}{dt} \\
           &= \begin{pmatrix} \frac{d}{dt}(6t) \\ \frac{d}{dt}(5 - 16t) \end{pmatrix} \\
           &= \begin{pmatrix} 6 \\ -16 \end{pmatrix}
\end{align}
$$

## Final Result

The velocity vector is $\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$. The acceleration vector is constant: $\vec{a}(t) = 6\hat{i} - 16\hat{j}$.

## Interpretation

Because the position vector components are quadratic polynomials, the velocity is linear with time, and the resulting acceleration vector is constant.

---

# Task 05 – Relative Velocity

## Problem Statement

A river flows east at $2 \text{ m/s}$. A boat that can travel at $5 \text{ m/s}$ in still water wants to go directly north. In what direction should it head? How long will it take to cross if the river is 200 meters wide?



## Theory

The velocity of the boat with respect to the ground is the vector sum of the velocity of the boat with respect to the water and the velocity of the water with respect to the ground.

$$
\vec{v}_{bg} = \vec{v}_{bw} + \vec{v}_{wg}
$$

## Step-by-Step Solution

The water flows east, giving the water velocity vector.

$$
\vec{v}_{wg} =
\begin{pmatrix}
2 \\
0
\end{pmatrix}
$$

The boat must travel purely north relative to the ground.

$$
\vec{v}_{bg} =
\begin{pmatrix}
0 \\
v_y
\end{pmatrix}
$$

The boat's speed in still water is the magnitude of $\vec{v}_{bw}$, which is $5 \text{ m/s}$. The relationship between the velocity components is

$$
\begin{pmatrix} 0 \\ v_y \end{pmatrix} = \begin{pmatrix} v_{bx} \\ v_{by} \end{pmatrix} + \begin{pmatrix} 2 \\ 0 \end{pmatrix}
$$

This requires $v_{bx} + 2 = 0$, leading to $v_{bx} = -2 \text{ m/s}$. The boat must head west to counteract the current. The vertical component is found using the magnitude.

$$
|\vec{v}_{bw}| = \sqrt{v_{bx}^2 + v_{by}^2} = 5
$$

$$
(-2)^2 + v_{by}^2 = 25
$$

$$
v_{by} = \sqrt{21} \approx 4.58 \text{ m/s}
$$

The heading angle $\theta$ relative to the north (y-axis) is

$$
\sin(\theta) = \frac{|v_{bx}|}{|\vec{v}_{bw}|} = \frac{2}{5}
$$

$$
\theta = \arcsin(0.4) \approx 23.6^\circ \text{ West of North}
$$

The time required to cross the 200-meter river uses the northward component of velocity.

$$
t = \frac{d}{v_{by}} = \frac{200}{\sqrt{21}} \approx 43.64 \text{ s}
$$

## Final Result

The boat should head $23.6^\circ$ West of North. It will take approximately $43.64 \text{ s}$ to cross.

## Interpretation

The boat sacrifices a portion of its speed capability to fight the current. Consequently, its effective speed across the river ($\approx 4.58 \text{ m/s}$) is lower than its speed in still water ($5 \text{ m/s}$).

---

# Task 06 – Variable Velocity

## Problem Statement

An object's velocity is given by $v(t) = t^2 + 2t - 5$. If the object was at $x=4$ at $t=0$, what is its position and acceleration at time $t=3$?

## Theory

Position is the integral of velocity with respect to time, evaluated with an initial condition. Acceleration is the first derivative of velocity with respect to time.

## Step-by-Step Solution

Acceleration is derived first.

$$
\begin{align}
a(t) &= \frac{dv}{dt} \\
     &= \frac{d}{dt}(t^2 + 2t - 5) \\
     &= 2t + 2
\end{align}
$$

Evaluating at $t=3$,

$$
a(3) = 2(3) + 2 = 8 \text{ m/s}^2
$$

Position $x(t)$ is found by integrating $v(t)$.

$$
\begin{align}
x(t) &= \int v(t) dt \\
     &= \int (t^2 + 2t - 5) dt \\
     &= \frac{1}{3}t^3 + t^2 - 5t + C
\end{align}
$$

Apply the initial condition $x(0) = 4$ to solve for $C$.

$$
x(0) = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C = 4
$$

$$
C = 4
$$

The complete position function is

$$
x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4
$$

Evaluate at $t=3$.

$$
x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4
$$

$$
x(3) = 9 + 9 - 15 + 4 = 7 \text{ m}
$$

## Final Result

At $t=3$, the position is $7 \text{ m}$ and the acceleration is $8 \text{ m/s}^2$.

## Interpretation

The polynomial form of the velocity indicates non-constant acceleration. The constants of integration are critical to anchor the function to the specified physical starting point.

---

# Task 07 – Elimination of time and interpretation of acceleration

## Problem Statement

The path equation is $x(t)=2t^2, y(t)=3t^3$. Eliminate the parameter $t$. Calculate $\vec{v}(t), |\vec{v}(t)|, \vec{a}(t)$ and $|\vec{a}(t)|$. Is the acceleration constant?

## Theory

Parametric equations can be converted to Cartesian equations by solving one equation for the parameter and substituting it into the other. Kinematic vectors are derivatives of the position vector.

## Step-by-Step Solution

To eliminate $t$, rearrange the $x(t)$ equation.

$$
t = \sqrt{\frac{x}{2}}
$$

Substitute this into $y(t)$.

$$
y(x) = 3\left(\sqrt{\frac{x}{2}}\right)^3 = \frac{3}{2\sqrt{2}} x^{3/2}
$$

Calculate the velocity vector.

$$
\vec{v}(t) = \begin{pmatrix} \frac{dx}{dt} \\ \frac{dy}{dt} \end{pmatrix} = \begin{pmatrix} 4t \\ 9t^2 \end{pmatrix}
$$

The magnitude of velocity is

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = t\sqrt{16 + 81t^2}
$$

Calculate the acceleration vector.

$$
\vec{a}(t) = \begin{pmatrix} \frac{dv_x}{dt} \\ \frac{dv_y}{dt} \end{pmatrix} = \begin{pmatrix} 4 \\ 18t \end{pmatrix}
$$

The magnitude of acceleration is

$$
|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \sqrt{16 + 324t^2} = 2\sqrt{4 + 81t^2}
$$

## Final Result

The path equation is $y(x) = \frac{3}{2\sqrt{2}} x^{3/2}$. Acceleration is not constant because the $y$-component depends on time $t$. 

## Interpretation

A trajectory of the form $x^{3/2}$ describes a curve starting from the origin. The acceleration vector grows over time due to the cubic nature of the $y$-position component.

---

# Task 08 – Circular Motion

## Problem Statement

Calculate the centripetal acceleration of a person standing on the Earth's equator. The Earth's radius is $6378 \text{ km}$.

## Theory

An object in uniform circular motion experiences a centripetal acceleration directed toward the center of rotation, depending on the angular velocity and radius.

$$
a_c = \omega^2 r
$$

## Step-by-Step Solution

First, determine the angular velocity $\omega$ of the Earth. The Earth completes one full rotation ($2\pi$ radians) in approximately 24 hours.

$$
\omega = \frac{2\pi}{T}
$$

$$
T = 24 \text{ hours} = 24 \times 60 \times 60 = 86400 \text{ s}
$$

$$
\omega = \frac{2\pi}{86400} \approx 7.27 \times 10^{-5} \text{ rad/s}
$$

The radius is $r = 6378 \text{ km} = 6378 \times 10^3 \text{ m}$. Calculate the centripetal acceleration.

$$
a_c = (7.27 \times 10^{-5})^2 (6378 \times 10^3)
$$

$$
a_c \approx 0.0337 \text{ m/s}^2
$$

## Final Result

The centripetal acceleration is approximately $0.0337 \text{ m/s}^2$.

## Interpretation

This acceleration is very small compared to gravity ($9.81 \text{ m/s}^2$). It slightly reduces the apparent weight of a person at the equator compared to someone at the poles.

---

# Task 09 – Momentum Comparison

## Problem Statement

Which has greater momentum: a 2-gram fly flying at $10 \text{ m/s}$ or a 60-gram tennis ball moving at $1 \text{ m/s}$?

## Theory

Linear momentum $p$ is the product of an object's mass and velocity.

$$
p = mv
$$

## Step-by-Step Solution

Calculate momentum for the fly. Convert mass to kilograms.

$$
m_{\text{fly}} = 0.002 \text{ kg}
$$

$$
p_{\text{fly}} = (0.002 \text{ kg})(10 \text{ m/s}) = 0.02 \text{ kg}\cdot\text{m/s}
$$

Calculate momentum for the tennis ball.

$$
m_{\text{ball}} = 0.060 \text{ kg}
$$

$$
p_{\text{ball}} = (0.060 \text{ kg})(1 \text{ m/s}) = 0.06 \text{ kg}\cdot\text{m/s}
$$

Compare the magnitudes.

$$
0.06 > 0.02
$$

## Final Result

The tennis ball has the greater momentum ($0.06 \text{ kg}\cdot\text{m/s}$ compared to $0.02 \text{ kg}\cdot\text{m/s}$).

## Interpretation

Despite the fly's significantly higher speed, the mass difference dominates the momentum equation. 

---

# Task 10 – Kinematics

## Problem Statement

Point M moves according to $\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)$. Find the trajectory equation, compute the path length from $t=0$ to $t=t_0$, and discuss special cases.



## Theory

The path length $s$ is computed by integrating the magnitude of the velocity vector over time.

$$
s = \int_{0}^{t_0} |\vec{v}(t)| dt
$$

## Step-by-Step Solution

**a) Equation of the trajectory**

By isolating the trigonometric terms in $x$ and $y$, the standard form of an ellipse in the $xy$-plane emerges.

$$
\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = \cos^2(\omega t) + \sin^2(\omega t) = 1
$$

In 3D, this trajectory is an elliptical helix, propagating along the z-axis according to $z(t) = bt$.

**b) Path length**

Calculate the velocity vector components.

$$
\vec{v}(t) = \begin{pmatrix} -a\omega \sin(\omega t) \\ b\omega \cos(\omega t) \\ b \end{pmatrix}
$$

Calculate the magnitude of velocity.

$$
|\vec{v}(t)| = \sqrt{(-a\omega \sin(\omega t))^2 + (b\omega \cos(\omega t))^2 + b^2}
$$

The path length integral is

$$
s = \int_{0}^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2} \: dt
$$

This is generally an elliptic integral, depending on the constants.

**c) Special cases (Trajectory drawing theory)**

A Python snippet to draw this requires parameterizing over $t$.

```python
import numpy as np
import matplotlib.pyplot as plt

t = np.linspace(0, 10, 1000)
a, b, w = 2, 1, 1
x = a * np.cos(w * t)
y = b * np.sin(w * t)
z = b * t

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')
ax.plot(x, y, z)
plt.show()

```

If $a = b$, the base of the cylinder is circular rather than elliptical, yielding a standard circular helix. If $b = 0$, the particle undergoes simple harmonic motion on the x-axis.

## Final Result

The trajectory is an elliptical helix. The path length is given by an integral involving $\sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}$.

## Interpretation

The formulation combines 2D cyclical motion (represented by sine and cosine) with linear translation in the third dimension, mapping out a helical path commonly found in particle physics involving magnetic fields.

```

```