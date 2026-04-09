<h1 style="color:#4fc3f7">Task 02 – String Harmonics</h1>

<h2 style="color:#81d4fa">Problem Statement</h2>

A guitar string has a length of $L = 64\ \text{cm} = 0.64\ \text{m}$ and vibrates at its fundamental frequency $f_1 = 330\ \text{Hz}$ (one antinode). Determine the speed of the wave on this string.

---

<h2 style="color:#81d4fa">Theory</h2>

A string fixed at both ends supports standing waves. The boundary conditions require a node at each end. For the $n$-th harmonic, the string accommodates $n$ half-wavelengths:

$$
L = n \frac{\lambda_n}{2}, \quad n = 1, 2, 3, \ldots
$$

For the **fundamental mode** ($n = 1$, one antinode):

$$
L = \frac{\lambda_1}{2}
$$

$$
\lambda_1 = 2L
$$

The wave speed on the string is then obtained from the fundamental relation:

$$
v = f_1 \lambda_1
$$

The wave speed on a string is a physical property of the string itself (dependent on tension and linear mass density), not of the frequency — the same $v$ applies to all harmonics.

---

<h2 style="color:#81d4fa">Step-by-Step Solution</h2>

<h3 style="color:#b3e5fc">Step 1 — Find the Fundamental Wavelength</h3>

$$
\lambda_1 = 2L = 2 \times 0.64\ \text{m} = 1.28\ \text{m}
$$

<h3 style="color:#b3e5fc">Step 2 — Find the Wave Speed</h3>

$$
v = f_1 \lambda_1 = 330\ \text{Hz} \times 1.28\ \text{m}
$$

$$
v = 422.4\ \text{m/s}
$$

---

<h2 style="color:#81d4fa">Final Result</h2>

$$
v = 422.4\ \text{m/s}
$$

---

<h2 style="color:#81d4fa">Interpretation</h2>

The wave speed of approximately 422 m/s is the transverse wave speed specific to this string under its operating tension. The fundamental mode has a single antinode at the midpoint of the string, with nodes at both fixed ends. Higher harmonics ($n = 2, 3, \ldots$) share the same wave speed but have shorter wavelengths and higher frequencies: $f_n = n f_1$.