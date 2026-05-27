
### **1. Theoretical Framework & Error Propagation**

#### **Step A: The Physics of a Simple Pendulum**

For a simple pendulum (a point mass on a massless string of length $L$) swinging at small angles, the period of one complete oscillation ($T$) is defined by:


$$T = 2\pi\sqrt{\frac{L}{g}}$$

To determine the acceleration due to gravity ($g$), we rearrange this formula:


$$g = \frac{4\pi^2 L}{T^2}$$

#### **Step B: Statistical Analysis of the Period**

Just like the mass-spring system, human reaction time introduces error. We measure the time for 10 complete oscillations ($t_{10}$) and divide by 10 to find the period of a single oscillation:


$$T_i = \frac{t_{10}}{10}$$

By recording 10 separate trials, we can calculate the **Mean Period** ($\bar{T}$) and the **Standard Deviation** ($\sigma$):


$$\bar{T} = \frac{1}{N} \sum_{i=1}^{N} T_i$$

$$\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^{N} (T_i - \bar{T})^2}$$

The measurement uncertainty of our calculated mean period is the **Standard Error of the Mean** ($\delta T$):


$$\delta T = \frac{\sigma}{\sqrt{N}}$$

#### **Step C: Propagating Uncertainty to Gravity**

Assuming the length ($L$) is an exact value with zero uncertainty ($\delta L = 0$), the error in $g$ stems entirely from our timing error $\delta T$. Because $g$ is inversely proportional to $T^2$ ($g \propto T^{-2}$), the exponent is $n = -2$.

The relative uncertainty is:


$$\frac{\delta g}{g} = |-2| \frac{\delta T}{\bar{T}} = 2 \frac{\delta T}{\bar{T}}$$

Solving for the absolute uncertainty in gravity ($\delta g$):


$$\delta g = 2g \frac{\delta T}{\bar{T}}$$

---

### **2. Virtual Experiment: Pendulum Simulator**

Use the interactive simulator below to run the virtual experiment. It assumes an exact string length of **1.0 m**. You can click the button to simulate the 10 manual stopwatch measurements (which will include slight, realistic human reaction errors), calculate the statistical spread, and determine $g \pm \delta g$.

---

### **3. Real-Life Experiment Guide**

If you want to perform this physically at home, here is how you translate the theory into practice:

**Materials Needed:**

* A string and a small, relatively heavy weight (a metal nut, keys, or a small ball).
* A measuring tape or ruler.
* Your smartphone stopwatch.

**Procedure:**

1. **Set up the pendulum:** Tie the weight to the string and suspend it from a fixed, stable point (like a doorway or the edge of a table).
2. **Measure the length ($L$):** Measure from the pivot point at the top to the *center of mass* of your weight at the bottom. Record this in meters (e.g., 0.85 m).
3. **Perform the trials:** * Pull the mass back slightly (keep the angle less than 15 degrees to keep the physics formula accurate).
* Release the mass and start the stopwatch simultaneously.
* Count 10 *full* oscillations (one oscillation is a complete back-and-forth swing).
* Stop the stopwatch exactly when the 10th swing completes. Record this time as $t_{10}$.


4. **Repeat:** Do this 10 separate times to get your 10 trials.
5. **Calculate:**
* Divide each $t_{10}$ by 10 to get your 10 periods ($T_i$).
* Calculate the mean $\bar{T}$ and standard deviation $\sigma$.
* Calculate the standard error $\delta T = \frac{\sigma}{\sqrt{10}}$.
* Plug your $L$ and $\bar{T}$ into $g = \frac{4\pi^2 L}{\bar{T}^2}$.
* Calculate your uncertainty $\delta g = 2g \frac{\delta T}{\bar{T}}$.



