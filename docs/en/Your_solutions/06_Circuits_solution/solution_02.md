
### **1. Theory: Resistor Network Topologies**

When you have exactly three identical resistors, there are exactly **four unique ways (topologies)** to connect them together in a circuit.

The formulas used to calculate their combinations are:

* **Series Formula:** Resistors connected end-to-end add up directly.

$$R_{\text{series}} = R_1 + R_2 + \dots$$


* **Parallel Formula:** For resistors connected side-by-side, the reciprocal of the total resistance is the sum of the reciprocals.

$$\frac{1}{R_{\text{parallel}}} = \frac{1}{R_1} + \frac{1}{R_2} + \dots$$


* **Two-Resistor Parallel Shortcut:** When exactly two resistors are in parallel, you can use the product-over-sum rule:

$$R_p = \frac{R_1 \cdot R_2}{R_1 + R_2}$$



---

### **2. Determination: Step-by-Step Calculations**

Let our three resistors be $R_1 = 1\ \Omega$, $R_2 = 1\ \Omega$, and $R_3 = 1\ \Omega$.

#### **Configuration 1: All Three in Series**

The current must pass through all three resistors sequentially.

* **Calculation:** 
$$R_{\text{eq}} = R_1 + R_2 + R_3$$


$$R_{\text{eq}} = 1 + 1 + 1 = 3\ \Omega$$



#### **Configuration 2: All Three in Parallel**

The current splits evenly across three separate parallel branches.

* **Calculation:**

$$\frac{1}{R_{\text{eq}}} = \frac{1}{1} + \frac{1}{1} + \frac{1}{1} = 3$$


$$R_{\text{eq}} = \frac{1}{3}\ \Omega \approx 0.33\ \Omega$$



#### **Configuration 3: Two in Parallel, in Series with the Third**

First, combine two resistors in parallel, then treat that entire block as being in a straight line (series) with the final remaining resistor.

* **Step 1 (Parallel block):** 
$$R_p = \frac{1 \cdot 1}{1 + 1} = 0.5\ \Omega$$


* **Step 2 (Add the third in series):** 
$$R_{\text{eq}} = R_p + R_3$$


$$R_{\text{eq}} = 0.5 + 1 = 1.5\ \Omega \text{ (or } \frac{3}{2}\ \Omega\text{)}$$



#### **Configuration 4: Two in Series, in Parallel with the Third**

First, combine two resistors in a single series line, then treat that combined branch as being in parallel with the final single resistor.

* **Step 1 (Series branch):** 
$$R_s = 1 + 1 = 2\ \Omega$$


* **Step 2 (Parallel with the third):** 
$$R_{\text{eq}} = \frac{R_s \cdot R_3}{R_s + R_3}$$


$$R_{\text{eq}} = \frac{2 \cdot 1}{2 + 1} = \frac{2}{3}\ \Omega \approx 0.67\ \Omega$$



---

### **Final Answer Summary**

By combining all three $1\ \Omega$ resistors, you can create exactly **4 unique values** of equivalent resistance:

1. **0.33 Ω** (or $\frac{1}{3}\ \Omega$) — *All in parallel*
2. **0.67 Ω** (or $\frac{2}{3}\ \Omega$) — *Two in series, parallel to the third*
3. **1.50 Ω** (or $\frac{3}{2}\ \Omega$) — *Two in parallel, series to the third*
4. **3.00 Ω** — *All in series*

*(Note: If your prompt allowed for networks where you don't use all three resistors, you could also get **1 Ω** by using just a single resistor, and **0.5 Ω** or **2 Ω** by using only two of them.)*
