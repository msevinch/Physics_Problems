Here is the step-by-step breakdown of the differential equation for a series RLC circuit, its mechanical analogies, and the theoretical solution using the characteristic equation.

### **1. Deriving the Differential Equation**

In a series RLC circuit, Kirchhoff’s Voltage Law (KVL) states that the sum of the voltage drops across the components must equal the supplied voltage $V(t)$:

$$V_L(t) + V_R(t) + V_C(t) = V(t)$$

Using the fundamental voltage-current relationships for each component:

* **Inductor:** $V_L(t) = L \frac{dI}{dt}$
* **Resistor:** $V_R(t) = R \cdot I(t)$
* **Capacitor:** $I(t) = C \frac{dV_C}{dt}$ (and consequently $V_C(t) = \frac{1}{C} \int I(t) dt$)

**Formulation in terms of Capacitor Voltage, $V_C(t)$:**
Substitute the relationship $I(t) = C \frac{dV_C}{dt}$ and its derivative $\frac{dI}{dt} = C \frac{d^2V_C}{dt^2}$ into the KVL equation:

$$L \left( C \frac{d^2V_C}{dt^2} \right) + R \left( C \frac{dV_C}{dt} \right) + V_C(t) = V(t)$$

Dividing by $LC$ gives the standard standard form:

$$\frac{d^2V_C}{dt^2} + \frac{R}{L} \frac{dV_C}{dt} + \frac{1}{LC} V_C(t) = \frac{V(t)}{LC}$$

**Formulation in terms of Current, $I(t)$:**
If we start with $L \frac{dI}{dt} + RI + \frac{1}{C} \int I dt = V(t)$ and differentiate the entire equation with respect to time $t$, we get:

$$L \frac{d^2I}{dt^2} + R \frac{dI}{dt} + \frac{1}{C} I(t) = \frac{dV(t)}{dt}$$

---

### **2. Analogy to the Damped Harmonic Oscillator**

A damped mechanical harmonic oscillator (like a mass-spring-damper system) is governed by Newton's Second Law:

$$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = F(t)$$

Where $m$ is mass, $b$ is the damping coefficient, $k$ is the spring constant, $x(t)$ is displacement, and $F(t)$ is the external driving force.

If we compare this to the RLC equation expressed in terms of electrical charge $q(t)$ (where $I = \frac{dq}{dt}$):

$$L \frac{d^2q}{dt^2} + R \frac{dq}{dt} + \frac{1}{C} q(t) = V(t)$$

We can draw exact one-to-one mathematical analogies:

| Mechanical System | Electrical System (RLC) | Physical Meaning |
| --- | --- | --- |
| Displacement ($x$) | Charge ($q$) or ($C \cdot V_C$) | The fundamental quantity being moved. |
| Velocity ($v = \dot{x}$) | Current ($I = \dot{q}$) | The rate of flow of the fundamental quantity. |
| Mass ($m$) | Inductance ($L$) | Inertia; resistance to changes in flow/velocity. |
| Damping Constant ($b$) | Resistance ($R$) | Energy dissipation (friction / Joule heating). |
| Spring Constant ($k$) | Inverse Capacitance ($1/C$) | Stiffness; tendency to return to equilibrium. |
| Driving Force ($F$) | Voltage Source ($V$) | The external input driving the system. |

---

### **3. Solving Step-by-Step Using Theory & The Characteristic Equation**

To solve this linear, second-order differential equation, we use the theory of linear operators. The total solution $V_C(t)$ consists of two parts:

1. **Transient Solution** $V_h(t)$: The solution to the homogeneous equation (when $V(t) = 0$).
2. **Steady-State Solution** $V_p(t)$: The particular solution driven by the specific shape of $V(t)$.

Let's find the transient (natural) response using the **characteristic equation** (also known as the determinant of the state matrix).

Set the external voltage to zero:


$$\frac{d^2V_C}{dt^2} + \frac{R}{L} \frac{dV_C}{dt} + \frac{1}{LC} V_C = 0$$

Assume a solution of the form $V_C(t) = A e^{st}$. Substituting this and its derivatives yields the characteristic polynomial:

$$s^2 + \frac{R}{L} s + \frac{1}{LC} = 0$$

To simplify, we define two critical theoretical parameters:

* **Neper Frequency / Damping Factor ($\alpha$):** $\alpha = \frac{R}{2L}$ (How fast the transient dies out).
* **Resonant Frequency ($\omega_0$):** $\omega_0 = \frac{1}{\sqrt{LC}}$ (The frequency of oscillation with zero resistance).

Rewriting the characteristic equation:


$$s^2 + 2\alpha s + \omega_0^2 = 0$$

Using the quadratic formula, the roots (determinants of the system's behavior) are:


$$s_{1,2} = -\alpha \pm \sqrt{\alpha^2 - \omega_0^2}$$

The physical behavior of the circuit depends entirely on the discriminant ($\alpha^2 - \omega_0^2$), leading to three distinct cases:

#### **Case 1: Overdamped ($\alpha > \omega_0$)**

The resistance is high. The roots $s_1$ and $s_2$ are real, negative, and distinct.


$$V_h(t) = A_1 e^{s_1 t} + A_2 e^{s_2 t}$$


*Result:* The voltage smoothly decays to equilibrium without oscillating.

#### **Case 2: Critically Damped ($\alpha = \omega_0$)**

The resistance is perfectly balanced to prevent oscillation while returning to zero as fast as possible. The roots are real and repeated: $s_1 = s_2 = -\alpha$.


$$V_h(t) = (A_1 + A_2 t) e^{-\alpha t}$$


*Result:* The fastest possible decay without ringing.

#### **Case 3: Underdamped ($\alpha < \omega_0$)**

The resistance is low. The roots are complex conjugates: $s_{1,2} = -\alpha \pm j\omega_d$, where $j$ is the imaginary unit and $\omega_d = \sqrt{\omega_0^2 - \alpha^2}$ is the damped resonant frequency.


$$V_h(t) = e^{-\alpha t} (A_1 \cos(\omega_d t) + A_2 \sin(\omega_d t))$$


*Result:* The voltage oscillates (rings) at frequency $\omega_d$ while decaying exponentially.

**Finalizing the Total Solution:**
To find the exact final formula, you add the particular steady-state solution $V_p(t)$—which depends on whether $V(t)$ is a DC step, an AC sine wave, etc.—to the transient solution $V_h(t)$. Finally, the constants $A_1$ and $A_2$ are determined by applying the initial boundary conditions of the circuit (initial voltage across the capacitor $V_C(0)$ and initial current through the inductor $I(0)$).
