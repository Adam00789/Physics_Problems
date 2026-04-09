<h1 style="color:#4fc3f7">Task 04 – Phase Difference</h1>

<h2 style="color:#81d4fa">Problem Statement</h2>

Two points on a wave are separated by a distance $\Delta x = \lambda/3$. Determine the phase difference $\Delta \phi$ between them in radians.

---

<h2 style="color:#81d4fa">Theory</h2>

A travelling wave can be written as:

$$
y(x, t) = A \sin(kx - \omega t + \phi_0)
$$

where $k = \dfrac{2\pi}{\lambda}$ is the wave number. The **phase** at position $x$ and time $t$ is:

$$
\phi(x, t) = kx - \omega t + \phi_0
$$

The phase difference between two points at positions $x_1$ and $x_2$ (at the same instant $t$) is:

$$
\Delta \phi = \phi(x_2, t) - \phi(x_1, t) = k \Delta x = \frac{2\pi}{\lambda} \Delta x
$$

This result is general: a spatial separation $\Delta x$ corresponds to a phase difference proportional to the fraction of the wavelength covered.

---

<h2 style="color:#81d4fa">Step-by-Step Solution</h2>

<h3 style="color:#b3e5fc">Step 1 — Write the Phase Difference Formula</h3>

$$
\Delta \phi = \frac{2\pi}{\lambda} \Delta x
$$

<h3 style="color:#b3e5fc">Step 2 — Substitute $\Delta x = \lambda / 3$</h3>

$$
\Delta \phi = \frac{2\pi}{\lambda} \cdot \frac{\lambda}{3}
$$

$$
\Delta \phi = \frac{2\pi}{3}
$$

---

<h2 style="color:#81d4fa">Final Result</h2>

$$
\Delta \phi = \frac{2\pi}{3}\ \text{rad} \approx 2.094\ \text{rad} \approx 120°
$$

---

<h2 style="color:#81d4fa">Interpretation</h2>

A spatial separation of one-third of a wavelength corresponds to a phase difference of $120°$. This can be understood geometrically: one full wavelength corresponds to a complete cycle of $2\pi$ radians, so one-third of that distance yields one-third of $2\pi$. As a reference: a separation of $\lambda/2$ gives $\Delta\phi = \pi$ (the two points are always exactly out of phase), and $\lambda$ gives $\Delta\phi = 2\pi$ (the points are always in phase).