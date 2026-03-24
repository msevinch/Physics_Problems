
### 3. Conservation of Energy


### Fundamental Theory

To solve this, we rely on the **Law of Conservation of Mechanical Energy**. In an ideal system with no air resistance or friction at the pivot, the total mechanical energy of the pendulum remains constant. 

When the pendulum is pulled back, it gains Gravitational Potential Energy ($PE$). As it swings down, this potential energy is converted entirely into Kinetic Energy ($KE$) at the very bottom of the swing.

$$Energy_{Top} = Energy_{Bottom}$$
$$PE_{Top} = KE_{Bottom}$$



---

### Step 1: Define the Energy Equations
* **Gravitational Potential Energy ($PE$):** The energy stored due to height is calculated as $PE = mgh$, where $m$ is mass, $g$ is the acceleration due to gravity (approx. $9.8 \text{ m/s}^2$), and $h$ is the change in height.
* **Kinetic Energy ($KE$):** The energy of motion is calculated as $KE = \frac{1}{2}mv^2$, where $v$ is the velocity.

Setting them equal:
$$mgh = \frac{1}{2}mv^2$$

Notice that the mass ($m$) appears on both sides, so we can cancel it out. This means the speed at the bottom is completely independent of how heavy the pendulum bob is:
$$gh = \frac{1}{2}v^2$$

### Step 2: Determine the Change in Height ($h$)
We need to figure out how high the bob was lifted from its resting position. We can find this using simple trigonometry based on the length of the string ($L$) and the release angle ($\theta$).

When hanging straight down, the bob is at length $L$ from the pivot. When pulled to an angle $\theta$, the vertical depth from the pivot to the bob forms the adjacent side of a right triangle, which is $L\cos\theta$. 

The height ($h$) the bob has risen is the difference between the full length of the string and that vertical depth:
$$h = L - L\cos\theta$$
$$h = L(1 - \cos\theta)$$

### Step 3: Create the Final Velocity Formula
Substitute our new expression for $h$ back into the simplified energy equation:
$$g \cdot L(1 - \cos\theta) = \frac{1}{2}v^2$$

Multiply both sides by 2 and take the square root to isolate the velocity ($v$):
$$v^2 = 2gL(1 - \cos\theta)$$
$$v = \sqrt{2gL(1 - \cos\theta)}$$

### Step 4: Plug in the Known Values
Now we substitute the values provided in your problem:
* $g \approx 9.8 \text{ m/s}^2$
* $L = 1.0 \text{ m}$
* $\theta = 15^\circ$

First, calculate the cosine of 15 degrees:
$$\cos(15^\circ) \approx 0.9659$$

Now, find the height ($h$):
$$h = 1.0 \cdot (1 - 0.9659)$$
$$h = 1.0 \cdot (0.0341)$$
$$h = 0.0341 \text{ meters}$$

Finally, calculate the velocity ($v$):
$$v = \sqrt{2 \cdot 9.8 \cdot 0.0341}$$
$$v = \sqrt{19.6 \cdot 0.0341}$$
$$v = \sqrt{0.66836}$$
$$v \approx 0.817 \text{ m/s}$$

**Answer:** The speed of the pendulum bob at the exact bottom of its swing is approximately **0.817 m/s**.

---
