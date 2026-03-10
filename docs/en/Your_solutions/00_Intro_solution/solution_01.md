# Vector Algebra: Theory and Step-by-Step Solutions

This document explores the fundamental operations of vector algebra in $\mathbb{R}^3$ using two specific vectors:
$$\vec{a} = [2, 1, -3]$$
$$\vec{b} = [4, -2, 1]$$

---

## 1. Vector Magnitude (Norm)

### Theory
The **magnitude** (or Euclidean norm) represents the length of a vector from the origin to its terminal point. It is a scalar value derived from the Pythagorean theorem extended to three dimensions.

### Formula
For a vector $\vec{v} = [x, y, z]$:
$$\|\vec{v}\| = \sqrt{x^2 + y^2 + z^2}$$



### Determination
* **For $\vec{a}$:**
    $$\|\vec{a}\| = \sqrt{2^2 + 1^2 + (-3)^2} = \sqrt{4 + 1 + 9} = \mathbf{\sqrt{14}} \approx 3.74$$
* **For $\vec{b}$:**
    $$\|\vec{b}\| = \sqrt{4^2 + (-2)^2 + 1^2} = \sqrt{16 + 4 + 1} = \mathbf{\sqrt{21}} \approx 4.58$$

---

## 2. The Dot Product (Scalar Product)

### Theory
The **dot product** measures how much one vector aligns with another. Geometrically, it is the product of the magnitudes of the two vectors and the cosine of the angle between them. If the result is zero, the vectors are **orthogonal** (perpendicular).

### Formula
$$\vec{a} \cdot \vec{b} = (a_x b_x) + (a_y b_y) + (a_z b_z)$$



### Determination
$$\vec{a} \cdot \vec{b} = (2 \times 4) + (1 \times -2) + (-3 \times 1)$$
$$\vec{a} \cdot \vec{b} = 8 - 2 - 3 = \mathbf{3}$$

---

## 3. The Cross Product (Vector Product)

### Theory
Unlike the dot product, the **cross product** results in a new **vector**. This resulting vector is strictly perpendicular to the plane containing $\vec{a}$ and $\vec{b}$. Its direction is determined by the "Right-Hand Rule."

### Formula
The cross product is calculated using the determinant of a $3 \times 3$ matrix:
$$\vec{a} \times \vec{b} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ a_x & a_y & a_z \\ b_x & b_y & b_z \end{vmatrix}$$



[Image of right-hand rule for cross product]


### Determination
$$\vec{a} \times \vec{b} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 1 & -3 \\ 4 & -2 & 1 \end{vmatrix}$$

* **i-component:** $(1 \times 1) - (-3 \times -2) = 1 - 6 = -5$
* **j-component:** $-[(2 \times 1) - (-3 \times 4)] = -(2 + 12) = -14$
* **k-component:** $(2 \times -2) - (1 \times 4) = -4 - 4 = -8$

**Result:** $\vec{a} \times \vec{b} = \mathbf{[-5, -14, -8]}$

---

## 4. Angle Between Vectors

### Theory
The angle $\theta$ between two vectors can be extracted from the geometric definition of the dot product. It describes the angular separation between the two lines segmenting from the origin.

### Formula
$$\theta = \arccos \left( \frac{\vec{a} \cdot \vec{b}}{\|\vec{a}\| \|\vec{b}\|} \right)$$



### Determination
1.  **Calculate Cosine:** $\cos(\theta) = \frac{3}{\sqrt{14} \cdot \sqrt{21}} = \frac{3}{\sqrt{294}} \approx 0.17496$
2.  **Inverse Cosine:** $\theta = \arccos(0.17496)$
3.  **Results:**
    * **Radians:** $\approx \mathbf{1.395 \text{ rad}}$
    * **Degrees:** $\approx \mathbf{79.92^\circ}$

---

## Summary Table

| Property | Formula | Result |
| :--- | :--- | :--- |
| **Magnitude of $\vec{a}$** | $\sqrt{\sum v_i^2}$ | $\approx 3.74$ |
| **Magnitude of $\vec{b}$** | $\sqrt{\sum v_i^2}$ | $\approx 4.58$ |
| **Dot Product** | $\sum a_i b_i$ | $3$ |
| **Cross Product** | Determinant | $[-5, -14, -8]$ |
| **Angle $\theta$** | $\arccos(\frac{\text{dot}}{\text{mags}})$ | $79.92^\circ$ |
