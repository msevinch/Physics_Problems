

### **1. Theory: Simplifying Mixed Circuits**

To solve a complex circuit, the standard strategy is to work from the "inside out."

1. **Identify Nodes:** Find the junctions (dots) where the current splits or recombines.
2. **Find Simple Series:** Look for paths where the current has no choice but to flow through multiple resistors sequentially. Add their resistances together: $R_{series} = R_1 + R_2 + \dots$
3. **Find Simple Parallels:** Look for paths that start at the same node and end at the same node. Combine them using the parallel formula: $\frac{1}{R_{parallel}} = \frac{1}{R_1} + \frac{1}{R_2} + \dots$

---

### **2. Determination: Step-by-Step Calculation**

First, let's identify the main nodes (junctions) and count the resistors based on the visual blocks in your image:

* **Node A (Input):** The dot at the bottom left.
* **Node B (Top-Mid):** The dot at the top center.
* **Node C (Output):** The dot at the bottom right.
* *(Note: The diagram shows 8 distinct grey rectangles. The central vertical branch and the rightmost vertical branch are each drawn with two resistors.)*

#### **Step A: The Parallel Paths from Node A to Node B**

From the input (Node A), the current can take two different paths to reach the top-mid junction (Node B):

* **Path 1 (Outer Left):** The current goes up through the left vertical resistor and turns right through the top horizontal resistor. Since there are no junctions between them, they are in series.

$$R_{\text{path1}} = 5\ \Omega + 5\ \Omega = 10\ \Omega$$


* **Path 2 (Inner Middle):** The current goes right through the inner horizontal resistor, then turns up and goes through the *two* central vertical resistors. These three are in a single series path.

$$R_{\text{path2}} = 5\ \Omega + 5\ \Omega + 5\ \Omega = 15\ \Omega$$



Now, combine these two parallel paths into a single equivalent resistance ($R_{AB}$):


$$\frac{1}{R_{AB}} = \frac{1}{10} + \frac{1}{15}$$

$$\frac{1}{R_{AB}} = \frac{3}{30} + \frac{2}{30} = \frac{5}{30}$$

$$R_{AB} = \frac{30}{5} = 6\ \Omega$$

#### **Step B: The Series Path from Node B to Node C**

Once the current reaches Node B, it must travel to the output junction (Node C) down the rightmost vertical branch. This branch contains two resistors drawn in series.


$$R_{BC} = 5\ \Omega + 5\ \Omega = 10\ \Omega$$

#### **Step C: Total Upper Network Resistance**

The entire upper complex network is just the $6\ \Omega$ block we calculated in Step A, in series with the $10\ \Omega$ right branch we found in Step B.


$$R_{\text{upper}} = R_{AB} + R_{BC}$$

$$R_{\text{upper}} = 6\ \Omega + 10\ \Omega = 16\ \Omega$$

#### **Step D: Final Equivalent Resistance**

Finally, looking at the whole circuit from input to output, the entire upper network ($16\ \Omega$) is in parallel with the single main bottom horizontal resistor ($5\ \Omega$).

Combine them to find the final equivalent resistance ($R_{eq}$):


$$\frac{1}{R_{eq}} = \frac{1}{16} + \frac{1}{5}$$

$$\frac{1}{R_{eq}} = \frac{5}{80} + \frac{16}{80} = \frac{21}{80}$$

$$R_{eq} = \frac{80}{21}\ \Omega$$

---

### **Final Answer**

Calculating the final fraction gives us the equivalent resistance of the entire circuit:
**$R_{eq} \approx 3.81\ \Omega$**
