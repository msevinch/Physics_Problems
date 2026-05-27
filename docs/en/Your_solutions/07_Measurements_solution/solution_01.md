
### **1. Theory: Propagation of Error**

When a quantity is calculated from a measured value that has an inherent uncertainty, that uncertainty propagates into the final result.

For a calculated function $V(r)$ dependent on a single measured variable $r$ with an absolute uncertainty $\Delta r$, the absolute uncertainty in the final calculation $\Delta V$ can be determined using the **Derivative Method** (based on a first-order Taylor series expansion):


$$\Delta V = \left| \frac{dV}{dr} \right| \Delta r$$

Alternatively, for power-law relationships like volume where $V = c \cdot r^n$ (where $c$ is a constant), you can use the **Relative Uncertainty Method**. The relative error of the result is the relative error of the measurement multiplied by the exponent $n$:


$$\frac{\Delta V}{V} = |n| \frac{\Delta r}{r}$$

Both methods are mathematically equivalent for this problem and will yield the exact same result.

---

### **2. Determination: Step-by-Step Calculation**

**Given Values:**

* Radius ($r$) = **6.20 cm**
* Uncertainty in radius ($\Delta r$) = **0.05 cm**

#### **Step A: Calculate the Nominal Volume ($V$)**

The formula for the volume of a sphere is:


$$V = \frac{4}{3}\pi r^3$$

Substitute the measured value of the radius:


$$V = \frac{4}{3}\pi (6.20)^3$$

$$V = \frac{4}{3}\pi (238.328)$$

$$V = 998.30599... \text{ cm}^3$$

#### **Step B: Calculate the Propagated Uncertainty ($\Delta V$)**

**Using the Derivative Method:**
First, find the derivative of the volume equation with respect to $r$:


$$\frac{dV}{dr} = \frac{4}{3}\pi (3r^2) = 4\pi r^2$$

Now, multiply this by the given uncertainty $\Delta r$:


$$\Delta V = (4\pi r^2) \Delta r$$

$$\Delta V = 4\pi (6.20)^2 (0.05)$$

$$\Delta V = 4\pi (38.44) (0.05)$$

$$\Delta V = 24.15256... \text{ cm}^3$$


#### **Step C: Rounding and Significant Figures**

Experimental uncertainties determine how you round your final answer.

1. **Round the uncertainty:** Standard practice dictates that uncertainties should be rounded to one significant figure. However, a common exception in experimental physics is to keep *two* significant figures if the leading digit is a 1 or a 2, to prevent overly aggressive rounding.
* Rounding to two significant figures gives us **24 cm³**.


2. **Match the nominal value:** The main value must be rounded to the same decimal place (or place value) as the uncertainty. Since our uncertainty (24) ends in the "ones" place, we round 998.30599... to the nearest whole number, which is **998 cm³**.

---

### **Final Answer**

The calculated volume of the sphere and its associated uncertainty is:
**V = 998 ± 24 cm³** *(If your specific course strictly requires rounding all uncertainties to exactly one significant figure, the result would be rounded to the tens place: **V = 1000 ± 20 cm³**, often written in scientific notation as **(1.00 ± 0.02) × 10³ cm³**).*
