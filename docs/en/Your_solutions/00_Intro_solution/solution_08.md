## 8. Definite Integrals

This document provides a step-by-step calculation to find the area under a trigonometric curve using the principles of integral calculus.

---

### 1. Theory and Formulas

**The Definite Integral** is a fundamental tool in calculus used to calculate the exact area under a curve $f(x)$ between two points $a$ and $b$. Geometrically, it sums up an infinite number of infinitesimally thin rectangles under the function's graph.



#### The Fundamental Theorem of Calculus
To evaluate a definite integral, we find the antiderivative (indefinite integral) of the function and calculate the difference between its values at the upper and lower limits:
$$\int_a^b f(x) \, dx = F(b) - F(a)$$
Where $F(x)$ is the antiderivative of $f(x)$.

---

### 2. Step-by-Step Determination

**Given Problem:**
Calculate the area under $f(x) = \sin(x)$ from $x = 0$ to $x = \pi$.

#### Step 1: Set up the Integral
$$\text{Area} = \int_{0}^{\pi} \sin(x) \, dx$$

#### Step 2: Find the Antiderivative
The antiderivative of $\sin(x)$ is $-\cos(x)$ (since the derivative of $\cos(x)$ is $-\sin(x)$).
$$F(x) = -\cos(x)$$

#### Step 3: Apply the Limits of Integration
Substitute the upper limit ($\pi$) and the lower limit ($0$) into the antiderivative:
$$\text{Area} = [-\cos(x)]_{0}^{\pi}$$
$$\text{Area} = (-\cos(\pi)) - (-\cos(0))$$

#### Step 4: Evaluate Trigonometric Values
Using the unit circle values:
* $\cos(\pi) = -1$
* $\cos(0) = 1$

Substitute these values back into the equation:
$$\text{Area} = (-(-1)) - (-(1))$$
$$\text{Area} = 1 + 1$$
$$\mathbf{\text{Area} = 2}$$

---

### 3. Summary Table

| Property | Symbol / Value |
| :--- | :--- |
| **Function** | $f(x) = \sin(x)$ |
| **Antiderivative** | $F(x) = -\cos(x)$ |
| **Lower Limit ($a$)** | $0$ |
| **Upper Limit ($b$)** | $\pi$ |
| **Calculated Area** | **$2$** |

**Conclusion:** The total area under the curve of $\sin(x)$ on the interval $[0, \pi]$ is exactly **2 square units**.
