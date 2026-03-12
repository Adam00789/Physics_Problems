<h1 style="color:#6CB6FF">Section 1 – Mechanics I</h1>

---

<h1 style="color:#6CB6FF">Task 01 – Projectile Motion</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

A projectile is fired from the ground with an initial velocity

$v_0 = 100 \text{ m/s}$

at an angle

$\theta = 37^\circ$

above the horizontal. Air resistance is neglected.

Determine:

- the differential equations of motion
- the time of flight
- the maximum height
- the range

<h2 style="color:#6CB6FF">Theory</h2>

In projectile motion the only force acting on the object is gravity.

The acceleration vector is

$$
\vec a =
\begin{pmatrix}
0 \\
- g
\end{pmatrix}
$$

The horizontal and vertical motions are independent.

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

<h3 style="color:#6CB6FF">Differential Equations</h3>

Horizontal motion

$$
\frac{d^2 x}{dt^2} = 0
$$

Vertical motion

$$
\frac{d^2 y}{dt^2} = -g
$$

<h3 style="color:#6CB6FF">Initial Velocity Components</h3>

$$
v_{0x} = v_0 \cos\theta
$$

$$
v_{0y} = v_0 \sin\theta
$$

<h3 style="color:#6CB6FF">Time of Flight</h3>

The vertical position is

$$
y(t) =
v_0 \sin\theta \, t -
\frac{1}{2} g t^2
$$

Setting $y(T)=0$ gives

$$
T =
\frac{2 v_0 \sin\theta}{g}
$$

Substituting values

$$
T =
\frac{2 (100) \sin 37^\circ}{9.81}
$$

$$
T \approx 12.3 \text{ s}
$$

<h3 style="color:#6CB6FF">Maximum Height</h3>

Maximum height occurs when

$v_y = 0$

The result is

$$
H =
\frac{(v_0 \sin\theta)^2}{2g}
$$

$$
H \approx 184.7 \text{ m}
$$

<h3 style="color:#6CB6FF">Range</h3>

The horizontal range is

$$
R =
v_0 \cos\theta \cdot T
$$

$$
R \approx 983 \text{ m}
$$

<h2 style="color:#6CB6FF">Final Result</h2>

Time of flight

$T \approx 12.3 \text{ s}$

Maximum height

$H \approx 184.7 \text{ m}$

Range

$R \approx 983 \text{ m}$

<h2 style="color:#6CB6FF">Interpretation</h2>

The trajectory is parabolic because the vertical motion experiences constant gravitational acceleration while the horizontal motion has constant velocity.

---

<h1 style="color:#6CB6FF">Task 02 – Range Optimization</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

Show analytically that the projectile range

$$
R(\theta) =
\frac{v_0^2 \sin(2\theta)}{g}
$$

is maximized when

$\theta = 45^\circ$.

<h2 style="color:#6CB6FF">Theory</h2>

To determine the maximum of a function we compute its derivative and set it equal to zero.

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

$$
R(\theta) =
\frac{v_0^2}{g}\sin(2\theta)
$$

Differentiate

$$
\frac{dR}{d\theta} =
\frac{v_0^2}{g} 2\cos(2\theta)
$$

Set equal to zero

$$
\cos(2\theta)=0
$$

$$
2\theta = 90^\circ
$$

$$
\theta = 45^\circ
$$

<h2 style="color:#6CB6FF">Final Result</h2>

Maximum range occurs at

$$
\theta = 45^\circ
$$

<h2 style="color:#6CB6FF">Interpretation</h2>

At $45^\circ$ the horizontal and vertical components of the initial velocity balance in a way that maximizes horizontal displacement.

---

<h1 style="color:#6CB6FF">Task 03 – Path Intersection</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

Alice moves according to

$$
A(t) = (2+t, 8-3t)
$$

Bob moves according to

$$
B(t) = (2t-1, 2t+2)
$$

Determine whether they collide.

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

For a collision both coordinates must match.

Horizontal coordinates

$$
2 + t = 2t - 1
$$

$$
t = 3
$$

Check vertical coordinates.

Alice

$$
8 - 3(3) = -1
$$

Bob

$$
2(3) + 2 = 8
$$

Coordinates are different.

<h2 style="color:#6CB6FF">Final Result</h2>

No collision occurs.

<h2 style="color:#6CB6FF">Interpretation</h2>

The paths intersect geometrically but the objects reach the intersection point at different times.

---

<h1 style="color:#6CB6FF">Task 04 – Vector Calculus</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

The position vector is

$$
\vec r(t) =
(3t^2)\hat{i} +
(5t - 8t^2)\hat{j}
$$

Find velocity and acceleration.

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

Velocity

$$
\vec v(t) =
\frac{d\vec r}{dt}
$$

$$
\vec v(t) =
(6t)\hat{i} +
(5-16t)\hat{j}
$$

Acceleration

$$
\vec a(t) =
\frac{d\vec v}{dt}
$$

$$
\vec a(t) =
6\hat{i} - 16\hat{j}
$$

<h2 style="color:#6CB6FF">Final Result</h2>

Velocity

$$
\vec v(t) = (6t, 5-16t)
$$

Acceleration

$$
\vec a = (6,-16)
$$

<h2 style="color:#6CB6FF">Interpretation</h2>

Acceleration is constant, indicating motion under uniform force.

---

<h1 style="color:#6CB6FF">Task 05 – Relative Velocity</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

A river flows east at

$2 \text{ m/s}$

A boat can move

$5 \text{ m/s}$

in still water. The river is 200 m wide.

Determine the heading direction required to move directly north and the crossing time.

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

To cancel the river drift the boat must aim westward.

Let $\theta$ be the angle west of north.

$$
5 \sin\theta = 2
$$

$$
\sin\theta = 0.4
$$

$$
\theta \approx 23.6^\circ
$$

Northward velocity

$$
v_y = 5\cos\theta
$$

$$
v_y \approx 4.58
$$

Crossing time

$$
t = \frac{200}{4.58}
$$

$$
t \approx 43.7 \text{ s}
$$

<h2 style="color:#6CB6FF">Final Result</h2>

Heading angle

$23.6^\circ$ west of north

Crossing time

$43.7 \text{ s}$

<h2 style="color:#6CB6FF">Interpretation</h2>

The boat must aim upstream so that the river drift is exactly cancelled.

---

<h1 style="color:#6CB6FF">Task 06 – Variable Velocity</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

Velocity

$$
v(t) = t^2 + 2t -5
$$

Initial position

$x(0)=4$

Find position and acceleration at $t=3$.

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

Position from integration

$$
x(t) =
\int v(t) dt
$$

$$
x(t) =
\frac{t^3}{3} + t^2 -5t + C
$$

Using $x(0)=4$

$$
C = 4
$$

Position at $t=3$

$$
x(3) = 9 + 9 -15 +4
$$

$$
x(3)=7
$$

Acceleration

$$
a(t) =
\frac{dv}{dt}
$$

$$
a(t)=2t+2
$$

$$
a(3)=8
$$

<h2 style="color:#6CB6FF">Final Result</h2>

Position

$x(3)=7$

Acceleration

$a(3)=8$

---

<h1 style="color:#6CB6FF">Task 07 – Parametric Motion</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

$$
x(t)=2t^2
$$

$$
y(t)=3t^3
$$

Eliminate the parameter and compute velocity and acceleration.

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

Solve for $t$

$$
t=\sqrt{x/2}
$$

Substitute

$$
y=3(x/2)^{3/2}
$$

Velocity

$$
\vec v =
(4t,9t^2)
$$

Speed

$$
|\vec v| =
\sqrt{16t^2 + 81t^4}
$$

Acceleration

$$
\vec a =
(4,18t)
$$

Magnitude

$$
|\vec a| =
\sqrt{16 + 324t^2}
$$

<h2 style="color:#6CB6FF">Final Result</h2>

Acceleration is not constant.

---

<h1 style="color:#6CB6FF">Task 08 – Circular Motion</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

Find centripetal acceleration at Earth's equator.

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

Earth rotation period

$$
T = 86400
$$

Angular velocity

$$
\omega =
\frac{2\pi}{T}
$$

Radius

$$
R = 6.378\times10^6
$$

Acceleration

$$
a = \omega^2 R
$$

$$
a \approx 0.034 \text{ m/s}^2
$$

<h2 style="color:#6CB6FF">Final Result</h2>

$$
a \approx 0.034 \text{ m/s}^2
$$

---

<h1 style="color:#6CB6FF">Task 09 – Momentum Comparison</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

Compare momenta.

Fly: $2$ g at $10$ m/s

Tennis ball: $60$ g at $1$ m/s

<h2 style="color:#6CB6FF">Step-by-Step Solution</h2>

Momentum

$$
p = mv
$$

Fly

$$
p = 0.002 \times 10
$$

$$
p = 0.02
$$

Tennis ball

$$
p = 0.06 \times 1
$$

$$
p = 0.06
$$

<h2 style="color:#6CB6FF">Final Result</h2>

The tennis ball has larger momentum.

---

<h1 style="color:#6CB6FF">Task 10 – Kinematics</h1>

<h2 style="color:#6CB6FF">Problem Statement</h2>

$$
\vec r(t) =
(a\cos\omega t, b\sin\omega t, bt)
$$

<h2 style="color:#6CB6FF">Trajectory</h2>

Eliminating time

$$
\frac{x^2}{a^2} +
\frac{y^2}{b^2} = 1
$$

The motion forms a helix.

<h2 style="color:#6CB6FF">Path Length</h2>

Velocity magnitude

$$
|\vec v| =
\sqrt{a^2\omega^2\sin^2(\omega t) +
b^2\omega^2\cos^2(\omega t) +
b^2}
$$

Arc length

$$
s =
\int_0^{t_0}
|\vec v| dt
$$

<h2 style="color:#6CB6FF">Interpretation</h2>

The motion represents a **helical trajectory** rising along the $z$ axis.