## 6. Function Analysis

This document provides a step-by-step calculus-based analysis of the quadratic function $f(x) = 3x^2 - 12x + 7$ to identify its local extrema.

---

### 1. Theory and Formulas

**Local Extrema** (maxima or minima) occur at **critical points**, which are found where the first derivative of the function equals zero (or is undefined). 

Because this function is a parabola (a polynomial of degree 2), it will have exactly one global extremum, which also serves as its local extremum.

#### The First and Second Derivative Tests
1.  **First Derivative:** Find $f'(x)$ and set $f'(x) = 0$ to find the critical value $x_c$.
2.  **Second Derivative:** Find $f''(x)$ to determine concavity:
    * If $f''(x_c) > 0$, the curve is concave up, making the point a **local minimum**.
    * If $f''(x_c) < 0$, the curve is concave down, making the point a **local maximum**.

---

### 2. Step-by-Step Determination

**Given Function:**
$$f(x) = 3x^2 - 12x + 7$$

#### Step 1: Find the First Derivative
Using the power rule for derivatives:
$$f'(x) = \frac{d}{dx}(3x^2) - \frac{d}{dx}(12x) + \frac{d}{dx}(7)$$
$$f'(x) = 6x - 12$$

#### Step 2: Find the Critical Points
Set the first derivative to zero:
$$6x - 12 = 0$$
$$6x = 12$$
$$\mathbf{x = 2}$$

#### Step 3: Apply the Second Derivative Test
Differentiate $f'(x)$ to find the second derivative:
$$f''(x) = \frac{d}{dx}(6x - 12)$$
$$f''(x) = 6$$

Since $f''(2) = 6$, which is strictly greater than $0$, the function is **concave up** at $x = 2$. Therefore, this critical point is a **local minimum**.

#### Step 4: Find the Corresponding y-value
Substitute $x = 2$ back into the original function to find the minimum value:
$$f(2) = 3(2)^2 - 12(2) + 7$$
$$f(2) = 3(4) - 24 + 7$$
$$f(2) = 12 - 24 + 7$$
$$f(2) = \mathbf{-5}$$

---

### 3. Summary Table

| Property | Calculation / Value |
| :--- | :--- |
| **First Derivative $f'(x)$** | $6x - 12$ |
| **Second Derivative $f''(x)$** | $6$ |
| **Critical Point ($x$)** | $2$ |
| **Function Value $f(x)$** | $-5$ |
| **Extremum Type** | **Local Minimum** |

**Conclusion:** The function $f(x) = 3x^2 - 12x + 7$ has a single **local minimum** located at the coordinates **$(2, -5)$**. There are no local maxima.
