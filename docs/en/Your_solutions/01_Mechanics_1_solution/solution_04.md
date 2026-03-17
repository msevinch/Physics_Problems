## 4. Vector Calculus

This document provides a step-by-step derivation of velocity and acceleration vectors from a time-dependent position function in 2D space.

---

### 1. Theory

In vector calculus, the motion of a particle is described by a **position vector** $\vec{r}(t)$. To find how the particle moves over time, we use differentiation:

* **Velocity ($\vec{v}$)** is the first derivative of position with respect to time. It represents the instantaneous rate of change of the particle's displacement.
* **Acceleration ($\vec{a}$)** is the second derivative of position (or the first derivative of velocity). It represents how the velocity changes over time.



---

### 2. Formulas

For a position vector defined in terms of its components $\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j}$:

1.  **Velocity Formula:**
    $$\vec{v}(t) = \frac{d\vec{r}}{dt} = \frac{dx}{dt}\hat{i} + \frac{dy}{dt}\hat{j}$$

2.  **Acceleration Formula:**
    $$\vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{d^2x}{dt^2}\hat{i} + \frac{d^2y}{dt^2}\hat{j}$$

3.  **Power Rule for Differentiation:**
    $$\frac{d}{dt}(t^n) = nt^{n-1}$$

---

### 3. Determination

**Given Position Vector:**
$$\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$$

#### Step 1: Find the Velocity Vector $\vec{v}(t)$
We differentiate the $x$ and $y$ components individually:
* **$x$-component:** $\frac{d}{dt}(3t^2) = 2 \cdot 3t^{2-1} = 6t$
* **$y$-component:** $\frac{d}{dt}(5t - 8t^2) = 5 - 16t$

**Result:**
$$\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$$

#### Step 2: Find the Acceleration Vector $\vec{a}(t)$
We differentiate the velocity components found in Step 1:
* **$x$-component:** $\frac{d}{dt}(6t) = 6$
* **$y$-component:** $\frac{d}{dt}(5 - 16t) = -16$

**Result:**
$$\vec{a}(t) = 6\hat{i} - 16\hat{j}$$

---

### 4. Summary Table

| Property | Symbol | Formula | Resulting Vector |
| :--- | :--- | :--- | :--- |
| **Position** | $\vec{r}(t)$ | Given | $(3t^2)\hat{i} + (5t - 8t^2)\hat{j}$ |
| **Velocity** | $\vec{v}(t)$ | $\frac{d\vec{r}}{dt}$ | $(6t)\hat{i} + (5 - 16t)\hat{j}$ |
| **Acceleration** | $\vec{a}(t)$ | $\frac{d\vec{v}}{dt}$ | $6\hat{i} - 16\hat{j}$ |

**Note:** The acceleration is constant in this case, meaning the object experiences a steady force in both the $x$ and $y$ directions.
