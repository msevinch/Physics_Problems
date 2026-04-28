```python?code_reference&code_event_index=2
k = 8.9875517923e9
G = 6.67430e-11
q_e = 1.602176634e-19
m_p = 1.67262192369e-27
m_e = 9.1093837e-31
r = 5.3e-11

F_e = k * (q_e**2) / (r**2)
F_g = G * m_p * m_e / (r**2)
ratio = F_e / F_g

print(f"{F_e=}")
print(f"{F_g=}")
print(f"{ratio=}")

```
```text?code_stdout&code_event_index=2
F_e=8.213163233719126e-08
F_g=3.6202683619962034e-47
ratio=2.2686614395598055e+39

```
This comparison highlights the staggering difference in strength between the electromagnetic force and gravity at the atomic scale. To solve this, we will calculate both forces using their respective universal laws.

---

### 1. Identify the Physical Constants
To be precise, we need the following values:
* **Proton Charge ($q_p$):** $+1.602 \times 10^{-19}\text{ C}$
* **Electron Charge ($q_e$):** $-1.602 \times 10^{-19}\text{ C}$
* **Proton Mass ($m_p$):** $1.673 \times 10^{-27}\text{ kg}$
* **Electron Mass ($m_e$):** $9.109 \times 10^{-31}\text{ kg}$
* **Distance ($r$):** $5.3 \times 10^{-11}\text{ m}$
* **Coulomb's Constant ($k$):** $8.99 \times 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$
* **Gravitational Constant ($G$):** $6.674 \times 10^{-11}\text{ N}\cdot\text{m}^2/\text{kg}^2$

---

### 2. Calculate the Electric Force ($F_e$)
Using **Coulomb’s Law**:
$$F_e = k \frac{|q_p q_e|}{r^2}$$

$$F_e = (8.99 \times 10^9) \frac{(1.602 \times 10^{-19})^2}{(5.3 \times 10^{-11})^2}$$
$$F_e \approx 8.21 \times 10^{-8}\text{ N}$$



---

### 3. Calculate the Gravitational Force ($F_g$)
Using **Newton’s Law of Universal Gravitation**:
$$F_g = G \frac{m_p m_e}{r^2}$$

$$F_g = (6.674 \times 10^{-11}) \frac{(1.673 \times 10^{-27})(9.109 \times 10^{-31})}{(5.3 \times 10^{-11})^2}$$
$$F_g \approx 3.62 \times 10^{-47}\text{ N}$$

---

### 4. Calculate the Ratio ($F_e / F_g$)
Note that when calculating the ratio, the distance $r^2$ cancels out, meaning the relative strength of these forces is independent of the distance between the particles:
$$\frac{F_e}{F_g} = \frac{k |q_p q_e|}{G m_p m_e}$$

Plugging in our calculated results:
$$\text{Ratio} = \frac{8.21 \times 10^{-8}}{3.62 \times 10^{-47}}$$
$$\text{Ratio} \approx 2.27 \times 10^{39}$$

---

### Final Result Summary

| Force Type | Magnitude |
| :--- | :--- |
| **Electric Force ($F_e$)** | $\approx 8.21 \times 10^{-8}\text{ N}$ |
| **Gravitational Force ($F_g$)** | $\approx 3.62 \times 10^{-47}\text{ N}$ |
| **Ratio ($F_e / F_g$)** | $\approx 2.27 \times 10^{39}$ |

**Conclusion:** The electric force is approximately **$10^{39}$ times stronger** than the gravitational force. This is why gravity is completely neglected when studying atomic and molecular interactions; it is effectively non-existent compared to the massive "pull" of electromagnetism.
