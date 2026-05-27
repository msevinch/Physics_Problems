Here is the step-by-step solution for calculating the area of the rectangular plate and its associated uncertainty.

### **1. Theory: Propagation of Error for Products**

When calculating a final value from two or more independent measurements, the uncertainties of those measurements combine to form the uncertainty of the final result.

For a calculated area $A = L \cdot W$, where the length $L$ and width $W$ have independent and random uncertainties ($\delta L$ and $\delta W$), the standard method to determine the propagated uncertainty ($\delta A$) is adding them in **quadrature**. This is derived from the general partial derivative formula for error propagation:


$$\delta A = \sqrt{\left(\frac{\partial A}{\partial L}\delta L\right)^2 + \left(\frac{\partial A}{\partial W}\delta W\right)^2}$$

Because the partial derivatives for a simple product are $\frac{\partial A}{\partial L} = W$ and $\frac{\partial A}{\partial W} = L$, this simplifies to:


$$\delta A = \sqrt{(W \cdot \delta L)^2 + (L \cdot \delta W)^2}$$

Alternatively, this can be written using relative uncertainties:


$$\frac{\delta A}{A} = \sqrt{\left(\frac{\delta L}{L}\right)^2 + \left(\frac{\delta W}{W}\right)^2}$$

*(Note: In some introductory courses, a simpler "maximum error" or "worst-case" method is taught, which simply adds the relative errors: $\frac{\delta A}{A} = \frac{\delta L}{L} + \frac{\delta W}{W}$. The quadrature method above is the more rigorous standard for independent random errors and will be used for the primary determination here.)*

---

### **2. Determination: Step-by-Step Calculation**

**Given Values:**

* Length ($L$) = **15.3 cm**
* Uncertainty in length ($\delta L$) = **0.1 cm**
* Width ($W$) = **8.4 cm**
* Uncertainty in width ($\delta W$) = **0.1 cm**

#### **Step A: Calculate the Nominal Area ($A$)**

The formula for the area of a rectangle is:


$$A = L \cdot W$$

Substitute the measured values:


$$A = 15.3 \cdot 8.4$$

$$A = 128.52\text{ cm}^2$$

#### **Step B: Calculate the Propagated Uncertainty ($\delta A$)**

Using the simplified absolute uncertainty formula from the theory section:


$$\delta A = \sqrt{(W \cdot \delta L)^2 + (L \cdot \delta W)^2}$$

Substitute the known values:


$$\delta A = \sqrt{(8.4 \cdot 0.1)^2 + (15.3 \cdot 0.1)^2}$$

$$\delta A = \sqrt{(0.84)^2 + (1.53)^2}$$

$$\delta A = \sqrt{0.7056 + 2.3409}$$

$$\delta A = \sqrt{3.0465}$$

$$\delta A \approx 1.7454\text{ cm}^2$$

#### **Step C: Rounding and Significant Figures**

To report the final value properly, we must apply the standard rules for experimental significant figures:

1. **Round the uncertainty:** Experimental uncertainties are usually rounded to one significant figure. However, a standard convention allows keeping **two** significant figures if the leading digit is a 1, to avoid disproportionate rounding errors.
* Following this rule, we round $1.7454$ to **1.7 cm²**.


2. **Match the nominal value:** The main value must be rounded to match the decimal precision (the tenths place) of the rounded uncertainty.
* We round $128.52$ to the nearest tenth, giving us **128.5 cm²**.



---

### **Final Answer**

Using standard error propagation (quadrature), the calculated area of the rectangular plate and its associated uncertainty is:
**A = 128.5 ± 1.7 cm²**

