
---

### **1. Theoretical Framework**

#### **Step A: The Physics of the Spring**

For a mass ($m$) undergoing simple harmonic motion on a spring with a spring constant ($k$), the period of one complete oscillation ($T$) is given by:


$$T = 2\pi\sqrt{\frac{m}{k}}$$

To find the spring constant, we rearrange this formula to solve for $k$:


$$k = \frac{4\pi^2 m}{T^2}$$

#### **Step B: Statistical Analysis of the Period**

Measuring a single oscillation with a stopwatch introduces significant human reaction error. To minimize this, we measure the time for 10 complete oscillations ($t_{10}$) and divide by 10 to find the period of one oscillation:


$$T_i = \frac{t_{10}}{10}$$

By taking 10 separate measurements (trials), we can calculate the **Mean Period** ($\bar{T}$) and the **Standard Deviation** ($\sigma$) of those periods to understand the spread of our data:


$$\bar{T} = \frac{1}{N} \sum_{i=1}^{N} T_i$$

$$\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^{N} (T_i - \bar{T})^2}$$

The measurement uncertainty of our mean period ($\delta T$) is represented by the **Standard Error of the Mean** (SEM), which divides the standard deviation by the square root of the number of trials ($N=10$):


$$\delta T = \frac{\sigma}{\sqrt{N}}$$

#### **Step C: Propagation of Error for the Spring Constant**

We are given that the mass ($m$) has zero uncertainty ($\delta m = 0$). Therefore, the uncertainty in the calculated spring constant ($\delta k$) comes entirely from the uncertainty in our period measurement ($\delta T$).

Using the relative uncertainty rule for power functions (since $k \propto T^{-2}$, the exponent $n = -2$), the relative uncertainty is:


$$\frac{\delta k}{k} = |-2| \frac{\delta T}{\bar{T}}$$

Solving for the absolute uncertainty of the spring constant ($\delta k$):


$$\delta k = 2k \frac{\delta T}{\bar{T}}$$

---

### **2. Interactive Mass-Spring Simulator**

Use the widget below to perform the experiment. The simulator will generate 10 realistic stopwatch measurements (including slight random human reaction variations), calculate the statistical spread, and determine $k \pm \delta k$.
