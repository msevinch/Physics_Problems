

To make the calculations clean and follow standard physics conventions for this specific angle, we will use the common approximations: **cos(37°) ≈ 0.8** and **sin(37°) ≈ 0.6**. We will use standard Earth gravity as **9.8 m/s²**.



Before diving into the calculus, let's establish our initial velocity components based on the 100 m/s launch speed:
* **Horizontal Velocity:** $v_{0x} = 100 \cdot \cos(37°) = 100 \cdot 0.8 =$ **80 m/s**
* **Vertical Velocity:** $v_{0y} = 100 \cdot \sin(37°) = 100 \cdot 0.6 =$ **60 m/s**

---

### Step 1: Derive the Differential Equations of Motion

To find the equations of motion, we start with Newton's Second Law of Motion ($F = ma$). Because we are ignoring air resistance, the only force acting on the projectile after launch is gravity, which pulls straight down.

**Horizontal Direction (x):**
There are no forces acting in the horizontal direction. Therefore, the horizontal acceleration is zero. 
$$F_x = m \frac{d^2x}{dt^2} = 0$$
Dividing by mass ($m$) gives us our first differential equation:
$$\frac{d^2x}{dt^2} = 0$$

**Vertical Direction (y):**
The only force is gravity acting downwards (negative y-direction). 
$$F_y = m \frac{d^2y}{dt^2} = -mg$$
Dividing by mass ($m$) gives us our second differential equation:
$$\frac{d^2y}{dt^2} = -g$$

---

### Step 2: Determine the Time of Flight

The time of flight is the total time the projectile is in the air before it hits the ground (when $y = 0$).

First, we integrate the vertical differential equation twice to get the position equation $y(t)$:
1.  **Velocity:** Integrate $\frac{d^2y}{dt^2} = -g$ to get $v_y(t) = v_{0y} - gt$.
2.  **Position:** Integrate velocity to get $y(t) = v_{0y}t - \frac{1}{2}gt^2$ (assuming initial height is 0).

To find the time of flight ($t$), we set the final vertical position $y(t)$ to 0:
$$0 = v_{0y}t - \frac{1}{2}gt^2$$
$$0 = t \left(v_{0y} - \frac{1}{2}gt\right)$$

Since $t = 0$ is the launch time, we solve for the other time it hits the ground:
$$v_{0y} = \frac{1}{2}gt$$
$$t = \frac{2v_{0y}}{g}$$

Now, plug in our known values (initial vertical velocity is 60 m/s, gravity is 9.8 m/s²):
$$t = \frac{2 \cdot 60}{9.8}$$
$$t = \frac{120}{9.8} \approx 12.24 \text{ s}$$

**Answer:** The time of flight is approximately **12.24 seconds**.

---

### Step 3: Determine the Maximum Height

The maximum height occurs at the exact peak of the trajectory, where the projectile momentarily stops moving upward before falling back down. At this peak, the vertical velocity $v_y(t)$ is exactly 0.

First, find the time it takes to reach the peak using our velocity equation:
$$v_y(t) = v_{0y} - gt$$
$$0 = v_{0y} - gt_{peak}$$
$$t_{peak} = \frac{v_{0y}}{g} = \frac{60}{9.8} \approx 6.12 \text{ s}$$
*(Note: As expected, this is exactly half the total time of flight).*

Next, plug this peak time into our vertical position equation to find the Max Height ($H$):
$$H = v_{0y}t_{peak} - \frac{1}{2}gt_{peak}^2$$
$$H = 60(6.12) - \frac{1}{2}(9.8)(6.12)^2$$
$$H = 367.2 - 183.53 \approx 183.67 \text{ m}$$

*Alternative shortcut formula:* $H = \frac{v_{0y}^2}{2g} = \frac{60^2}{2 \cdot 9.8} \approx 183.67$ m.

**Answer:** The maximum height reached is approximately **183.67 meters**.

---

### Step 4: Determine the Range

The range ($R$) is the total horizontal distance traveled. 

First, we integrate the horizontal differential equation twice to get the position equation $x(t)$:
1.  **Velocity:** Integrate $\frac{d^2x}{dt^2} = 0$ to get $v_x(t) = v_{0x}$ (horizontal velocity is constant).
2.  **Position:** Integrate velocity to get $x(t) = v_{0x}t$.

To find the total range, we plug the total time of flight (12.24 seconds) into our horizontal position equation:
$$R = v_{0x} \cdot t_{flight}$$
$$R = 80 \cdot 12.24$$
$$R = 979.2 \text{ m}$$

**Answer:** The total horizontal range is exactly **979.2 meters**.

---
