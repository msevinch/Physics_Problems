### 10. Kinematics

### Fundamental Theory

When dealing with kinematics in three dimensions, the position of a particle is given by a vector $\vec{r}(t) = (x(t), y(t), z(t))$. 
* **Trajectory Equation:** To find the geometric shape of the path independent of time, we mathematically eliminate the time variable ($t$) to relate the $x$, $y$, and $z$ coordinates directly.
* **Path Length (Arc Length):** The distance an object travels along its curved path is found by integrating its speed (the magnitude of the velocity vector) over a given time interval: $S = \int |\vec{v}(t)| dt$.



---

### Part A: Equation of the Trajectory

We are given the parametric equations for the $x$, $y$, and $z$ components:
1.  $x(t) = a\cos(\omega t)$
2.  $y(t) = b\sin(\omega t)$
3.  $z(t) = bt$

First, let's isolate the trigonometric functions in the $x$ and $y$ equations:
$$\frac{x}{a} = \cos(\omega t)$$
$$\frac{y}{b} = \sin(\omega t)$$

Square both equations and add them together to utilize the fundamental trigonometric identity $\cos^2(\theta) + \sin^2(\theta) = 1$:
$$\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = \cos^2(\omega t) + \sin^2(\omega t)$$
$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$$

**Answer (a):** The projection of the trajectory on the $xy$-plane is an ellipse. Because the $z$-coordinate increases linearly with time ($z = bt$), the point moves continuously upwards while tracing this ellipse. The overall trajectory is an **elliptical helix** that lies strictly on the surface of the elliptical cylinder defined by $\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$.

---

### Part B: Compute the Path Length

**1. Find the Velocity Vector $\vec{v}(t)$:**
Take the time derivative of the position vector $\vec{r}(t)$:
$$\vec{v}(t) = \frac{d\vec{r}}{dt} = \left( \frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt} \right)$$
$$\vec{v}(t) = (-a\omega\sin(\omega t), b\omega\cos(\omega t), b)$$

**2. Find the Speed $|\vec{v}(t)|$:**
Calculate the magnitude of the velocity vector using the 3D Pythagorean theorem:
$$|\vec{v}(t)| = \sqrt{(-a\omega\sin(\omega t))^2 + (b\omega\cos(\omega t))^2 + b^2}$$
$$|\vec{v}(t)| = \sqrt{a^2\omega^2\sin^2(\omega t) + b^2\omega^2\cos^2(\omega t) + b^2}$$

**3. Set up the Integral:**
The path length $S$ from $t=0$ to $t=t_0$ is:
$$S = \int_{0}^{t_0} \sqrt{a^2\omega^2\sin^2(\omega t) + b^2\omega^2\cos^2(\omega t) + b^2} \, dt$$

**Answer (b):** Because $a$ and $b$ are distinct constants, this integral does not evaluate to a simple elementary function; it requires what is known as an **incomplete elliptic integral of the second kind**. The exact path length is represented by the definite integral above. 

*(Note: We will see in the special cases below how this simplifies if the constants are modified).*

---

### Part C: Discussion of Special Cases

The most mathematically significant special case occurs if we assume **$a = b$**. 

If $a = b$, the base equation $\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$ simplifies to $x^2 + y^2 = a^2$. The elliptical cylinder becomes a perfect circular cylinder, and the trajectory becomes a standard **circular helix**. 

This dramatically simplifies the path length calculation. Let's look at the speed equation if we substitute $a$ for $b$:
$$|\vec{v}(t)| = \sqrt{a^2\omega^2\sin^2(\omega t) + a^2\omega^2\cos^2(\omega t) + b^2}$$
Factor out $a^2\omega^2$:
$$|\vec{v}(t)| = \sqrt{a^2\omega^2(\sin^2(\omega t) + \cos^2(\omega t)) + b^2}$$
$$|\vec{v}(t)| = \sqrt{a^2\omega^2(1) + b^2}$$
$$|\vec{v}(t)| = \sqrt{a^2\omega^2 + b^2}$$

Because $a, \omega$, and $b$ are constants, the speed is strictly constant! The integral for path length then becomes trivial:
$$S = \int_{0}^{t_0} \sqrt{a^2\omega^2 + b^2} \, dt = t_0\sqrt{a^2\omega^2 + b^2}$$

---
