<style>
h1, h2, h3, h4 {
    color: #007acc;
}
</style>

# Task 07 – Dynamics with Friction

## Problem Statement

A $5 \text{ kg}$ block is placed on a $10 \text{ kg}$ block. A horizontal force of $45 \text{ N}$ is applied to the $10 \text{ kg}$ block, and the $5 \text{ kg}$ block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is $0.2$. Find the acceleration of the $10 \text{ kg}$ block.

## Theory

To find the acceleration, we apply Newton's Second Law ($\sum F = ma$) to the moving block ($m_2 = 10 \text{ kg}$). We must identify all horizontal forces acting on it:
1.  **Applied Force ($F$):** $45 \text{ N}$ forward.
2.  **Friction from the ground ($f_g$):** Opposes motion. Depends on the total normal force ($m_1 + m_2)g$.
3.  **Friction from the top block ($f_t$):** Since the top block is held stationary by a wall, it slides relative to the bottom block, exerting a kinetic friction force backwards.

The formula for kinetic friction is $f = \mu N$.

## Step-by-Step Solution

### 1. Calculate Individual Friction Forces

Acceleration due to gravity $g = 9.81 \text{ m/s}^2$.

**Friction between the blocks ($f_t$):**
The normal force is the weight of the $5 \text{ kg}$ block.

$$
f_t = \mu m_1 g = 0.2 \times 5 \times 9.81 = 9.81 \text{ N}
$$

**Friction between the floor and $10 \text{ kg}$ block ($f_g$):**
The normal force is the total weight of both blocks.

$$
f_g = \mu (m_1 + m_2) g = 0.2 \times (5 + 10) \times 9.81
$$

$$
f_g = 0.2 \times 15 \times 9.81 = 29.43 \text{ N}
$$

### 2. Apply Newton's Second Law

The net force on the $10 \text{ kg}$ block is:

$$
F_{net} = F_{applied} - f_t - f_g
$$

$$
F_{net} = 45 - 9.81 - 29.43 = 5.76 \text{ N}
$$

### 3. Calculate Acceleration

$$
a = \frac{F_{net}}{m_2} = \frac{5.76}{10} = 0.576 \text{ m/s}^2
$$

## Final Result

The acceleration of the $10 \text{ kg}$ block is **$0.576 \text{ m/s}^2$**.

## Interpretation

Despite the $45 \text{ N}$ force, the acceleration is quite low because friction is acting on both the top and bottom surfaces of the moving block. The top block, being tied to the wall, acts as an additional "drag" on the system.