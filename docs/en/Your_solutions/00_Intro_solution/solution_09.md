# Task 09 – Optimization of a Rectangle Under a Curve

## Problem Statement

A rectangle is inscribed under the curve $y = 3 - x^2$ in the first quadrant. Determine the dimensions of the rectangle that maximize its area.

---

## Theory

For optimization problems, the general procedure is:

1. Express the quantity to be maximized (area) as a function of a single variable.
2. Compute the derivative of this function.
3. Find critical points by solving $A'(x) = 0$.
4. Determine which point gives the maximum value.

The area of a rectangle is

$$
A = \text{width} \cdot \text{height}
$$

---

## Step-by-Step Solution

### Geometry of the Rectangle

The rectangle lies under the curve $y = 3 - x^2$ in the first quadrant.

- The top-right corner of the rectangle lies on the curve.
- Let this point be $(x, y)$.
- Then the height is

$$
y = 3 - x^2
$$

- The rectangle extends symmetrically from $-x$ to $x$, so the width is

$$
\text{width} = 2x
$$

---

### Area Function

The area as a function of $x$ is

$$
A(x) = 2x(3 - x^2)
$$

Expand:

$$
A(x) = 6x - 2x^3
$$

---

### First Derivative

Differentiate with respect to $x$:

$$
A'(x) = 6 - 6x^2
$$

---

### Critical Points

Set the derivative equal to zero:

$$
6 - 6x^2 = 0
$$

$$
6x^2 = 6
$$

$$
x^2 = 1
$$

$$
x = 1
$$

(Only the positive solution is valid in the first quadrant.)

---

### Dimensions

Height:

$$
y = 3 - x^2 = 3 - 1 = 2
$$

Width:

$$
\text{width} = 2x = 2
$$

---

## Final Result

The rectangle with maximum area has dimensions:

- Width: $2$
- Height: $2$

---

## Interpretation

The optimal rectangle is centered symmetrically about the $y$-axis and touches the curve at $(1, 2)$.

At this point, any increase in width reduces height too much, and any decrease in width reduces the total area, making this configuration the maximum-area solution.