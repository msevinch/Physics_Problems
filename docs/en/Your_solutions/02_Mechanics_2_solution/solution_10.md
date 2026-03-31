

### **Step 1: The Position Vector ($\mathbf{r}$)**
First, we write the given coordinates as a single position vector $\mathbf{r}(t)$:
$$\mathbf{r}(t) = (5t^2 - t)\mathbf{i} + (2t^3)\mathbf{j} + (-3t + 2)\mathbf{k}$$

---

### **Step 2: Find Velocity ($\mathbf{v}$)**
**Theory:** Velocity is the rate of change of position ($d\mathbf{r}/dt$). We differentiate each component with respect to time.
* **x-component:** $\frac{d}{dt}(5t^2 - t) = 10t - 1$
* **y-component:** $\frac{d}{dt}(2t^3) = 6t^2$
* **z-component:** $\frac{d}{dt}(-3t + 2) = -3$

**Result:** $\mathbf{v}(t) = (10t - 1)\mathbf{i} + 6t^2\mathbf{j} - 3\mathbf{k}$

---

### **Step 3: Find Momentum ($\mathbf{p}$)**
**Theory:** Momentum is mass times velocity ($\mathbf{p} = m\mathbf{v}$). Here, $m = 0.5$ kg.
* **x:** $0.5 \times (10t - 1) = 5t - 0.5$
* **y:** $0.5 \times (6t^2) = 3t^2$
* **z:** $0.5 \times (-3) = -1.5$

**Result:** $\mathbf{p}(t) = (5t - 0.5)\mathbf{i} + 3t^2\mathbf{j} - 1.5\mathbf{k}$

---

### **Step 4: Find Acceleration ($\mathbf{a}$)**
**Theory:** Acceleration is the rate of change of velocity ($d\mathbf{v}/dt$). We differentiate our velocity results.
* **x:** $\frac{d}{dt}(10t - 1) = 10$
* **y:** $\frac{d}{dt}(6t^2) = 12t$
* **z:** $\frac{d}{dt}(-3) = 0$

**Result:** $\mathbf{a}(t) = 10\mathbf{i} + 12t\mathbf{j} + 0\mathbf{k}$

---

### **Step 5: Find Force ($\mathbf{F}$)**
**Theory:** Newton’s Second Law ($\mathbf{F} = m\mathbf{a}$). Multiply acceleration by $m = 0.5$ kg.
* **x:** $0.5 \times 10 = 5$
* **y:** $0.5 \times 12t = 6t$
* **z:** $0.5 \times 0 = 0$

**Result:** $\mathbf{F}(t) = 5\mathbf{i} + 6t\mathbf{j} + 0\mathbf{k}$

---

### **Step 6: Find Power ($P$)**
**Theory:** Power is the dot product of the Force and Velocity vectors ($P = \mathbf{F} \cdot \mathbf{v}$).
Multiply corresponding components and add them up:
$$P = (F_x \cdot v_x) + (F_y \cdot v_y) + (F_z \cdot v_z)$$
$$P = [5 \cdot (10t - 1)] + [6t \cdot (6t^2)] + [0 \cdot (-3)]$$
$$P = 50t - 5 + 36t^3$$

**Final Result:** $P(t) = 36t^3 + 50t - 5$ Watts.

