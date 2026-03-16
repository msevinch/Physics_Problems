## 10. Infinite Series

This document analyzes the convergent path of an ant moving in a repeating pattern of orthogonal steps, eventually stabilizing at a specific point in the 2D plane.

---

### 1. Theory and Concepts

**Separation of Components**
In a 2D coordinate system, horizontal (East/West) and vertical (North/South) movements are independent. To find the final position, we treat the $x$-coordinates and $y$-coordinates as two separate infinite series.

**Convergent Alternating Series**
The ant's steps get progressively smaller ($1, 1/2, 1/3, \dots$). Because the direction alternates (East then West, North then South), these form **Alternating Series**. According to the Alternating Series Test, if the terms decrease toward zero, the sum converges to a specific finite value.



---

### 2. Formulas

To solve this, we rely on two famous Taylor series expansions:

1.  **Gregory-Leibniz Series for $\pi$:**
    $$\arctan(x) = x - \frac{x^3}{3} + \frac{x^5}{5} - \frac{x^7}{7} + \dots$$
    When $x=1$, $\arctan(1) = \frac{\pi}{4}$.

2.  **Mercator Series for Natural Logarithms:**
    $$\ln(1+x) = x - \frac{x^2}{2} + \frac{x^3}{3} - \frac{x^4}{4} + \dots$$
    When $x=1$, $\ln(2) = 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \dots$

---

### 3. Step-by-Step Determination

The ant starts at $(0, 0)$. Let's track the movement:

#### Step 1: Horizontal Position ($x$)
The ant moves 1m East ($+$), 1/3m West ($-$), 1/5m East ($+$), and so on.
$$x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots$$
Matching this to the formula for $\arctan(1)$:
$$\mathbf{x = \frac{\pi}{4}} \approx 0.7854 \text{ m}$$

#### Step 2: Vertical Position ($y$)
The ant moves 1/2m North ($+$), 1/4m South ($-$), 1/6m North ($+$), and so on.
$$y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \dots$$
To solve this, we factor out $1/2$ from the series:
$$y = \frac{1}{2} \left( 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \dots \right)$$
Using the $\ln(2)$ identity:
$$\mathbf{y = \frac{1}{2} \ln 2} \approx 0.3466 \text{ m}$$

---

### 4. Summary Table

| Direction | Movement Pattern | Mathematical Identity | Final Coordinate |
| :--- | :--- | :--- | :--- |
| **Horizontal ($x$)** | $1 - 1/3 + 1/5 \dots$ | $\arctan(1)$ | $\frac{\pi}{4}$ |
| **Vertical ($y$)** | $1/2 - 1/4 + 1/6 \dots$ | $\frac{1}{2} \ln 2$ | $\frac{1}{2} \ln 2$ |

**Final Position:**
$$\boxed{\left( \frac{\pi}{4}, \frac{1}{2} \ln 2 \right)}$$
