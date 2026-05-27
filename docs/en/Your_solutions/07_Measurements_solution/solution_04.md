Here is the step-by-step solution to find the range of the car's actual speed, breaking down the underlying theory of relative uncertainty and the calculation.

### **1. Theory: Relative vs. Absolute Uncertainty**

When an uncertainty is given as a percentage, it is known as a **relative uncertainty** (or fractional uncertainty). It tells you the size of the measurement error relative to the total measured value.

To find the actual physical range of possible values, you must convert this percentage back into an **absolute uncertainty** ($\delta v$).

The relationship between the absolute uncertainty ($\delta v$), the measured value ($v$), and the percentage uncertainty is defined as:


$$\text{Percentage Uncertainty} = \left( \frac{\delta v}{v} \right) \cdot 100$$

By rearranging this formula to solve for the absolute uncertainty, we get:


$$\delta v = v \cdot \left( \frac{\text{Percentage Uncertainty}}{100} \right)$$

Once the absolute uncertainty is calculated, the true value is expressed as $v \pm \delta v$. This creates a range from a minimum possible value ($v - \delta v$) to a maximum possible value ($v + \delta v$).

---

### **2. Determination: Step-by-Step Calculation**

**Given Values:**

* Measured speed ($v$) = **60 km/h**
* Percentage uncertainty = **5%**

#### **Step A: Calculate the Absolute Uncertainty ($\delta v$)**

First, convert the 5% relative uncertainty into a decimal by dividing by 100 (which gives **0.05**). Then, multiply it by the measured speed:


$$\delta v = 60 \cdot 0.05$$

$$\delta v = 3$$

The absolute uncertainty is **3 km/h**. This means the speedometer could be off by exactly 3 kilometers per hour in either direction.

#### **Step B: Determine the Range**

Apply the absolute uncertainty to the measured speed to find the lower and upper bounds of the car's actual speed:

* **Lower Bound (Minimum Speed):** 60 - 3 = **57 km/h**
* **Upper Bound (Maximum Speed):** 60 + 3 = **63 km/h**

---

### **Final Answer**

The absolute uncertainty of the speedometer is **± 3 km/h**. Therefore, the actual speed of the car falls strictly within the range of **57 km/h to 63 km/h**.
