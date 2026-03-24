Here is the step-by-step theoretical solution for both questions based on the physics of a simple pendulum.

### Fundamental Theory

The period ($T$) of a simple pendulum—the time it takes to complete one full back-and-forth swing—is determined by its length ($L$) and the local acceleration due to gravity ($g$). The formula is:

$$T = 2\pi \sqrt{\frac{L}{g}}$$

*Notice that the mass of the pendulum bob and the amplitude of the swing (as long as the angle is small) do not affect the period.*

---

### Part 1: Period on the Moon

**1. Establish the known variables on Earth:**
On Earth, the period is 4 seconds. Let's write the formula for Earth:
$$T_{Earth} = 2\pi \sqrt{\frac{L}{g_{Earth}}} = 4 \text{ s}$$

**2. Set up the formula for the Moon:**
We know the gravity on the Moon ($g_{Moon}$) is roughly $\frac{1}{6}$ of Earth's gravity ($g_{Earth}$). We substitute this into the standard period formula:
$$T_{Moon} = 2\pi \sqrt{\frac{L}{g_{Moon}}}$$
$$T_{Moon} = 2\pi \sqrt{\frac{L}{\left(\frac{g_{Earth}}{6}\right)}}$$

**3. Isolate the "Earth" portion of the equation:**
When dividing by a fraction inside the square root, we can multiply by its reciprocal (which means pulling the 6 to the numerator):
$$T_{Moon} = 2\pi \sqrt{6 \cdot \frac{L}{g_{Earth}}}$$

We can factor out the $\sqrt{6}$:
$$T_{Moon} = \sqrt{6} \cdot \left( 2\pi \sqrt{\frac{L}{g_{Earth}}} \right)$$

**4. Solve for the new period:**
Notice that the term in the parentheses is exactly the formula for the Earth period, which we know is exactly 4 seconds.
$$T_{Moon} = \sqrt{6} \cdot T_{Earth}$$
$$T_{Moon} = \sqrt{6} \cdot 4$$
$$T_{Moon} \approx 2.449 \cdot 4 \approx 9.80 \text{ seconds}$$

**Answer:** The period of the pendulum on the Moon would be approximately **9.80 seconds**. Because gravity is weaker, the restoring force pulling the pendulum down is smaller, causing it to swing much slower.

---

### Part 2: Length for a 1-Second Period on Earth

**1. Establish the known variables:**
* Desired Period ($T$) = $1 \text{ s}$
* Earth's gravity ($g$) $\approx 9.8 \text{ m/s}^2$
* Length ($L$) = Unknown

**2. Substitute knowns into the formula:**
$$1 = 2\pi \sqrt{\frac{L}{9.8}}$$

**3. Isolate the variable $L$ step-by-step:**
First, divide both sides by $2\pi$:
$$\frac{1}{2\pi} = \sqrt{\frac{L}{9.8}}$$

Next, square both sides to remove the square root:
$$\left(\frac{1}{2\pi}\right)^2 = \frac{L}{9.8}$$
$$\frac{1}{4\pi^2} = \frac{L}{9.8}$$

Finally, multiply both sides by 9.8 to solve for $L$:
$$L = \frac{9.8}{4\pi^2}$$

**4. Calculate the final value:**
We know that $\pi \approx 3.14159$, so $\pi^2 \approx 9.8696$. 
$$L \approx \frac{9.8}{4 \cdot 9.8696}$$
$$L \approx \frac{9.8}{39.478}$$
$$L \approx 0.248 \text{ meters}$$

**Answer:** To have a period of exactly 1 second on Earth, the pendulum must be approximately **0.248 meters (or 24.8 centimeters)** long.
