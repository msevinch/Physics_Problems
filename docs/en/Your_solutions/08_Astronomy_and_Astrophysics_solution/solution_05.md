```python
G = 6.67430e-11
M_M = 7.35e22
R_M = 1737 * 1000  # in meters

v_esc_M = (2 * G * M_M / R_M) ** 0.5
v_esc_M_kms = v_esc_M / 1000

v_esc_E_kms = 11.2
fraction = v_esc_M_kms / v_esc_E_kms

print(f"v_esc_M: {v_esc_M} m/s")
print(f"v_esc_M_kms: {v_esc_M_kms} km/s")
print(f"fraction: {fraction}")



```

```text
v_esc_M: 2376.6302467735914 m/s
v_esc_M_kms: 2.3766302467735914 km/s
fraction: 0.21219912917621353


```


---

## Theory: What is Escape Velocity?

**Escape velocity** is the minimum speed an unpropelled object needs to escape from the gravitational influence of a primary body (like a planet or moon) and achieve an infinite distance from it without further acceleration.

This concept is derived from the **principle of conservation of mechanical energy**. For an object to just barely escape a gravitational field, its total mechanical energy (Kinetic Energy + Gravitational Potential Energy) at an infinite distance must equal zero.

Mathematically, at the surface of the celestial body:

$$E_{\text{total}} = K + U = 0$$

$$\frac{1}{2}mv_{\text{esc}}^2 - \frac{GMm}{R} = 0$$

Solving for the escape velocity ($v_{\text{esc}}$) gives the standard formula:

$$v_{\text{esc}} = \sqrt{\frac{2GM}{R}}$$

Where:

* $G$ is the universal gravitational constant ($\approx 6.6743 \times 10^{-11} \text{ m}^3\text{kg}^{-1}\text{s}^{-2}$).
* $M$ is the mass of the celestial body.
* $R$ is the radius of the celestial body.
* $m$ is the mass of the escaping object (which cancels out, meaning escape velocity depends only on the host body).

---

## Determine: Step-by-Step Calculation

### Step 1: Identify Given Values and Constants

* **Moon's Mass ($M_M$):** $7.35 \times 10^{22} \text{ kg}$
* **Moon's Radius ($R_M$):** $1,737 \text{ km}$
* **Earth's Escape Velocity ($v_E$):** $11.2 \text{ km/s}$
* **Gravitational Constant ($G$):** $6.6743 \times 10^{-11} \text{ m}^3\text{kg}^{-1}\text{s}^{-2}$

### Step 2: Convert Units to SI (Meters)

To keep units consistent with the gravitational constant, convert the Moon's radius from kilometers to meters:


$$R_M = 1,737 \text{ km} \times 1,000 \text{ m/km} = 1.737 \times 10^6 \text{ m}$$

### Step 3: Calculate the Escape Velocity in m/s

Substitute the values into the theoretical formula:

$$v_{\text{esc}} = \sqrt{\frac{2 \times (6.6743 \times 10^{-11}) \times (7.35 \times 10^{22})}{1.737 \times 10^6}}$$

First, calculate the numerator:


$$2 \times 6.6743 \times 10^{-11} \times 7.35 \times 10^{22} = 9.811221 \times 10^{12}$$

Next, divide by the radius:


$$\frac{9.811221 \times 10^{12}}{1.737 \times 10^6} \approx 5,648,371.33 \text{ m}^2/\text{s}^2$$

Now, take the square root:


$$v_{\text{esc}} = \sqrt{5,648,371.33} \approx 2,376.63 \text{ m/s}$$

### Step 4: Convert the Result to km/s

Divide the metric velocity by 1,000 to convert meters to kilometers:


$$v_{\text{esc}} = \frac{2,376.63 \text{ m/s}}{1,000} \approx \mathbf{2.38 \text{ km/s}}$$

### Step 5: Express as a Fraction of Earth's Escape Velocity

To find the ratio, divide the Moon's escape velocity by the Earth's given escape velocity ($11.2 \text{ km/s}$):

$$\text{Fraction} = \frac{v_{\text{Moon}}}{v_{\text{Earth}}} = \frac{2.377 \text{ km/s}}{11.2 \text{ km/s}} \approx 0.2122$$

As a simplified fraction, $0.2122$ is approximately **$\frac{1}{4.7}$** (or about **$21.2\%$** of Earth's escape velocity).

---

## Final Results Comparison

| Parameter | Value |
| --- | --- |
| **Moon's Escape Velocity** | **$2.38 \text{ km/s}$** ($2,377 \text{ m/s}$) |
| **Fraction of Earth's Escape Velocity** | **$0.212$** (approx. $\frac{1}{4.7}$ or $21.2\%$) |
