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

It measures the projection of one vector onto another.

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

It produces a vector perpendicular to both $\vec{a}$ and $\vec{b}$.

---

## Step-by-Step Solution

### a) Magnitudes

For vector $\vec{a}$:

$$
|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}
$$

$$
|\vec{a}| = \sqrt{4 + 1 + 9}
$$

$$
|\vec{a}| = \sqrt{14}
$$

---

For vector $\vec{b}$:

$$
|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}
$$

$$
|\vec{b}| = \sqrt{16 + 4 + 1}
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
\vec{a} \cdot \vec{b} = 8 - 2 - 3
$$

$$
\vec{a} \cdot \vec{b} = 3
$$

---

### c) Cross Product

Start from the determinant:

$$
\vec{a} \times \vec{b} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & 1 & -3 \\
4 & -2 & 1
\end{vmatrix}
$$

Expand along the first row:

$$
\vec{a} \times \vec{b} =
\hat{i}
\begin{vmatrix}
1 & -3 \\
-2 & 1
\end{vmatrix}
-
\hat{j}
\begin{vmatrix}
2 & -3 \\
4 & 1
\end{vmatrix}
+
\hat{k}
\begin{vmatrix}
2 & 1 \\
4 & -2
\end{vmatrix}
$$

---

Compute each minor:

For $\hat{i}$ component:

$$
\begin{vmatrix}
1 & -3 \\
-2 & 1
\end{vmatrix}
= (1)(1) - (-3)(-2)
$$

$$
= 1 - 6 = -5
$$

---

For $\hat{j}$ component:

$$
\begin{vmatrix}
2 & -3 \\
4 & 1
\end{vmatrix}
= (2)(1) - (-3)(4)
$$

$$
= 2 + 12 = 14
$$

---

For $\hat{k}$ component:

$$
\begin{vmatrix}
2 & 1 \\
4 & -2
\end{vmatrix}
= (2)(-2) - (1)(4)
$$

$$
= -4 - 4 = -8
$$

---

Assemble the vector:

$$
\vec{a} \times \vec{b} = (-5)\hat{i} - (14)\hat{j} + (-8)\hat{k}
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

- The magnitudes describe the lengths of the vectors in three-dimensional space.  
- The positive dot product indicates that the angle between $\vec{a}$ and $\vec{b}$ is acute.  
- The cross product produces a vector perpendicular to both $\vec{a}$ and $\vec{b}$, following the right-hand rule. Its magnitude corresponds to the area of the parallelogram spanned by the two vectors.