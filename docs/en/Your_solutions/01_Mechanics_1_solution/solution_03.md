

### Fundamental Theory

When analyzing the movement of two objects using parametric equations (where position is a function of time, $t$), we must distinguish between two concepts:
1.  **Path Intersection:** The physical geometric paths cross. Alice and Bob step on the exact same location, but potentially at *different* times.
2.  **Collision:** Alice and Bob are at the exact same location at the *exact same time*.
3.  **Distance Optimization:** If they do not collide, the distance between them changes over time. We can find the minimum distance by creating a function for the distance between their coordinates, squaring it (to remove the messy square root for calculus), and finding the minimum using a first derivative.



---

### Step 1: Check for Collision

A collision occurs if there is a single time $t$ where both the $x$ and $y$ coordinates of Alice and Bob are identical. 
$$A(t) = B(t)$$

Let's test the $x$-coordinates:
$$x_A(t) = x_B(t)$$
$$2 + t = 2t - 1$$
$$3 = t$$

For a collision to happen, their $y$-coordinates must *also* be equal at exactly $t = 3$. Let's test the $y$-coordinates:
$$y_A(t) = y_B(t)$$
$$8 - 3t = 2t + 2$$
$$6 = 5t$$
$$t = 1.2$$

**Conclusion:** Since $t = 3 \neq t = 1.2$, Alice and Bob **do not collide**. They reach the matching horizontal coordinates at 3 seconds, but the matching vertical coordinates at 1.2 seconds.

---

### Step 2: Check for Path Intersection

Their physical paths cross if Alice is at a point at time $t_A$ and Bob is at that *same* point at time $t_B$. We set up a system of equations:
1. $2 + t_A = 2t_B - 1 \quad \Rightarrow \quad t_A - 2t_B = -3$
2. $8 - 3t_A = 2t_B + 2 \quad \Rightarrow \quad 3t_A + 2t_B = 6$

We can solve this system by adding Equation 1 and Equation 2 together:
$$(t_A - 2t_B) + (3t_A + 2t_B) = -3 + 6$$
$$4t_A = 3$$
$$t_A = 0.75 \text{ seconds}$$

Now plug $t_A$ back into Equation 1 to find $t_B$:
$$0.75 - 2t_B = -3$$
$$3.75 = 2t_B$$
$$t_B = 1.875 \text{ seconds}$$

**Answer:** Yes, **their paths intersect**. The intersection occurs at the physical coordinate $(2.75, 5.75)$. Alice crosses this point at $t = 0.75\text{s}$, and Bob crosses this exact same spot later at $t = 1.875\text{s}$.

---

### Step 3: Determine the Minimum Distance

Since they do not collide, let's find the minimum distance between them. The distance $D(t)$ between two points $(x_A, y_A)$ and $(x_B, y_B)$ is given by the distance formula:
$$D(t) = \sqrt{(x_A - x_B)^2 + (y_A - y_B)^2}$$

To make the calculus easier, we will optimize the *square* of the distance, $D^2(t)$. 
First, find the differences in their coordinates at any time $t$:
* $X_{diff} = (2 + t) - (2t - 1) = 3 - t$
* $Y_{diff} = (8 - 3t) - (2t + 2) = 6 - 5t$

Now, build the $D^2(t)$ function:
$$D^2(t) = (3 - t)^2 + (6 - 5t)^2$$

Expand the binomials:
$$D^2(t) = (9 - 6t + t^2) + (36 - 60t + 25t^2)$$
$$D^2(t) = 26t^2 - 66t + 45$$

To find the minimum, take the derivative with respect to $t$ and set it to $0$:
$$\frac{d}{dt} [D^2(t)] = 52t - 66$$
$$0 = 52t - 66$$
$$52t = 66$$
$$t = \frac{66}{52} = \frac{33}{26} \approx 1.269 \text{ seconds}$$

Finally, plug this time back into the distance squared function to find the actual minimum distance:
$$D^2\left(\frac{33}{26}\right) = 26\left(\frac{33}{26}\right)^2 - 66\left(\frac{33}{26}\right) + 45$$
$$D^2 = \frac{26 \cdot 1089}{676} - \frac{2178}{26} + \frac{1170}{26}$$
$$D^2 = \frac{1089}{26} - \frac{2178}{26} + \frac{1170}{26}$$
$$D^2 = \frac{81}{26}$$

Take the square root to find $D$:
$$D = \sqrt{\frac{81}{26}} = \frac{9}{\sqrt{26}} \approx 1.765 \text{ units}$$

**Answer:** The minimum distance between Alice and Bob is exactly **$\frac{9}{\sqrt{26}}$ units (approx. 1.765 units)**, and it occurs at exactly **$t = \frac{33}{26}$ seconds (approx. 1.269 s)**.

---
