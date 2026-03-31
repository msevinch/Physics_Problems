

---

### **Step 1: Solve for Velocity $v(t)$**
We start with Newton's Second Law:
$$m \frac{dv}{dt} = -mg - kv$$

**1.1 Separate the variables:**
Move all terms involving $v$ to one side and $t$ to the other:
$$\frac{dv}{mg + kv} = -\frac{1}{m} dt$$

**1.2 Integrate both sides:**
Integrate from the initial state ($t=0, v=v_0$) to a general state ($t, v$):
$$\int_{v_0}^{v} \frac{dv}{mg + kv} = \int_{0}^{t} -\frac{1}{m} dt$$

Using the substitution $u = mg + kv$, where $du = k \, dv$:
$$\frac{1}{k} \left[ \ln(mg + kv) \right]_{v_0}^{v} = -\frac{t}{m}$$
$$\ln\left(\frac{mg + kv}{mg + kv_0}\right) = -\frac{k}{m}t$$

**1.3 Isolate $v$:**
Exponentiate both sides:
$$\frac{mg + kv}{mg + kv_0} = e^{-\frac{k}{m}t}$$
$$v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}$$



---

### **Step 2: Solve for Position $x(t)$**
Since $v = \frac{dx}{dt}$, we integrate the velocity function:
$$x(t) = \int v(t) \, dt = \int \left[ \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k} \right] dt$$

**2.1 Perform the integration:**
$$x(t) = \left(v_0 + \frac{mg}{k}\right) \left( -\frac{m}{k} e^{-\frac{k}{m}t} \right) - \frac{mg}{k}t + C$$

**2.2 Solve for $C$ using initial condition $x(0) = 10$:**
$$10 = -\frac{m}{k}\left(v_0 + \frac{mg}{k}\right)(1) - 0 + C \implies C = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)$$

**2.3 Final Position Equation:**
$$x(t) = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)\left(1 - e^{-\frac{k}{m}t}\right) - \frac{mg}{k}t$$

---

### **Step 3: Determine Maximum Height**
The object reaches its maximum height when its velocity is zero ($v(t_{up}) = 0$).

**3.1 Find the time to reach the peak ($t_{up}$):**
From our velocity equation:
$$0 = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t_{up}} - \frac{mg}{k}$$
$$e^{-\frac{k}{m}t_{up}} = \frac{mg}{mg + kv_0} \implies t_{up} = \frac{m}{k} \ln\left(1 + \frac{kv_0}{mg}\right)$$

**3.2 Find $x_{max}$:**
Substitute $t_{up}$ back into the $x(t)$ equation. After simplifying the exponential term:
$$x_{max} = 10 + \frac{mv_0}{k} - \frac{m^2g}{k^2} \ln\left(1 + \frac{kv_0}{mg}\right)$$

---

### **Step 4: Comparison with the "No Drag" Case**
| Feature | Vacuum (No Drag) | With Drag ($kv$) |
| :--- | :--- | :--- |
| **Forces** | Gravity only | Gravity + Drag |
| **Acceleration** | Constant ($-g$) | Variable ($-g - \frac{k}{m}v$) |
| **Path Symmetry** | Symmetric rise/fall | Asymmetric (risen faster than fallen) |
| **Peak Height** | $10 + \frac{v_0^2}{2g}$ | Always lower than vacuum peak |



---

### **Step 5: Numerical Simulation (Python)**
This script uses the **Euler Method** to approximate the motion and compares it to the ideal trajectory.

```python
import numpy as np
import matplotlib.pyplot as plt

# Parameters
m, g, k = 1.0, 9.81, 0.25
v0, x0 = 30.0, 10.0
dt = 0.01

t_arr, x_drag, v_drag = [0], [x0], [v0]

# Simulation Loop
while x_drag[-1] >= 0:
    # Physics: a = F/m
    a = -g - (k/m) * v_drag[-1]
    
    # Update values
    v_new = v_drag[-1] + a * dt
    x_new = x_drag[-1] + v_drag[-1] * dt
    
    x_drag.append(x_new)
    v_drag.append(v_new)
    t_arr.append(t_arr[-1] + dt)

# Analytical Vacuum Case for comparison
t_ideal = np.array(t_arr)
x_ideal = x0 + v0*t_ideal - 0.5*g*t_ideal**2

# Visualization
plt.figure(figsize=(8, 5))
plt.plot(t_arr, x_drag, label=f"With Drag (k={k})", color='blue', linewidth=2)
plt.plot(t_ideal, x_ideal, label="Vacuum (k=0)", color='red', linestyle='--')
plt.ylim(0, max(x_ideal)+5)
plt.title("Vertical Throw Dynamics")
plt.xlabel("Time (s)"); plt.ylabel("Height (m)")
plt.legend(); plt.grid(True, alpha=0.3)
plt.show()
```
