```python
import math

# ISS calculation
G = 6.67430e-11 # m^3 kg^-1 s^-2
M_E = 5.97e24 # kg
R_E = 6378000 # m (from previous prompt)
h = 400000 # m
r_ISS = R_E + h

v_ISS = math.sqrt((G * M_E) / r_ISS) # m/s
v_ISS_km_s = v_ISS / 1000

# Earth calculation
R_Sun = 150e6 # km
R_Sun_m = R_Sun * 1000 # m
T_days = 365.25
T_seconds = T_days * 24 * 60 * 60

v_Earth_km_s = (2 * math.PI if hasattr(math, 'PI') else 2 * math.pi * R_Sun) / (T_seconds) # km/s
v_Earth_m_s = v_Earth_km_s * 1000

print(f"v_ISS: {v_ISS} m/s, {v_ISS_km_s} km/s")
print(f"v_Earth: {v_Earth_km_s} km/s")



```

```text
v_ISS: 7667.243308183652 m/s, 7.667243308183652 km/s
v_Earth: 29.865319164858477 km/s


```

This problem takes us into the realm of orbital mechanics, where we get to look at two different scales of cosmic motion: a human-made satellite orbiting our planet, and our planet orbiting our star.

Here is the step-by-step breakdown using **Theory** and **Determine** for both calculations, followed by the final comparison.

---

## **Part 1: Orbital Speed of the ISS**

### **The Theory**

For any object to stay in a stable circular orbit, the gravitational force pulling it inward must perfectly balance the centripetal force required to keep it moving in a circle.

Mathematically, this looks like:


$$F_g = F_c \implies \frac{G \cdot M_E \cdot m}{r^2} = \frac{m \cdot v^2}{r}$$

If we solve for the orbital velocity ($v$), the mass of the satellite ($m$) cancels out, leaving us with the orbital speed formula:


$$v = \sqrt{\frac{G \cdot M_E}{r}}$$

Where:

* $G$ = Universal gravitational constant ($\approx 6.674 \times 10^{-11}\text{ m}^3\text{kg}^{-1}\text{s}^{-2}$)
* $M_E$ = Mass of the Earth ($5.97 \times 10^{24}\text{ kg}$)
* $r$ = Total distance from the **center** of the Earth to the ISS ($R_E + \text{altitude}$)

---

### **Determine: Step-by-Step ISS Calculation**

#### **Step 1: Determine the total orbital radius ($r$)**

The ISS orbits 400 km above the surface. We must add this to the Earth's radius ($6378\text{ km}$, from our previous calculation) to find the distance to the Earth's center.


$$r = R_E + \text{altitude}$$

$$r = 6378\text{ km} + 400\text{ km} = 6778\text{ km}$$


Convert this to meters for standard SI units:


$$r = 6,778,000\text{ m}$$

#### **Step 2: Plug the values into the formula**

$$v_{\text{ISS}} = \sqrt{\frac{(6.674 \times 10^{-11}) \cdot (5.97 \times 10^{24})}{6,778,000}}$$

$$v_{\text{ISS}} = \sqrt{\frac{3.9844 \times 10^{14}}{6,778,000}}$$

$$v_{\text{ISS}} = \sqrt{58,784,302}$$

$$v_{\text{ISS}} \approx 7667\text{ m/s}$$

#### **Step 3: Convert to km/s**

$$v_{\text{ISS}} \approx 7.67\text{ km/s}$$

---

## **Part 2: Earth's Orbital Speed Around the Sun**

### **The Theory**

Because we are already given the distance from the Earth to the Sun (the radius of Earth's orbit) and the time it takes to complete one revolution (the period), we don't need to use the gravitational constant here. We can use the simple circular velocity formula:

$$v = \frac{\text{Distance}}{\text{Time}} = \frac{2\pi R_{\text{orbit}}}{T}$$

Where:

* $R_{\text{orbit}}$ = Earth-Sun distance ($\approx 150 \times 10^6\text{ km}$)
* $T$ = Earth's orbital period ($\approx 365.25\text{ days}$)

---

### **Determine: Step-by-Step Earth Calculation**

#### **Step 1: Calculate the total distance (Circumference)**

$$C = 2 \cdot \pi \cdot (150 \times 10^6\text{ km})$$

$$C \approx 2 \cdot 3.14159 \cdot 150,000,000\text{ km}$$

$$C \approx 942,477,796\text{ km}$$

#### **Step 2: Convert the orbital period ($T$) into seconds**

$$T = 365.25\text{ days} \cdot 24\text{ hours/day} \cdot 3600\text{ seconds/hour}$$

$$T \approx 31,557,600\text{ seconds}$$

#### **Step 3: Calculate the Earth's speed ($v$)**

$$v_{\text{Earth}} = \frac{942,477,796\text{ km}}{31,557,600\text{ s}}$$

$$v_{\text{Earth}} \approx 29.87\text{ km/s}$$

---

## **Comparison and Conclusion**

* **ISS around the Earth:** $\approx 7.67\text{ km/s}$ (about $27,600\text{ km/h}$)
* **Earth around the Sun:** $\approx 29.87\text{ km/s}$ (about $107,500\text{ km/h}$)

> **Which is faster?** > The **Earth orbiting the Sun** is significantly faster—nearly **4 times faster** than the ISS orbiting the Earth! Even though the ISS feels like it's blazing across our night sky, it's just a hitchhiker on a planet that is absolutely hauling through the solar system.
