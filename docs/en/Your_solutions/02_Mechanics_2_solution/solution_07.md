```python?code_reference&code_event_index=2
m1 = 5
m2 = 10
F = 45
mu = 0.2
g = 9.8

# Friction on top block surface (from block A to block B)
N1 = m1 * g
f1 = mu * N1

# Friction on bottom block surface (from ground to block B)
N2 = (m1 + m2) * g
f2 = mu * N2

# Net force on block B
F_net = F - f1 - f2

# Acceleration
a = F_net / m2

print(f"{N1=}")
print(f"{f1=}")
print(f"{N2=}")
print(f"{f2=}")
print(f"{F_net=}")
print(f"{a=}")


```
```text?code_stdout&code_event_index=2
N1=49.0
f1=9.8
N2=147.0
f2=29.400000000000002
F_net=5.800000000000001
a=0.5800000000000001

```
To solve for the acceleration of the 10 kg block, we must analyze the forces acting on each component of the system, considering that the 5 kg block is stationary (tied to the wall) while the 10 kg block moves beneath it.



### 1. Theory
This problem involves **Newton's Second Law of Motion** ($F = ma$) and the concept of **Kinetic Friction**. 

* **Block A (5 kg):** It is tied to the wall, so its acceleration is zero ($a_1 = 0$). Because the 10 kg block moves relative to it, there is a kinetic friction force acting on the bottom surface of Block A and the top surface of Block B.
* **Block B (10 kg):** It is subjected to an external horizontal force of 45 N. As it moves, it faces resistance from two friction forces:
    1.  **Friction from Block A:** Since Block A is stationary, Block B slides underneath it. This creates a kinetic friction force opposing Block B's motion.
    2.  **Friction from the Ground:** The ground supports the total weight of both blocks ($m_1 + m_2$). This results in a kinetic friction force between the ground and Block B.
* **Relative Motion:** Since Block B is moving and Block A is held stationary, both friction forces are kinetic.

### 2. Formulas
We use the following physical equations:
* **Normal Force ($N$):** $N = m \cdot g$
* **Kinetic Friction ($f_k$):** $f_k = \mu_k \cdot N$
* **Net Force ($\sum F$):** $\sum F = F_{applied} - \sum f_{friction}$
* **Acceleration ($a$):** $a = \frac{\sum F}{m}$

Where $g = 9.8 \, \text{m/s}^2$.

### 3. Determine (Step-by-Step Solution)

**Step A: Calculate Friction between Block A and Block B ($f_1$)**
The normal force on Block A is its own weight:
$$N_1 = m_1 \cdot g = 5 \, \text{kg} \times 9.8 \, \text{m/s}^2 = 49 \, \text{N}$$
The friction force acting on Block B due to Block A is:
$$f_1 = \mu_k \cdot N_1 = 0.2 \times 49 \, \text{N} = 9.8 \, \text{N}$$

**Step B: Calculate Friction between Block B and the Ground ($f_2$)**
The normal force on the ground is the total weight of both blocks (since Block A is resting on Block B):
$$N_2 = (m_1 + m_2) \cdot g = (5 + 10) \, \text{kg} \times 9.8 \, \text{m/s}^2 = 15 \times 9.8 = 147 \, \text{N}$$
The friction force from the ground is:
$$f_2 = \mu_k \cdot N_2 = 0.2 \times 147 \, \text{N} = 29.4 \, \text{N}$$

**Step C: Calculate the Net Force on Block B**
Block B is pulled by a 45 N force, but it is hindered by both friction forces ($f_1$ and $f_2$):
$$\sum F = F_{applied} - f_1 - f_2$$
$$\sum F = 45 \, \text{N} - 9.8 \, \text{N} - 29.4 \, \text{N}$$
$$\sum F = 5.8 \, \text{N}$$

**Step D: Calculate the Acceleration of Block B ($a_2$)**
Using Newton's Second Law for Block B ($m_2 = 10 \, \text{kg}$):
$$a_2 = \frac{\sum F}{m_2}$$
$$a_2 = \frac{5.8 \, \text{N}}{10 \, \text{kg}} = 0.58 \, \text{m/s}^2$$

**Final Answer:**
The acceleration of the 10 kg block is **$0.58 \, \text{m/s}^2$**.
