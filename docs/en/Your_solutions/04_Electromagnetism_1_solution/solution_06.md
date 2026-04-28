
---

### 1. General Field Vector $\vec{E}(x, y)$
Let $q_1 = +q$ be at $\vec{r}_1 = (-a, 0)$ and $q_2 = +2q$ be at $\vec{r}_2 = (a, 0)$. For a general point $P(x, y)$:
* **Distance from $q_1$:** $r_1 = \sqrt{(x+a)^2 + y^2}$
* **Distance from $q_2$:** $r_2 = \sqrt{(x-a)^2 + y^2}$

The general electric field vector is:

$$\vec{E}(x, y) = k q \left[ \frac{(x+a)\hat{i} + y\hat{j}}{((x+a)^2 + y^2)^{3/2}} \right] + k(2q) \left[ \frac{(x-a)\hat{i} + y\hat{j}}{((x-a)^2 + y^2)^{3/2}} \right]$$

---

### 2. Specific Field Vectors
#### **A. Along the y-axis: $\vec{E}(0, y)$**
Set $x = 0$. Note that $r_1 = r_2 = \sqrt{a^2 + y^2}$.
* $E_x = \frac{kq(a)}{(a^2+y^2)^{3/2}} + \frac{k(2q)(-a)}{(a^2+y^2)^{3/2}} = \frac{-kqa}{(a^2+y^2)^{3/2}}$
* $E_y = \frac{kq(y)}{(a^2+y^2)^{3/2}} + \frac{k(2q)(y)}{(a^2+y^2)^{3/2}} = \frac{3kqy}{(a^2+y^2)^{3/2}}$

$$\vec{E}(0, y) = \frac{kq}{(a^2+y^2)^{3/2}} \left[ -a\hat{i} + 3y\hat{j} \right]$$

#### **B. Along the x-axis: $\vec{E}(x, 0)$**
Set $y = 0$. The field only has an x-component ($E_y = 0$).

$$\vec{E}(x, 0) = kq \left[ \frac{\text{sgn}(x+a)}{(x+a)^2} + \frac{2 \cdot \text{sgn}(x-a)}{(x-a)^2} \right] \hat{i}$$

*(Where $\text{sgn}$ denotes the sign of the displacement to ensure the force is always repulsive).*

---

### 3. Conditions for Zero Components and Zero Field
* **$E_y = 0$:** Generally occurs whenever **$y = 0$** (on the x-axis), as the charges are located on the x-axis and their vertical components naturally cancel or don't exist.
* **$E_x = 0$:** On the y-axis ($x=0$), $E_x$ is never zero unless $q$ or $a$ is zero. In the general plane, this requires the horizontal "pushes" to balance.
* **$\vec{E} = 0$ (Zero Field Point):** This must occur on the line between the charges ($y=0$ and $-a < x < a$).

  $$\frac{kq}{(x+a)^2} = \frac{k(2q)}{(a-x)^2} \implies \frac{1}{(x+a)^2} = \frac{2}{(a-x)^2}$$

     Taking the square root:

   $$\frac{1}{x+a} = \frac{\sqrt{2}}{a-x} \implies a - x = \sqrt{2}x + \sqrt{2}a$$

   $$x(1+\sqrt{2}) = a(1-\sqrt{2}) \implies x = a\frac{1-\sqrt{2}}{1+\sqrt{2}} \approx -0.1716a$$

---

### 4. Numerical Calculation
**Given:** $a=0.2\text{ m}, y=0.3\text{ m}, q=2\mu\text{C}$ (at point $x=0$).
1.  **Calculate $r$:** $\sqrt{0.2^2 + 0.3^2} = \sqrt{0.13} \approx 0.3606\text{ m}$.
2.  **Calculate $k q$:** $(8.99 \times 10^9) \times (2 \times 10^{-6}) = 17980$.
3.  **Find $E_x$:**

    $$E_x = \frac{-17980 \times 0.2}{(0.13)^{3/2}} \approx \frac{-3596}{0.04687} \approx -76,723 \text{ N/C}$$

5.  **Find $E_y$:**

     $$E_y = \frac{3 \times 17980 \times 0.3}{(0.13)^{3/2}} \approx \frac{16182}{0.04687} \approx 345,253 \text{ N/C}$$
    
**Result:** $\vec{E} \approx (-7.67 \times 10^4 \hat{i} + 3.45 \times 10^5 \hat{j}) \text{ N/C}$.

---

### 5. Limit Investigation ($y \gg a$)
When the observation point is very far away compared to the separation of the charges:
* The term $(a^2 + y^2) \approx y^2$.
* $E_x \approx \frac{-kqa}{y^3} \to 0$ (The x-component vanishes faster).
* $E_y \approx \frac{3kqy}{(y^2)^{3/2}} = \frac{3kq}{y^2}$.

**Conclusion:** In the limit $y \gg a$, the field behaves like that of a single point charge of magnitude **$3q$** (the sum of the two charges) located at the origin.
$$\vec{E} \approx \frac{k(3q)}{y^2} \hat{j}$$
