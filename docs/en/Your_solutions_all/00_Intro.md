# Problem Set 01 – Solutions

---

# Task 01 – Vector Algebra

## Problem Statement

Given two vectors in three-dimensional space

$
\vec{a} = (2,1,-3)
$

$
\vec{b} = (4,-2,1)
$

Determine:

1. The magnitude of each vector  
2. The dot product  
3. The cross product  
4. The angle between the vectors

---

## Theory

### Vector Magnitude

The magnitude of a vector

$
\vec{v} = (v_x, v_y, v_z)
$

is defined as

$$
|\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}
$$

---

### Dot Product

The dot product of two vectors

$
\vec{a} = (a_x,a_y,a_z)
$

$
\vec{b} = (b_x,b_y,b_z)
$

is

$$
\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z
$$

It is also related to the angle between vectors:

$$
\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos\theta
$$

---

### Cross Product

The cross product produces a vector perpendicular to both inputs.

$$
\vec{a} \times \vec{b} =
\begin{pmatrix}
a_y b_z - a_z b_y \\
a_z b_x - a_x b_z \\
a_x b_y - a_y b_x
\end{pmatrix}
$$

---

### Angle Between Vectors

The angle is obtained from

$$
\cos\theta =
\frac{\vec{a}\cdot\vec{b}}{|\vec{a}| |\vec{b}|}
$$

---

## Step-by-Step Solution

### Magnitude of Vector a

$$
|\vec{a}| =
\sqrt{2^2 + 1^2 + (-3)^2}
$$

$$
|\vec{a}| =
\sqrt{4 + 1 + 9}
$$

$$
|\vec{a}| =
\sqrt{14}
$$

---

### Magnitude of Vector b

$$
|\vec{b}| =
\sqrt{4^2 + (-2)^2 + 1^2}
$$

$$
|\vec{b}| =
\sqrt{16 + 4 + 1}
$$

$$
|\vec{b}| =
\sqrt{21}
$$

---

### Dot Product

$$
\vec{a}\cdot\vec{b}
=
2\cdot4 + 1\cdot(-2) + (-3)\cdot1
$$

$$
=
8 - 2 - 3
$$

$$
=
3
$$

---

### Cross Product

Using the component definition

$$
\vec{a}\times\vec{b} =
\begin{pmatrix}
1\cdot1 - (-3)(-2) \\
(-3)4 - 2\cdot1 \\
2(-2) - 1\cdot4
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 - 6 \\
-12 - 2 \\
-4 - 4
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
-5 \\
-14 \\
-8
\end{pmatrix}
$$

---

### Angle Between Vectors

First compute the cosine of the angle.

$$
\cos\theta =
\frac{3}{\sqrt{14}\sqrt{21}}
$$

$$
\cos\theta =
\frac{3}{\sqrt{294}}
$$

The angle is therefore

$$
\theta =
\cos^{-1}
\left(
\frac{3}{\sqrt{294}}
\right)
$$

Numerically

$$
\theta \approx 79.9^\circ
$$

---

## Final Result

Magnitudes

$
|\vec{a}| = \sqrt{14}
$

$
|\vec{b}| = \sqrt{21}
$

Dot product

$
\vec{a}\cdot\vec{b} = 3
$

Cross product

$
\vec{a}\times\vec{b} = (-5,-14,-8)
$

Angle

$
\theta \approx 79.9^\circ
$

---

## Interpretation

The positive dot product indicates that the angle between the vectors is **acute**.  
The cross product vector is perpendicular to both original vectors and defines the orientation of the plane containing them.

---

# Task 02 – Systems of Equations

## Problem Statement

Solve the system

$
2x + 3y = 12
$

$
x - y = 1
$

---

## Theory

A system of linear equations can be solved by substitution.

If one equation isolates a variable, the expression can be substituted into the other equation.

---

## Step-by-Step Solution

From the second equation

$$
x - y = 1
$$

solve for $x$

$$
x = 1 + y
$$

Substitute into the first equation.

$$
2(1+y) + 3y = 12
$$

Expand.

$$
2 + 2y + 3y = 12
$$

Combine terms.

$$
2 + 5y = 12
$$

$$
5y = 10
$$

$$
y = 2
$$

Substitute back into

$
x = 1 + y
$

$$
x = 3
$$

---

## Final Result

$
x = 3
$

$
y = 2
$

---

## Interpretation

The two equations represent straight lines in the plane.  
The solution $(3,2)$ corresponds to their **intersection point**.

---

# Task 03 – Proportionality in Gravitation

## Problem Statement

The gravitational force between two masses is

$$
F = G \frac{m_1 m_2}{r^2}
$$

Determine how the force changes if

- both masses are halved
- the distance is doubled.

---

## Theory

The gravitational force is proportional to

$
m_1 m_2
$

and inversely proportional to

$
r^2
$

Changes in variables therefore scale the force.

---

## Step-by-Step Solution

The modified masses are

$
m_1' = \frac{m_1}{2}
$

$
m_2' = \frac{m_2}{2}
$

The modified distance is

$
r' = 2r
$

Substitute into the law.

$$
F' =
G
\frac{(m_1/2)(m_2/2)}{(2r)^2}
$$

Simplify the numerator.

$$
F' =
G
\frac{m_1 m_2}{4}
\frac{1}{(2r)^2}
$$

Compute the denominator.

$$
(2r)^2 = 4r^2
$$

Thus

$$
F' =
G
\frac{m_1 m_2}{16 r^2}
$$

Compare with the original force

$$
F = G\frac{m_1 m_2}{r^2}
$$

Therefore

$$
F' = \frac{1}{16}F
$$

---

## Final Result

The gravitational force becomes

$
F' = \frac{F}{16}
$

---

## Interpretation

Halving both masses reduces the force by a factor of $4$, while doubling the distance reduces it by another factor of $4$.  
The combined effect is a reduction by a factor of **16**.

---

# Task 04 – Rearranging the Pendulum Formula

## Problem Statement

The period of a simple pendulum is

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

Rearrange the formula to obtain an expression for $g$.

---

## Theory

Solving equations often requires removing square roots by squaring both sides.

---

## Step-by-Step Solution

Start with

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

Square both sides.

$$
T^2 = 4\pi^2 \frac{L}{g}
$$

Multiply by $g$.

$$
gT^2 = 4\pi^2 L
$$

Solve for $g$.

$$
g = \frac{4\pi^2 L}{T^2}
$$

---

## Final Result

$$
g = \frac{4\pi^2 L}{T^2}
$$

---

## Interpretation

This expression allows the **gravitational acceleration** to be determined experimentally by measuring the pendulum length and oscillation period.

---

# Task 05 – Vector Components

## Problem Statement

A vector has magnitude $15$ and forms an angle of $60^\circ$ with the horizontal axis.

Determine the horizontal and vertical components.

---

## Theory

Vector components are obtained using trigonometry.

$$
A_x = A\cos\theta
$$

$$
A_y = A\sin\theta
$$

---

## Step-by-Step Solution

Horizontal component

$$
A_x = 15 \cos 60^\circ
$$

Since

$
\cos60^\circ = \frac12
$

$$
A_x = 7.5
$$

Vertical component

$$
A_y = 15\sin60^\circ
$$

Since

$
\sin60^\circ = \frac{\sqrt{3}}{2}
$

$$
A_y =
\frac{15\sqrt3}{2}
$$

---

## Final Result

$
A_x = 7.5
$

$
A_y = \frac{15\sqrt3}{2}
$

---

## Interpretation

The vertical component is larger than the horizontal component because the vector is oriented closer to the vertical direction.

---

# Task 06 – Function Analysis

## Problem Statement

Analyze the function

$
f(x) = 3x^2 - 12x + 7
$

and determine its local extrema.

---

## Theory

Extrema occur where

$$
f'(x) = 0
$$

A minimum occurs if

$
f''(x) > 0
$

---

## Step-by-Step Solution

First derivative

$$
f'(x) = 6x - 12
$$

Set derivative equal to zero.

$$
6x - 12 = 0
$$

$$
x = 2
$$

Second derivative

$$
f''(x) = 6
$$

Since this value is positive, the point corresponds to a **minimum**.

Evaluate the function.

$$
f(2) = 3(2)^2 - 12(2) + 7
$$

$$
= 12 - 24 + 7
$$

$$
= -5
$$

---

## Final Result

Minimum point

$
(2,-5)
$

---

## Interpretation

The quadratic function opens upward, meaning it possesses a single global minimum and no maximum.

---

# Task 07 – Fly and Bicycle Problem

## Problem Statement

A bicycle is $10$ m from a wall and moves toward it at $1$ m/s.

A fly starts at the bicycle and flies toward the wall at $2$ m/s, repeatedly bouncing between the wall and bicycle.

Determine the total distance traveled by the fly before the bicycle reaches the wall.

---

## Theory

Rather than summing infinitely many trips, the total travel time can be determined.

The fly travels continuously during this time.

---

## Step-by-Step Solution

The bicycle reaches the wall after

$$
t = \frac{d}{v}
$$

$$
t = \frac{10}{1}
$$

$$
t = 10
$$

seconds.

The fly travels at

$
2 \text{ m/s}
$

The total distance is

$$
d = vt
$$

$$
d = 2 \times 10
$$

$$
d = 20
$$

---

## Final Result

The fly travels

$
20 \text{ m}
$

---

## Interpretation

Although the fly performs infinitely many back-and-forth trips, the total time is finite.  
Therefore the total distance is also finite.

---

# Task 08 – Definite Integral

## Problem Statement

Evaluate the area under

$
f(x) = \sin x
$

between

$
x=0
$

and

$
x=\pi
$

---

## Theory

The area under a curve is computed using a definite integral.

---

## Step-by-Step Solution

$$
\int_0^\pi \sin x \, dx
$$

The antiderivative is

$$
-\cos x
$$

Evaluate at the limits.

$$
[-\cos x]_0^\pi
$$

$$
= -\cos\pi + \cos0
$$

Since

$
\cos\pi = -1
$

$
\cos0 = 1
$

$$
= 1 + 1
$$

$$
= 2
$$

---

## Final Result

The area equals

$
2
$

---

## Interpretation

Because $\sin x$ is positive over this interval, the integral represents the **true geometric area**.

---

# Task 09 – Optimization Problem

## Problem Statement

Find the rectangle of maximum area under the curve

$
y = 3 - x^2
$

in the first quadrant.

---

## Theory

Area must be expressed as a function of $x$, then maximized using derivatives.

---

## Step-by-Step Solution

Height of the rectangle

$$
y = 3 - x^2
$$

Area

$$
A = x(3 - x^2)
$$

$$
A = 3x - x^3
$$

Differentiate.

$$
A' = 3 - 3x^2
$$

Set equal to zero.

$$
3 - 3x^2 = 0
$$

$$
x = 1
$$

Compute height.

$$
y = 3 - 1
$$

$$
y = 2
$$

---

## Final Result

Maximum rectangle dimensions

Width

$
1
$

Height

$
2
$

---

## Interpretation

The optimal rectangle touches the parabola at its upper right corner and maximizes the enclosed area.

---

# Task 10 – Infinite Series Motion

## Problem Statement

An ant moves according to the pattern

- $1$ m east
- $1/2$ m north
- $1/3$ m west
- $1/4$ m south
- $1/5$ m east
- continuing indefinitely.

Determine the final position.

---

## Theory

The motion separates into horizontal and vertical series.

These correspond to alternating harmonic series.

---

## Step-by-Step Solution

Horizontal displacement

$$
1 - \frac13 + \frac15 - \frac17 + \dots
$$

This series equals

$$
\frac{\pi}{4}
$$

Vertical displacement

$$
\frac12 - \frac14 + \frac16 - \frac18 + \dots
$$

Factor out $1/2$.

$$
\frac12
\left(
1 - \frac12 + \frac13 - \frac14 + \dots
\right)
$$

The series in parentheses equals

$
\ln 2
$

Thus

$$
y = \frac{\ln 2}{2}
$$

---

## Final Result

Final position

$$
\left(
\frac{\pi}{4},
\frac{\ln2}{2}
\right)
$$

---

## Interpretation

Despite infinitely many steps, both alternating series converge.  
Therefore the ant approaches a **finite limiting position**.