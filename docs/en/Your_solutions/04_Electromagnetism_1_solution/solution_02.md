
---

### 1. Identify the Given Parameters
* **Charges:** $q_1 = +1\text{ C}$, $q_2 = -2\text{ C}$, $q_3 = +3\text{ C}$, $q_4 = -4\text{ C}$
* **Side of the square ($s$):** $1.0\text{ m}$
* **Coulomb's Constant ($k$):** $\approx 8.99 \times 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$

### 2. Determine the Geometry (Distance $r$)
To find the potential at the center, we need the distance $r$ from any corner of the square to its center.

1.  **Calculate the Diagonal ($d$):** Using the Pythagorean theorem for a square:
    $$d = \sqrt{s^2 + s^2} = s\sqrt{2} = 1.0\sqrt{2} \approx 1.414\text{ m}$$
2.  **Calculate Distance to Center ($r$):** The center is exactly half the diagonal length from any corner:
    $$r = \frac{d}{2} = \frac{\sqrt{2}}{2} \approx 0.7071\text{ m}$$



### 3. Theoretical Formula
The electric potential $V$ at a point due to a single point charge $q$ is given by:
$$V = \frac{kq}{r}$$

According to the **Principle of Superposition**, the total potential $V_{\text{total}}$ at the center is the algebraic sum of the potentials from each of the four charges:
$$V_{\text{total}} = V_1 + V_2 + V_3 + V_4$$
$$V_{\text{total}} = \frac{kq_1}{r} + \frac{kq_2}{r} + \frac{kq_3}{r} + \frac{kq_4}{r}$$

Since $k$ and $r$ are the same for all charges at the center, we can simplify the expression:
$$V_{\text{total}} = \frac{k}{r} (q_1 + q_2 + q_3 + q_4)$$

### 4. Step-by-Step Calculation

**Step A: Calculate the net charge ($\sum q$)**
$$\sum q = (+1) + (-2) + (+3) + (-4)$$
$$\sum q = 1 - 2 + 3 - 4 = -2\text{ C}$$

**Step B: Substitute values into the simplified equation**
$$V_{\text{total}} = \frac{8.99 \times 10^9}{0.7071} \times (-2)$$

**Step C: Final Computation**
$$V_{\text{total}} \approx (1.271 \times 10^{10}) \times (-2)$$
$$V_{\text{total}} \approx -2.542 \times 10^{10}\text{ V}$$

---

### Final Result
The electric potential at the center of the square is:
**$-2.54 \times 10^{10}\text{ V}$** (or **$-25.4\text{ GV}$**)

**Key Takeaway:** Because electric potential is a scalar, the "order" of the charges does not change the result at the center. The negative result indicates that the net electric potential is dominated by the negative charges in the system.
