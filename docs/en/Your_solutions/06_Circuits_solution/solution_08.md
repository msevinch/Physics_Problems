
### **Part 1: Theory**

To understand how voltage behaves in this circuit, we rely on two fundamental concepts in alternating current (AC) electronics:

1. **Ohm's Law in AC Circuits:** For a purely resistive circuit, Ohm's Law applies to alternating current exactly as it does to direct current. The instantaneous voltage $V(t)$ is directly proportional to the instantaneous current $I(t)$ multiplied by the resistance $R$.

$$V(t) = I(t) \times R$$


2. **Phase Relationship:** In a purely resistive AC circuit, **voltage and current are perfectly in phase**. This means they rise, peak, fall, and cross zero at the exact same moments. Because there is no phase shift (unlike in capacitive or inductive circuits), the sine argument $\omega t$ (angular frequency multiplied by time) remains identical for both the current and voltage equations.

If current is written as $I(t) = I_0 \sin(\omega t)$, then voltage will naturally take the form:


$$V(t) = V_0 \sin(\omega t)$$


*(where $I_0$ is the peak current and $V_0$ is the peak voltage)*

---

### **Part 2: Determine**

**1. Identify the Given Variables**
From the problem statement, we have:

* Current equation: $I(t) = 2 \sin(120\pi t)\text{ A}$
* Resistance ($R$): $50\,\Omega$

**2. Extract Peak Current ($I_0$) and Angular Frequency ($\omega$)**
By matching the given current equation to the standard form $I(t) = I_0 \sin(\omega t)$, we can extract:

* Peak Current ($I_0$) = $2\text{ A}$
* Angular Frequency ($\omega$) = $120\pi\text{ rad/s}$

**3. Calculate Peak Voltage ($V_0$)**
Using Ohm's Law for the peak values:


$$V_0 = I_0 \times R$$

$$V_0 = 2\text{ A} \times 50\,\Omega$$

$$V_0 = 100\text{ V}$$

**4. Formulate the Final Voltage Equation**
Since the voltage is in phase with the current, we keep the exact same angular frequency ($\omega = 120\pi$) and substitute our calculated peak voltage ($V_0 = 100\text{ V}$) into the standard AC voltage template:


$$V(t) = V_0 \sin(\omega t)$$

**Final Equation:**


$$V(t) = 100 \sin(120\pi t)\text{ V}$$
