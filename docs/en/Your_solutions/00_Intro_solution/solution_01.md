# Vector Algebra Calculations

This repository contains a step-by-step solution for common vector operations in 3D space using two given vectors:

$$\vec{a} = [2, 1, -3]$$
$$\vec{b} = [4, -2, 1]$$

---

## a) Magnitude of each vector

The magnitude (or length) of a vector $\vec{v} = [x, y, z]$ is calculated using the formula:
$$\|\vec{v}\| = \sqrt{x^2 + y^2 + z^2}$$



### Magnitude of $\vec{a}$:
$$\|\vec{a}\| = \sqrt{2^2 + 1^2 + (-3)^2}$$
$$\|\vec{a}\| = \sqrt{4 + 1 + 9} = \mathbf{\sqrt{14}} \approx 3.74$$

### Magnitude of $\vec{b}$:
$$\|\vec{b}\| = \sqrt{4^2 + (-2)^2 + 1^2}$$
$$\|\vec{b}\| = \sqrt{16 + 4 + 1} = \mathbf{\sqrt{21}} \approx 4.58$$

---

## b) Dot Product ($\vec{a} \cdot \vec{b}$)

The dot product is the sum of the products of the corresponding components:
$$\vec{a} \cdot \vec{b} = (a_x \cdot b_x) + (a_y \cdot b_y) + (a_z \cdot b_z)$$



**Calculation:**
$$\vec{a} \cdot \vec{b} = (2 \times 4) + (1 \times -2) + (-3 \times 1)$$
$$\vec{a} \cdot \vec{b} = 8 - 2 - 3$$
$$\vec{a} \cdot \vec{b} = \mathbf{3}$$

---

## c) Cross Product ($\vec{a} \times \vec{b}$)

The cross product is calculated using the determinant of a $3 \times 3$ matrix:

$$\vec{a} \times \vec{b} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 1 & -3 \\ 4 & -2 & 1 \end{vmatrix}$$



**Step-by-step expansion:**
* **i-component:** $(1 \times 1) - (-3 \times -2) = 1 - 6 = -5$
* **j-component:** $-[(2 \times 1) - (-3 \times 4)] = -(2 + 12) = -14$
* **k-component:** $(2 \times -2) - (1 \times 4) = -4 - 4 = -8$

**Result:**
$$\vec{a} \times \vec{b} = \mathbf{[-5, -14, -8]}$$

---

## d) Angle between vectors $\vec{a}$ and $\vec{b}$

We use the relationship between the dot product and the magnitudes:
$$\cos \theta = \frac{\vec{a} \cdot \vec{b}}{\|\vec{a}\| \|\vec{b}\|}$$



[Image of angle between two vectors in 3D]


**Calculation:**
$$\cos \theta = \frac{3}{\sqrt{14} \cdot \sqrt{21}}$$
$$\cos \theta = \frac{3}{\sqrt{294}} \approx 0.17496$$

**Final Result:**
* **Radians:** $\theta = \arccos(0.17496) \approx \mathbf{1.395 \text{ rad}}$
* **Degrees:** $\theta \approx \mathbf{79.92^\circ}$

---

## Summary Table

| Operation | Result |
| :--- | :--- |
| **Magnitude $\|\vec{a}\|$** | $\sqrt{14} \approx 3.74$ |
| **Magnitude $\|\vec{b}\|$** | $\sqrt{21} \approx 4.58$ |
| **Dot Product $\vec{a} \cdot \vec{b}$** | $3$ |
| **Cross Product $\vec{a} \times \vec{b}$** | $[-5, -14, -8]$ |
| **Angle $\theta$** | $79.92^\circ$ |

