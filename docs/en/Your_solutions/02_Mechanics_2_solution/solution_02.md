### 2. Harmonic Motion


### Fundamental Theory

The equation provided for the position of the mass is a standard Simple Harmonic Motion (SHM) equation:
$$x(t) = A \cos(\omega t + \phi)$$

By comparing your specific equation, $x(t) = 0.2 \cos(10\pi t)$, to the standard form, we can extract the key parameters of the system:
* **Amplitude ($A$):** The maximum displacement from equilibrium is **0.2 m**.
* **Angular Frequency ($\omega$):** The rate of oscillation is **$10\pi$ rad/s**.
* **Phase Angle ($\phi$):** In this case, it is **0**.



---

### Part 1: Finding the Spring Constant ($k$)

**1. State the relevant formula:**
The angular frequency ($\omega$) of a mass-spring system is determined by the spring constant ($k$) and the mass ($m$) attached to it:
$$\omega = \sqrt{\frac{k}{m}}$$

**2. Rearrange the formula to solve for $k$:**
Square both sides to remove the square root:
$$\omega^2 = \frac{k}{m}$$
Multiply by $m$:
$$k = m\omega^2$$

**3. Substitute the known values and calculate:**
We know $m =$ **10 kg** and $\omega =$ **$10\pi$ rad/s**.
$$k = 10 \cdot (10\pi)^2$$
$$k = 10 \cdot 100\pi^2$$
$$k = 1000\pi^2 \text{ N/m}$$

If we use the approximation $\pi \approx 3.14159$ (so $\pi^2 \approx 9.8696$):
$$k \approx 1000 \cdot 9.8696$$
$$k \approx 9869.6 \text{ N/m}$$

**Answer:** The spring constant $k$ is exactly **$1000\pi^2$ N/m**, or approximately **9869.6 N/m**.

---

### Part 2: Finding the Total Mechanical Energy ($E$)

**1. State the relevant formula:**
In an ideal simple harmonic oscillator (with no friction), the total mechanical energy is conserved. It is equal to the maximum potential energy stored in the spring when it is fully stretched or compressed to its amplitude ($A$).
$$E = \frac{1}{2}kA^2$$

**2. Substitute the known values and calculate:**
We now know $k = 1000\pi^2 \text{ N/m}$ and the given amplitude is $A = $ **0.2 m**.
$$E = \frac{1}{2} \cdot (1000\pi^2) \cdot (0.2)^2$$
$$E = 500\pi^2 \cdot 0.04$$
$$E = 20\pi^2 \text{ Joules}$$

Using the exact same approximation for $\pi^2$:
$$E \approx 20 \cdot 9.8696$$
$$E \approx 197.39 \text{ Joules}$$

**Answer:** The total mechanical energy of the system is exactly **$20\pi^2$ J**, or approximately **197.4 J**.

---
