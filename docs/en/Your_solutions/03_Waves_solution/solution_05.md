<h1 style="color:#4fc3f7">Task 05 – Echo Ranging</h1>

<h2 style="color:#81d4fa">Problem Statement</h2>

A person shouts toward a cliff and hears the echo $t = 1\ \text{s}$ later. The speed of sound in air is $v = 343\ \text{m/s}$. Determine the distance to the cliff.

---

<h2 style="color:#81d4fa">Theory</h2>

Sound travels from the person to the cliff and back — a total distance of twice the distance $d$ to the cliff. Since the speed of sound is constant, the total distance covered equals:

$$
d_\text{total} = v \cdot t
$$

The distance to the cliff is half of this:

$$
d = \frac{v \cdot t}{2}
$$

This principle is the basis of **echo ranging** (sonar, radar, and ultrasound imaging all rely on the same two-way travel-time concept).

---

<h2 style="color:#81d4fa">Step-by-Step Solution</h2>

<h3 style="color:#b3e5fc">Step 1 — Total Distance Travelled by the Sound</h3>

$$
d_\text{total} = v \cdot t = 343\ \text{m/s} \times 1\ \text{s} = 343\ \text{m}
$$

<h3 style="color:#b3e5fc">Step 2 — Distance to the Cliff</h3>

The sound covers the distance $d$ twice (outward and return), so:

$$
d = \frac{d_\text{total}}{2} = \frac{343}{2}\ \text{m}
$$

$$
d = 171.5\ \text{m}
$$

---

<h2 style="color:#81d4fa">Final Result</h2>

$$
d = 171.5\ \text{m}
$$

---

<h2 style="color:#81d4fa">Interpretation</h2>

The cliff is approximately 171.5 m away. A common error is to equate the full travel time directly to a single one-way journey — the factor of 2 is essential because the echo must return to the observer. For every additional second of echo delay, the cliff would be a further 171.5 m away. This two-way travel-time method is widely used in sonar (underwater ranging), radar (object detection), and medical ultrasonography.