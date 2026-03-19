# Problem Set 01 – Solutions

---

# Task 01 – Vector Algebra

## Problem Statement

Given the vectors

$$
\vec{a} = [2, 1, -3], \qquad \vec{b} = [4, -2, 1]
$$

Compute:

- magnitudes of the vectors  
- dot product  
- cross product  

---

## Theory

### Magnitude of a Vector

For a vector in three dimensions:

$$
|\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}
$$

---

### Dot Product

The scalar (dot) product is defined as:

$$
\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z
$$

---

### Cross Product

The vector (cross) product is defined via a determinant:

$$
\vec{a} \times \vec{b} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
a_x & a_y & a_z \\
b_x & b_y & b_z
\end{vmatrix}
$$

---

## Step-by-Step Solution

### a) Magnitudes

$$
|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}
$$

$$
|\vec{a}| = \sqrt{14}
$$

---

$$
|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}
$$

$$
|\vec{b}| = \sqrt{21}
$$

---

### b) Dot Product

$$
\vec{a} \cdot \vec{b} = 2 \cdot 4 + 1 \cdot (-2) + (-3) \cdot 1
$$

$$
\vec{a} \cdot \vec{b} = 3
$$

---

### c) Cross Product

$$
\vec{a} \times \vec{b} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & 1 & -3 \\
4 & -2 & 1
\end{vmatrix}
$$

$$
\vec{a} \times \vec{b} = [-5, -14, -8]
$$

---

## Final Result

$$
|\vec{a}| = \sqrt{14}, \qquad |\vec{b}| = \sqrt{21}
$$

$$
\vec{a} \cdot \vec{b} = 3
$$

$$
\vec{a} \times \vec{b} = [-5, -14, -8]
$$

---

## Interpretation

- The magnitudes represent vector lengths.  
- The dot product indicates an acute angle between vectors.  
- The cross product is perpendicular to both vectors.

---

# Task 02 – Systems of Equations

## Problem Statement

Find the values of $x$ and $y$ that satisfy the system:

$$
2x + 3y = 12
$$

$$
x - y = 1
$$

---

## Theory

A system of linear equations can be solved using substitution or elimination.

For two equations:

$$
\begin{cases}
ax + by = c \\
dx + ey = f
\end{cases}
$$

One variable is expressed in terms of the other and substituted into the second equation.

---

## Step-by-Step Solution

From the second equation:

$$
x - y = 1
$$

Solve for $x$:

$$
x = 1 + y
$$

---

Substitute into the first equation:

$$
2x + 3y = 12
$$

$$
2(1 + y) + 3y = 12
$$

---

Expand:

$$
2 + 2y + 3y = 12
$$

$$
2 + 5y = 12
$$

---

Solve for $y$:

$$
5y = 10
$$

$$
y = 2
$$

---

Substitute back to find $x$:

$$
x = 1 + y
$$

$$
x = 1 + 2
$$

$$
x = 3
$$

---

## Final Result

$$
x = 3, \qquad y = 2
$$

---

## Interpretation

The solution $(x, y) = (3, 2)$ represents the intersection point of the two lines in the plane. This point satisfies both equations simultaneously, indicating a unique solution to the system.