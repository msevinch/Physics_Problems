Here is the step-by-step solution for calculating the resistance and its associated uncertainty, using the standard rules for error propagation.

### **1. Theory: Propagation of Error for Quotients**

When calculating a final value from the division of two independent measurements, the relative (or fractional) uncertainties of those measurements combine to form the relative uncertainty of the final result.

For a calculated quotient $R = \frac{V}{I}$, where the voltage $V$ and current $I$ have independent and random uncertainties ($\delta V$ and $\delta I$), the standard method is to add their relative uncertainties in **quadrature**.

This is derived from the general partial derivative formula for error propagation:


$$\delta R = \sqrt{\left(\frac{\partial R}{\partial V}\delta V\right)^2 + \left(\frac{\partial R}{\partial I}\delta I\right)^2}$$

Because the partial derivatives are $\frac{\partial R}{\partial V} = \frac{1}{I}$ and $\frac{\partial R}{\partial I} = -\frac{V}{I^2}$, dividing the entire equation by $R$ (which is $V/I$) simplifies it to the standard relative uncertainty formula for quotients:


$$\frac{\delta R}{R} = \sqrt{\left(\frac{\delta V}{V}\right)^2 + \left(\frac{\delta I}{I}\right)^2}$$


---

### **2. Determination: Step-by-Step Calculation**

**Given Values:**

* Voltage ($V$) = **10.0 V**
* Uncertainty in voltage ($\delta V$) = **0.2 V**
* Current ($I$) = **2.00 A**
* Uncertainty in current ($\delta I$) = **0.05 A**

#### **Step A: Calculate the Nominal Resistance ($R$)**

Using Ohm's Law:


$$R = \frac{V}{I}$$

Substitute the measured values:


$$R = \frac{10.0}{2.00}$$

$$R = 5.00 \ \Omega$$

#### **Step B: Calculate the Propagated Uncertainty ($\delta R$)**

First, calculate the relative uncertainty for each measurement:

* Relative error in voltage: $\frac{\delta V}{V} = \frac{0.2}{10.0} = 0.02$
* Relative error in current: $\frac{\delta I}{I} = \frac{0.05}{2.00} = 0.025$

Now, combine them in quadrature using the formula from the theory section:


$$\frac{\delta R}{R} = \sqrt{(0.02)^2 + (0.025)^2}$$

$$\frac{\delta R}{R} = \sqrt{0.0004 + 0.000625}$$

$$\frac{\delta R}{R} = \sqrt{0.001025}$$

$$\frac{\delta R}{R} \approx 0.0320156$$

To find the absolute uncertainty ($\delta R$), multiply this relative uncertainty by the nominal resistance ($R$):


$$\delta R = R \cdot \left(\frac{\delta R}{R}\right)$$

$$\delta R = 5.00 \cdot 0.0320156$$

$$\delta R \approx 0.160078 \ \Omega$$

#### **Step C: Rounding and Significant Figures**

Apply the standard rules for experimental significant figures:

1. **Round the uncertainty:** Uncertainties are typically rounded to one significant figure. However, the accepted convention is to keep **two** significant figures when the leading digit is a 1, which prevents severe rounding errors.
* We round $0.160078$ to **0.16 Ω**.


2. **Match the nominal value:** The main value must be rounded to match the decimal precision (the hundredths place) of the rounded uncertainty.
* Our calculated $R$ is $5.00$, which already matches the hundredths place.



---

### **Final Answer**

Using standard error propagation (quadrature), the calculated resistance and its associated uncertainty is:
**R = 5.00 ± 0.16 Ω**

