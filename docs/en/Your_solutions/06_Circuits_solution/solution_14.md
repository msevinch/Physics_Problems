## Step 1: Apply Kirchhoff’s Voltage Law (KVL)

For a **series RLC circuit**, the source voltage is shared among:

* Resistor: (V_R)
* Inductor: (V_L)
* Capacitor: (V_C)

Using Kirchhoff’s Voltage Law:

[
V(t)=V_R+V_L+V_C
]

Now write each voltage in terms of current (I(t)).

---

## Step 2: Write the Voltage Relations

### Resistor

By Ohm’s law:

[
V_R = RI(t)
]

### Inductor

Voltage across an inductor:

[
V_L = L\frac{dI}{dt}
]

### Capacitor

For a capacitor:

[
V_C = \frac{q}{C}
]

where (q(t)) is the charge.

Since current is:

[
I(t)=\frac{dq}{dt}
]

we can express everything using charge.

---

## Step 3: Substitute into KVL

Substitute all terms:

[
V(t)=L\frac{dI}{dt}+RI+\frac{q}{C}
]

Since

[
I=\frac{dq}{dt}
]

then

[
\frac{dI}{dt}=\frac{d^2q}{dt^2}
]

So the equation becomes:

[
V(t)=L\frac{d^2q}{dt^2}+R\frac{dq}{dt}+\frac{1}{C}q
]

Rearranging:

[
L\frac{d^2q}{dt^2}+R\frac{dq}{dt}+\frac{1}{C}q=V(t)
]

This is the **differential equation of a series RLC circuit**.

---

# Final Differential Equation

[
\boxed{
L\frac{d^2q}{dt^2}+R\frac{dq}{dt}+\frac{1}{C}q=V(t)
}
]

Since (I=\frac{dq}{dt}), the equation may also be written in current form.

---

# Step 4: Compare with a Damped Harmonic Oscillator

The standard equation of a damped harmonic oscillator is:

m\frac{d^2x}{dt^2}+b\frac{dx}{dt}+kx=F(t)

where:

* (m) = mass
* (b) = damping coefficient
* (k) = spring constant
* (x(t)) = displacement
* (F(t)) = external force

---

# Step 5: Identify the Analogies

Compare the two equations:

### Electrical System

L\frac{d^2q}{dt^2}+R\frac{dq}{dt}+\frac{1}{C}q=V(t)

### Mechanical System

m\frac{d^2x}{dt^2}+b\frac{dx}{dt}+kx=F(t)

---

# Correspondence Between Terms

| RLC Circuit       | Damped Oscillator | Physical Meaning         |
| ----------------- | ----------------- | ------------------------ |
| (q(t))            | (x(t))            | Generalized displacement |
| (I=\frac{dq}{dt}) | (\frac{dx}{dt})   | Velocity                 |
| (L)               | (m)               | Inertia/storage effect   |
| (R)               | (b)               | Damping/loss             |
| (\frac{1}{C})     | (k)               | Restoring effect         |
| (V(t))            | (F(t))            | External driving source  |

---

# Physical Interpretation

## 1. Inductor ↔ Mass

The inductor resists changes in current just like mass resists changes in motion.

[
L \leftrightarrow m
]

---

## 2. Resistor ↔ Damping

The resistor dissipates energy as heat, similar to friction removing energy from oscillation.

[
R \leftrightarrow b
]

---

## 3. Capacitor ↔ Spring

The capacitor stores electrical energy and tends to restore equilibrium, similar to a spring storing elastic energy.

[
\frac{1}{C} \leftrightarrow k
]

---

# Step 6: Natural Oscillation Frequency

For the undamped case ((R=0)):

[
L\frac{d^2q}{dt^2}+\frac{1}{C}q=0
]

The natural angular frequency is:

\omega_0=\frac{1}{\sqrt{LC}}

which is analogous to the mechanical oscillator frequency:

\omega_0=\sqrt{\frac{k}{m}}

---

# Conclusion

The series RLC circuit behaves mathematically exactly like a damped harmonic oscillator.


Thus, electrical oscillations in an RLC circuit follow the same mathematics as mechanical vibrations in a spring–mass–damper system.
