
### 1. Theory
According to **Newton's Second Law**, the net force on a particle is proportional to its acceleration ($F = ma$). 
* Because the force is a function of time, the acceleration will also be a function of time. 
* To find **velocity**, we integrate acceleration with respect to time and add the initial velocity vector.
* To find **position**, we integrate the velocity function and add the initial position vector.

---

### 2. Formulas
* **Acceleration:** $\mathbf{a}(t) = \frac{\mathbf{F}(t)}{m}$
* **Velocity:** $\mathbf{v}(t) = \int \mathbf{a}(t) \, dt + \mathbf{v}_0$
* **Position:** $\mathbf{r}(t) = \int \mathbf{v}(t) \, dt + \mathbf{r}_0$

Given: $m = 3 \, \text{kg}$, $\mathbf{v}_0 = (2, 0, 1)$, $\mathbf{r}_0 = (5, 2, -3)$.

---

### 3. Determine (Step-by-Step Solution)

#### **Step A: Find the Acceleration $\mathbf{a}(t)$**
Divide each component of the force vector by the mass ($m=3$):
* $a_x = \frac{15t}{3} = 5t$
* $a_y = \frac{3t - 12}{3} = t - 4$
* $a_z = \frac{-6t^2}{3} = -2t^2$

**Vector form:** $\mathbf{a}(t) = (5t, t - 4, -2t^2) \, \text{m/s}^2$

#### **Step B: Find the Velocity $\mathbf{v}(t)$**
Integrate each component of acceleration and add the initial velocity $\mathbf{v}_0$:
* $v_x = \int 5t \, dt = \frac{5}{2}t^2 + v_{0x} = 2.5t^2 + 2$
* $v_y = \int (t - 4) \, dt = \frac{1}{2}t^2 - 4t + v_{0y} = 0.5t^2 - 4t + 0$
* $v_z = \int -2t^2 \, dt = -\frac{2}{3}t^3 + v_{0z} = -\frac{2}{3}t^3 + 1$

**Result:** $\mathbf{v}(t) = (2.5t^2 + 2)\mathbf{i} + (0.5t^2 - 4t)\mathbf{j} + (-\frac{2}{3}t^3 + 1)\mathbf{k} \, \text{m/s}$

#### **Step C: Find the Position $\mathbf{r}(t)$**
Integrate each component of velocity and add the initial position $\mathbf{r}_0$:

**X-component:**
$x(t) = \int (2.5t^2 + 2) \, dt = \frac{2.5}{3}t^3 + 2t + x_0 = \frac{5}{6}t^3 + 2t + 5$

**Y-component:**
$y(t) = \int (0.5t^2 - 4t) \, dt = \frac{0.5}{3}t^3 - \frac{4}{2}t^2 + y_0 = \frac{1}{6}t^3 - 2t^2 + 2$

**Z-component:**
$z(t) = \int (-\frac{2}{3}t^3 + 1) \, dt = -\frac{2}{12}t^4 + t + z_0 = -\frac{1}{6}t^4 + t - 3$

---

### **Final Results Summary**

| Quantity | Time-Dependent Expression |
| :--- | :--- |
| **Velocity $\mathbf{v}(t)$** | $(2.5t^2 + 2, 0.5t^2 - 4t, -0.67t^3 + 1)$ |
| **Position $\mathbf{r}(t)$** | $(\frac{5}{6}t^3 + 2t + 5, \frac{1}{6}t^3 - 2t^2 + 2, -\frac{1}{6}t^4 + t - 3)$ |

*(Note: Fractions like $\frac{5}{6}$ and $\frac{1}{6}$ are kept for exact precision, but can be approximated as $0.833$ and $0.167$ if needed.)*
