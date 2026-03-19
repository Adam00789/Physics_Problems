# Task 07 – Logic and Series (Fly and Bicycle Problem)

## Problem Statement

A bicycle is $10 \text{ m}$ from a wall and moves toward it at a constant speed of $1 \text{ m/s}$.  

A fly starts from the bicycle and flies toward the wall at $2 \text{ m/s}$. Each time it reaches either the wall or the bicycle, it instantly turns around.

Determine the total distance traveled by the fly before the bicycle reaches the wall.

---

## Theory

This problem can be approached in two ways:

- by summing an infinite series of back-and-forth trips  
- by using total time and constant speed  

The second method is more efficient.

Distance is given by:

$$
d = v t
$$

---

## Step-by-Step Solution

### Step 1: Time until collision

The bicycle moves toward the wall with speed:

$$
v_{\text{bike}} = 1 \text{ m/s}
$$

Initial distance:

$$
d = 10 \text{ m}
$$

Time to reach the wall:

$$
t = \frac{d}{v}
$$

$$
t = \frac{10}{1}
$$

$$
t = 10 \text{ s}
$$

---

### Step 2: Distance traveled by the fly

The fly moves continuously at:

$$
v_{\text{fly}} = 2 \text{ m/s}
$$

Total time of motion:

$$
t = 10 \text{ s}
$$

Distance traveled:

$$
d_{\text{fly}} = v_{\text{fly}} \cdot t
$$

$$
d_{\text{fly}} = 2 \cdot 10
$$

$$
d_{\text{fly}} = 20 \text{ m}
$$

---

## Final Result

$$
d_{\text{fly}} = 20 \text{ m}
$$

---

## Interpretation

- Although the fly makes infinitely many trips, the total time is finite.  
- The motion reduces to a simple constant-speed problem.  
- The total distance depends only on the fly's speed and the time before the bicycle reaches the wall.  
- This is a classic example where an infinite process yields a finite result.