To solve this problem, we will apply **Coulomb's Law** and the **Principle of Superposition**. 

### 1. Identify the Given Information
* **Corner Charges ($q$):** Four identical positive charges, each $q_1 = q_2 = q_3 = q_4 = +1.0\text{ C}$.
* **Central Charge ($Q$):** A single negative charge $Q = -2.0\text{ C}$.
* **Square Side ($s$):** $1.0\text{ m}$.
* **Coulomb's Constant ($k$):** $\approx 8.99 \times 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$.

### 2. Determine the Geometry
The central charge $Q$ is located at the geometric center of the square. To find the force, we first need the distance $r$ from any corner to the center.

1.  **Diagonal of the square ($d$):** Using the Pythagorean theorem ($d^2 = s^2 + s^2$):
    $$d = \sqrt{1.0^2 + 1.0^2} = \sqrt{2}\text{ m}$$
2.  **Distance to the center ($r$):** The distance from a corner to the center is half of the diagonal:
    $$r = \frac{d}{2} = \frac{\sqrt{2}}{2}\text{ m} \approx 0.707\text{ m}$$



### 3. Calculate the Magnitude of Individual Forces
According to **Coulomb’s Law**, the magnitude of the force ($F$) exerted by one corner charge ($q$) on the central charge ($Q$) is:
$$F = k \frac{|q \cdot Q|}{r^2}$$

Plugging in the values:
$$F = (8.99 \times 10^9) \frac{|(1.0)( -2.0)|}{(\frac{\sqrt{2}}{2})^2}$$
$$F = (8.99 \times 10^9) \frac{2.0}{0.5}$$
$$F = 35.96 \times 10^9\text{ N}$$

Each of the four corner charges exerts a force of this magnitude on the central charge. Since the corner charges are positive and the central charge is negative, these forces are **attractive** (directed from the center toward each corner).

### 4. Apply the Principle of Superposition (Vector Addition)
The net force on the central charge is the vector sum of the four individual forces:
$$\vec{F}_{\text{net}} = \vec{F}_1 + \vec{F}_2 + \vec{F}_3 + \vec{F}_4$$

Let's look at the arrangement:
* **Force Pair 1 (Opposite Corners):** The force from the top-right corner points toward the top-right. The force from the bottom-left corner points toward the bottom-left. Because the charges at these corners are equal and the distances are equal, these two force vectors have the same magnitude but point in **exactly opposite directions**. They cancel each other out.
    $$\vec{F}_{\text{top-right}} + \vec{F}_{\text{bottom-left}} = 0$$
* **Force Pair 2 (Opposite Corners):** Similarly, the force from the top-left corner and the force from the bottom-right corner are equal in magnitude and opposite in direction. They also cancel each other out.
    $$\vec{F}_{\text{top-left}} + \vec{F}_{\text{bottom-right}} = 0$$

### 5. Final Result
Because of the perfect symmetry of the square and the equality of the corner charges:
* **Magnitude:** $0\text{ N}$
* **Direction:** Undefined (the charge is in electrostatic equilibrium).

**Conclusion:** The net electric force on the $-2.0\text{ C}$ charge at the center is **zero**. Every pull from one corner is perfectly balanced by an equal and opposite pull from the diagonally opposite corner.
