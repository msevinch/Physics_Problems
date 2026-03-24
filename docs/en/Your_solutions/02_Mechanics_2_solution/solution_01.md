```python?code_reference&code_event_index=2
import math

# Problem 1
T_earth = 4
g_ratio = 1/6
T_moon = T_earth * math.sqrt(1 / g_ratio)

# Problem 2
T_target = 1
g_earth = 9.80665 # Standard gravity
L = g_earth * (T_target / (2 * math.pi))**2

print(f"{T_moon=}")
print(f"{L=}")


```
```text?code_stdout&code_event_index=2
T_moon=9.797958971132712
L=0.24840534639153294

```
To solve these problems, we use the fundamental formula for the period of a simple pendulum (for small angles):

$$T = 2\pi \sqrt{\frac{L}{g}}$$

Where:
* $T$ is the period (seconds)
* $L$ is the length of the pendulum (meters)
* $g$ is the acceleration due to gravity ($m/s^2$)



[Image of simple pendulum]


---

### 1. Gravitational Dependence: Period on the Moon

To find the period on the Moon without knowing the specific length, we can use the relationship between the period and gravity. From the formula, we see that the period is inversely proportional to the square root of the gravitational acceleration ($T \propto \frac{1}{\sqrt{g}}$).

**Step 1: Set up the ratio between Earth and Moon**
$$\frac{T_{moon}}{T_{earth}} = \frac{2\pi \sqrt{\frac{L}{g_{moon}}}}{2\pi \sqrt{\frac{L}{g_{earth}}}}$$

Since the length $L$ is the same, the constants $2\pi$ and $\sqrt{L}$ cancel out:
$$\frac{T_{moon}}{T_{earth}} = \sqrt{\frac{g_{earth}}{g_{moon}}}$$

**Step 2: Substitute the known gravity ratio**
We are told $g_{moon} = \frac{1}{6} g_{earth}$. Therefore:
$$\frac{T_{moon}}{T_{earth}} = \sqrt{\frac{g_{earth}}{\frac{1}{6}g_{earth}}} = \sqrt{6}$$

**Step 3: Calculate the Moon's period**
$$T_{moon} = T_{earth} \times \sqrt{6}$$
$$T_{moon} = 4 \text{ s} \times \sqrt{6} \approx 4 \times 2.449$$
$$T_{moon} \approx 9.80 \text{ seconds}$$

**Result:** The period of the pendulum on the Moon would be approximately **9.80 seconds**.

---

### 2. Required Length for a 1-Second Period on Earth

To find the specific length $L$ required for a target period, we rearrange the period formula to solve for $L$.

**Step 1: Rearrange the formula**
Square both sides of the original equation:
$$T^2 = (2\pi)^2 \frac{L}{g}$$
$$T^2 = 4\pi^2 \frac{L}{g}$$

Now, solve for $L$:
$$L = \frac{g \cdot T^2}{4\pi^2} \quad \text{or} \quad L = g \left( \frac{T}{2\pi} \right)^2$$

**Step 2: Substitute the known values**
On Earth, standard gravity $g \approx 9.81 \text{ m/s}^2$ and the desired period $T = 1 \text{ s}$.
$$L = 9.81 \cdot \left( \frac{1}{2\pi} \right)^2$$
$$L = \frac{9.81}{4\pi^2}$$

**Step 3: Calculate the final value**
$$L \approx \frac{9.81}{4 \times 3.14159^2}$$
$$L \approx \frac{9.81}{39.478}$$
$$L \approx 0.2485 \text{ meters}$$

**Result:** To have a period of exactly 1 second on Earth, the pendulum must have a length of approximately **0.248 meters** (or **24.8 cm**).
