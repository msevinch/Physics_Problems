
### **1. Theory: Series vs. Parallel Circuits**

When resistors are connected in a circuit, the way they are arranged determines how they resist the flow of electrical current and how the battery's voltage is distributed.

**Series Connection:**
In a series circuit, resistors are connected end-to-end, creating a single path for the electrons to flow.

* **Equivalent Resistance:** Because the current must push through every resistor one after the other, the total (equivalent) resistance is simply the sum of the individual resistances:

$$R_{eq} = R_1 + R_2 + R_3 + \dots$$


* **Current:** According to Ohm's Law ($V = I \cdot R$), the total current leaving the battery is determined by the total voltage divided by this equivalent resistance:

$$I = \frac{V}{R_{eq}}$$



**Parallel Connection:**
In a parallel circuit, the resistors are connected across multiple branches. The current from the battery splits, giving the electrons multiple paths to travel.

* **Equivalent Resistance:** Because there are multiple paths, the overall resistance to flow actually *decreases*. The reciprocal of the equivalent resistance is the sum of the reciprocals of the individual resistances:

$$\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + \dots$$


* **Current:** Just like in the series circuit, the total current leaving the battery is found using Ohm's Law with the newly calculated equivalent resistance.

---

### **2. Determination: Step-by-Step Calculation**

**Given Values:**

* Voltage ($V$) = **12 V**
* Resistor 1 ($R_1$) = **15 Ω**
* Resistor 2 ($R_2$) = **30 Ω**
* Resistor 3 ($R_3$) = **50 Ω**

#### **Case A: All Resistors Connected in Series**

**Step 1: Calculate Equivalent Resistance ($R_{eq}$)**
Add the resistance values directly:


$$R_{eq} = 15 + 30 + 50$$

$$R_{eq} = 95\text{ }\Omega$$

**Step 2: Calculate Total Current ($I$)**
Use Ohm's Law:


$$I = \frac{12}{95}$$

$$I \approx 0.126\text{ A}$$


*(The current flowing from the battery is approximately 126 mA).*

#### **Case B: All Resistors Connected in Parallel**

**Step 1: Calculate Equivalent Resistance ($R_{eq}$)**
Sum the reciprocals of the resistance values:


$$\frac{1}{R_{eq}} = \frac{1}{15} + \frac{1}{30} + \frac{1}{50}$$

To add these fractions, find a common denominator (which is 150):


$$\frac{1}{R_{eq}} = \frac{10}{150} + \frac{5}{150} + \frac{3}{150}$$

$$\frac{1}{R_{eq}} = \frac{18}{150}$$

Now, invert the fraction to solve for $R_{eq}$:


$$R_{eq} = \frac{150}{18}$$

$$R_{eq} = \frac{25}{3} \approx 8.33\text{ }\Omega$$

**Step 2: Calculate Total Current ($I$)**
Use Ohm's Law with the exact fractional value to avoid rounding errors:


$$I = \frac{12}{25/3}$$

$$I = \frac{12 \cdot 3}{25}$$

$$I = \frac{36}{25}$$

$$I = 1.44\text{ A}$$

---

### **Final Answer Summary**

* **Series Connection:** The equivalent resistance is **95 Ω**, and the total current flowing from the battery is **~0.126 A**.
* **Parallel Connection:** The equivalent resistance is **~8.33 Ω**, and the total current flowing from the battery is exactly **1.44 A**.
