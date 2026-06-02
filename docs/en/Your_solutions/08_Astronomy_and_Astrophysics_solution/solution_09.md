```python
import math

theta1 = 89.85
theta2 = 89.75
alpha = 0.53
d_EM = 3.84e5

# 1. d_ES
d_ES1 = d_EM / math.cos(math.radians(theta1))

# 2. D_S
alpha_rad = math.radians(alpha)
D_S = alpha_rad * d_ES1

# 3. Ratio D_M / D_S
# Since D_M = alpha_rad * d_EM
D_M = alpha_rad * d_EM
ratio = D_M / D_S

# 4. Change in d_ES
d_ES2 = d_EM / math.cos(math.radians(theta2))
diff = d_ES1 - d_ES2

print(f"d_ES1: {d_ES1}")
print(f"D_S: {D_S}")
print(f"Ratio D_M/D_S: {ratio}")
print(f"Ratio D_S/D_M: {1/ratio}")
print(f"d_ES2: {d_ES2}")
print(f"diff: {diff}")



```

```text
d_ES1: 146677363.10522616
D_S: 1356801.5498946088
Ratio D_M/D_S: 0.002617990887418114
Ratio D_S/D_M: 381.97229975319317
d_ES2: 88006596.5853948
diff: 58670766.51983136


```


### 1. The Earth–Sun distance ($d_{ES}$)

**Theory:** At the exact half-Moon phase (dichotomy), the Earth, Moon, and Sun form a right-angled triangle with the $90^\circ$ angle located at the Moon. The observer is on Earth, looking at both the Sun and the Moon, and the angular separation between them is given as $\theta$. Based on right triangle trigonometry, the cosine of the angle $\theta$ is the ratio of the adjacent side (Earth–Moon distance, $d_{EM}$) to the hypotenuse (Earth–Sun distance, $d_{ES}$).

$$\cos(\theta) = \frac{d_{EM}}{d_{ES}}$$

**Determination:**
Rearranging for $d_{ES}$ and plugging in the given values ($d_{EM} = 3.84 \times 10^5$ km and $\theta = 89.85^\circ$):

$$d_{ES} = \frac{3.84 \times 10^5}{\cos(89.85^\circ)}$$

$$d_{ES} = \frac{3.84 \times 10^5}{0.002618} \approx 1.467 \times 10^8 \text{ km}$$

### 2. The true diameter of the Sun ($D_S$)

**Theory:**
For objects that subtend a very small angle in the sky, we can use the small-angle approximation. If the apparent angular diameter is $\alpha$ (expressed in radians) and the distance to the object is $d$, the true diameter $D$ is approximated by arc length:

$$D \approx \alpha \times d$$

**Determination:**
First, we must convert the angular diameter $\alpha = 0.53^\circ$ into radians:

$$\alpha \text{ (in radians)} = 0.53^\circ \times \frac{\pi}{180^\circ} \approx 0.00925 \text{ rad}$$

Using the previously calculated distance to the Sun ($d_{ES}$):

$$D_S = 0.00925 \times 1.467 \times 10^8 \approx 1.357 \times 10^6 \text{ km}$$

### 3. The ratio of true diameters ($D_M / D_S$)

**Theory:**
Because the apparent angular diameter $\alpha$ of both the Sun and the Moon is the same as viewed from Earth, the ratio of their true diameters is strictly proportional to the ratio of their distances.

$$\frac{D_M}{d_{EM}} = \alpha \quad \text{and} \quad \frac{D_S}{d_{ES}} = \alpha$$

**Determination:**
By equating the two expressions, the ratio of their diameters is simply the ratio of their distances, which we already know is equal to $\cos(\theta)$:

$$\frac{D_M}{D_S} = \frac{d_{EM}}{d_{ES}} = \cos(89.85^\circ) \approx 0.002618$$

*(Note: This means the Moon's diameter is roughly $0.26\%$ of the Sun's diameter, or conversely, the Sun is about $382$ times larger than the Moon: $D_S/D_M \approx 382$)*.

### 4. Adjusting to $\theta = 89.75^\circ$ and Sensitivity Analysis

**Determination:**
If we recalculate the Earth-Sun distance using a separation angle of $\theta = 89.75^\circ$:

$$d_{ES}' = \frac{3.84 \times 10^5}{\cos(89.75^\circ)} = \frac{3.84 \times 10^5}{0.004363} \approx 8.801 \times 10^7 \text{ km}$$

Comparing this to our original calculation:


$$\Delta d_{ES} = 1.467 \times 10^8 - 8.801 \times 10^7 = 5.869 \times 10^7 \text{ km}$$

**Commentary on Sensitivity:**
A mere $0.1^\circ$ difference in the measurement of the angle $\theta$ results in an enormous shift of nearly $58.7$ million kilometers (about a $40\%$ drop in the calculated distance).
This demonstrates that as $\theta$ approaches $90^\circ$, the cosine function approaches $0$ and becomes non-linear and extremely steep. Small measurement errors in $\theta$ yield massive errors in $d_{ES}$.

For Aristarchus, this implied that while his **geometric theory was perfectly flawless**, the practical execution of his method was nearly impossible with the naked eye. Precisely determining the exact moment of dichotomy (when the terminator line on the Moon is perfectly straight) is incredibly difficult, making his method heavily susceptible to observational error.
