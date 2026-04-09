<h1 style="color:#4fc3f7">Task 06 – Wave Equation</h1>

<h2 style="color:#81d4fa">Problem Statement</h2>

A wave is described by:

$$
y(x, t) = 0.05 \sin(2\pi x - 50\pi t)
$$

where $x$ and $y$ are in metres and $t$ is in seconds. Determine:

- a) Amplitude $A$
- b) Wavelength $\lambda$
- c) Frequency $f$
- d) Wave speed $v$

---

<h2 style="color:#81d4fa">Theory</h2>

The standard form of a sinusoidal travelling wave is:

$$
y(x, t) = A \sin(kx - \omega t)
$$

where:

- $A$ — amplitude (maximum displacement from equilibrium)
- $k = \dfrac{2\pi}{\lambda}$ — wave number (spatial frequency, rad/m)
- $\omega = 2\pi f$ — angular frequency (rad/s)

From $k$ and $\omega$ one recovers:

$$
\lambda = \frac{2\pi}{k}, \qquad f = \frac{\omega}{2\pi}, \qquad v = \frac{\omega}{k} = f\lambda
$$

---

<h2 style="color:#81d4fa">Step-by-Step Solution</h2>

<h3 style="color:#b3e5fc">Identifying the Parameters</h3>

Comparing $y(x,t) = 0.05\sin(2\pi x - 50\pi t)$ with the standard form $A\sin(kx - \omega t)$:

$$
A = 0.05\ \text{m}, \qquad k = 2\pi\ \text{rad/m}, \qquad \omega = 50\pi\ \text{rad/s}
$$

<h3 style="color:#b3e5fc">a) Amplitude</h3>

$$
A = 0.05\ \text{m}
$$

<h3 style="color:#b3e5fc">b) Wavelength</h3>

$$
\lambda = \frac{2\pi}{k} = \frac{2\pi}{2\pi}
$$

$$
\lambda = 1\ \text{m}
$$

<h3 style="color:#b3e5fc">c) Frequency</h3>

$$
f = \frac{\omega}{2\pi} = \frac{50\pi}{2\pi}
$$

$$
f = 25\ \text{Hz}
$$

<h3 style="color:#b3e5fc">d) Wave Speed</h3>

$$
v = \frac{\omega}{k} = \frac{50\pi}{2\pi}
$$

$$
v = 25\ \text{m/s}
$$

Alternatively, using $v = f\lambda$:

$$
v = 25\ \text{Hz} \times 1\ \text{m} = 25\ \text{m/s}
$$

---

<h2 style="color:#81d4fa">Final Result</h2>

| Quantity | Symbol | Value |
|---|---|---|
| Amplitude | $A$ | $0.05\ \text{m}$ |
| Wavelength | $\lambda$ | $1\ \text{m}$ |
| Frequency | $f$ | $25\ \text{Hz}$ |
| Wave speed | $v$ | $25\ \text{m/s}$ |

---

<h2 style="color:#81d4fa">Interpretation</h2>

The wave oscillates with a small amplitude of 5 cm, travels in the positive $x$-direction (negative sign between $kx$ and $\omega t$), and completes 25 full cycles per second. A wavelength of 1 m means the spatial pattern repeats every metre. The wave speed of 25 m/s is consistent with $v = f\lambda = 25 \times 1$.