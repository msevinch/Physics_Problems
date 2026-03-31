

### 1. Theory
For a particle under a **constant force** $\vec{F}$:
* **Acceleration ($\vec{a}$):** Found via Newton's Second Law ($\vec{F} = m\vec{a}$). Since $\vec{F}$ is constant, $\vec{a}$ is also constant.
* **Kinematics:** We use the integral forms of motion for constant acceleration.
* **Work ($W$):** The work done by a constant force is the dot product of the force vector and the displacement vector ($\vec{F} \cdot \Delta\vec{r}$).
* **Work-Energy Theorem:** The net work done on an object equals its change in kinetic energy ($W = \Delta K$).

---

### 2. Determine (Step-by-Step)

#### **A. Acceleration $\vec{a}(t)$**
Using Newton's Second Law:
$$\vec{a} = \frac{\vec{F}}{m} = \frac{[6, 2]}{2} = [3, 1] \, \text{m/s}^2$$
Since the force does not change with time, the acceleration is constant: **$\vec{a}(t) = 3\mathbf{i} + 1\mathbf{j}$**.

#### **B. Velocity $\vec{v}(t)$**
Using the kinematic equation $\vec{v}(t) = \vec{v}_0 + \vec{a}t$:
$$\vec{v}(t) = [1, -1] + [3, 1]t$$
**$\vec{v}(t) = (1 + 3t)\mathbf{i} + (t - 1)\mathbf{j} \, \text{m/s}$**

#### **C. Position $\vec{r}(t)$**
Using the kinematic equation $\vec{r}(t) = \vec{r}_0 + \vec{v}_0t + \frac{1}{2}\vec{a}t^2$:
$$\vec{r}(t) = [0, 0] + [1, -1]t + \frac{1}{2}[3, 1]t^2$$
**$\vec{r}(t) = (t + 1.5t^2)\mathbf{i} + (0.5t^2 - t)\mathbf{j} \, \text{m}$**

#### **D. Trajectory**
The trajectory is a **parabola**. Since the acceleration vector $[3, 1]$ and the initial velocity $[1, -1]$ are not collinear, the object follows a curved path in the $xy$-plane.



---

### 3. Work Done at $t = 3 \, \text{s}$

**Step 1: Find the displacement $\Delta\vec{r}$ at $t=3$:**
Substitute $t=3$ into the position equation:
* $x(3) = 3 + 1.5(3^2) = 3 + 13.5 = 16.5 \, \text{m}$
* $y(3) = 0.5(3^2) - 3 = 4.5 - 3 = 1.5 \, \text{m}$
$$\Delta\vec{r} = [16.5, 1.5] \, \text{m}$$

**Step 2: Calculate Work ($W = \vec{F} \cdot \Delta\vec{r}$):**
$$W = [6, 2] \cdot [16.5, 1.5]$$
$$W = (6 \times 16.5) + (2 \times 1.5) = 99 + 3 = 102 \, \text{J}$$

---

### 4. Verification: Work-Energy Theorem
We check if $W = K_{final} - K_{initial}$.

**Initial Kinetic Energy ($K_0$):**
$$\vec{v}(0) = [1, -1] \implies v_0^2 = 1^2 + (-1)^2 = 2$$
$$K_0 = \frac{1}{2}mv_0^2 = \frac{1}{2}(2)(2) = 2 \, \text{J}$$

**Final Kinetic Energy ($K_3$) at $t=3$:**
First, find the velocity at $t=3$:
$$\vec{v}(3) = [1 + 3(3), 3 - 1] = [10, 2]$$
$$v_3^2 = 10^2 + 2^2 = 104$$
$$K_3 = \frac{1}{2}mv_3^2 = \frac{1}{2}(2)(104) = 104 \, \text{J}$$

**Change in Kinetic Energy ($\Delta K$):**
$$\Delta K = 104 \, \text{J} - 2 \, \text{J} = 102 \, \text{J}$$

**Conclusion:** Since $W = 102 \, \text{J}$ and $\Delta K = 102 \, \text{J}$, the **Work-Energy Theorem is verified**.
