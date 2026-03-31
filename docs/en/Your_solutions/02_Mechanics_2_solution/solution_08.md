
### 1. Theory
A **conservative force** is a force where the work done depends only on the initial and final positions, not the path taken. For such forces, we can define a **Potential Energy ($U$)** function. 
* The **Equation of Motion** is derived from Newton's Second Law ($F = ma$).
* The **Work-Energy Theorem** states that the work done by a force is the integral of that force over a displacement.
* **Potential Energy** is defined as the negative of the work done by a conservative force: $\Delta U = -W$.

---

### 2. Formulas
* **Newton's Second Law:** $F = m \frac{d^2x}{dt^2}$
* **Work Integral:** $W = \int_{x_1}^{x_2} F(x) \, dx$
* **Potential Energy Relation:** $F(x) = -\frac{dU}{dx}$
* **Angular Frequency:** $\omega = \sqrt{\frac{k}{m}}$

---

### 3. Determine (Step-by-Step Solution)

#### A. Equation of Motion and its Solution
Given $F(x) = -kx$, substitute this into Newton's Second Law:
$$m \frac{d^2x}{dt^2} = -kx \implies \frac{d^2x}{dt^2} + \frac{k}{m}x = 0$$
Let $\omega^2 = \frac{k}{m}$. The equation becomes:
$$\frac{d^2x}{dt^2} + \omega^2x = 0$$
This is a second-order linear differential equation representing **Simple Harmonic Motion (SHM)**. The general solution is:
$$x(t) = A \cos(\omega t + \phi)$$
*Where $A$ is the amplitude and $\phi$ is the phase constant.*

#### B. Work Done from $0$ to $x_0$
Work is the integral of the force over the displacement:
$$W = \int_{0}^{x_0} F(x) \, dx = \int_{0}^{x_0} (-kx) \, dx$$
$$W = -k \left[ \frac{1}{2}x^2 \right]_{0}^{x_0} = -\frac{1}{2}kx_0^2$$
The negative sign indicates that the force is acting in the opposite direction of the displacement (it is a restorative force).

#### C. Interpretation as Potential Energy
Potential energy $U(x)$ is defined as the work done by an **external agent** to move the object against the force, or simply the negative of the work done by the conservative force:
$$U(x) = -\int_{0}^{x} F(x') \, dx' = \int_{0}^{x} kx' \, dx'$$
$$U(x) = \frac{1}{2}kx^2$$
This represents the energy stored in the system (like a compressed or stretched spring) due to its position.

#### D. Verify the Relationship $F = -\frac{dU}{dx}$
Take the negative derivative of the potential energy function:
$$-\frac{dU}{dx} = -\frac{d}{dx} \left( \frac{1}{2}kx^2 \right)$$
$$-\frac{dU}{dx} = -\left( \frac{1}{2}k \cdot 2x \right) = -kx$$
Since this result equals our original $F(x)$, the relationship is verified.

---

### 4. Visual Representation (Graphs)

**The Force Graph ($F(x) = -kx$):**
This is a straight line passing through the origin with a negative slope ($-k$). It shows that as displacement increases, the restoring force increases in the opposite direction.



**The Potential Energy Graph ($U(x) = \frac{1}{2}kx^2$):**
This is a parabola opening upwards, centered at the origin. It shows that potential energy is always positive (whether $x$ is positive or negative) and increases quadratically with displacement.


