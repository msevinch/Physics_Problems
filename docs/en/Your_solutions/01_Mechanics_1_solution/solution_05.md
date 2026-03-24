### 5. Relative Velocity

### Fundamental Theory

To solve this, we rely on the principle of **Relative Velocity** and vector addition. The boat's actual motion as seen from the shore (its *resultant velocity*) is the combination of its movement through the water and the water's movement over the ground.

Mathematically, this is expressed as a vector sum:
$$\vec{v}_{result} = \vec{v}_{boat} + \vec{v}_{river}$$

Because the boat wants to travel directly North, its eastward/westward movement must perfectly cancel out. Since the river is pushing it East, the boat must aim West of North to fight the current.



---

### Step 1: Determine the Heading Angle ($\theta$)

Let's break the velocities into their horizontal (East/West) components. 
* **River's velocity:** **2 m/s** (East)
* **Boat's speed:** **5 m/s** (At some angle $\theta$ West of North)

To travel exactly North, the boat's westward velocity component must equal the river's eastward velocity. Using trigonometry, the westward component of the boat's velocity is $v_{boat} \sin(\theta)$.

Set these equal to each other:
$$v_{boat} \sin(\theta) = v_{river}$$
$$5 \sin(\theta) = 2$$

Now, isolate and solve for $\theta$:
$$\sin(\theta) = \frac{2}{5} = 0.4$$
$$\theta = \arcsin(0.4)$$
$$\theta \approx 23.58^\circ$$

**Answer:** The boat should head approximately **23.58° West of North** (or an angle of 113.58° measured counter-clockwise from the East bank).

---

### Step 2: Determine the Effective Crossing Speed

Even though the boat's engine is pushing it at **5 m/s**, some of that effort is wasted fighting the current. Its actual speed directly across the river (its northward component) will be less than 5. 

We can find this northward velocity ($v_y$) using the Pythagorean theorem, because the boat's speed, the river's speed, and the resultant speed form a right triangle:
$$v_{boat}^2 = v_y^2 + v_{river}^2$$
$$5^2 = v_y^2 + 2^2$$
$$25 = v_y^2 + 4$$
$$v_y^2 = 21$$
$$v_y = \sqrt{21} \approx 4.58 \text{ m/s}$$

*Alternatively, using trigonometry: $v_y = 5 \cos(23.58^\circ) \approx 4.58 \text{ m/s}$.*

---

### Step 3: Calculate the Time to Cross

Now that we know the boat's effective speed straight across the river, we can find the time ($t$) it takes to cover the **200 m** distance ($d$).

Since velocity is constant, we use the standard kinematic formula:
$$t = \frac{d}{v_y}$$
$$t = \frac{200}{\sqrt{21}}$$
$$t \approx \frac{200}{4.5826}$$
$$t \approx 43.64 \text{ seconds}$$

**Answer:** It will take the boat approximately **43.64 seconds** to cross the 200-meter river.

---
