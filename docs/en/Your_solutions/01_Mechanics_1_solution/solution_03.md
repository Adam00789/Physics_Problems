# Task 03 – Path Intersection

## Problem Statement

Determine whether the paths

$$
A(t) = (2+t, 8-3t), \quad B(t) = (2t-1, 2t+2)
$$

intersect. If yes, find when and where.

---

## Theory

Two paths intersect if there exist parameters $t_1$ and $t_2$ such that:

$$
A(t_1) = B(t_2)
$$

---

## Step-by-Step Solution

Equate coordinates:

$$
2 + t_1 = 2t_2 - 1
$$

$$
8 - 3t_1 = 2t_2 + 2
$$

Solve first equation:

$$
t_1 = 2t_2 - 3
$$

Substitute:

$$
8 - 3(2t_2 - 3) = 2t_2 + 2
$$

$$
8 - 6t_2 + 9 = 2t_2 + 2
$$

$$
17 - 6t_2 = 2t_2 + 2
$$

$$
15 = 8t_2
$$

$$
t_2 = \frac{15}{8}
$$

$$
t_1 = \frac{15}{4} - 3 = \frac{3}{4}
$$

Position:

$$
x = 2 + \frac{3}{4} = \frac{11}{4}, \quad y = 8 - \frac{9}{4} = \frac{23}{4}
$$

---

## Final Result

Intersection occurs at:

$$
\left(\frac{11}{4}, \frac{23}{4}\right)
$$

---

## Interpretation

The two paths intersect at different parameter times, meaning the objects pass through the same point but do not collide.