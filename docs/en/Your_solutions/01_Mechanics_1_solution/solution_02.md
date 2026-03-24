

### Fundamental Theory

In physics, optimization problems—finding the maximum or minimum value of a function—are typically solved using calculus. Alternatively, because this specific formula involves a standard trigonometric function, we can also use the known bounds of sine and cosine to prove it.

We are given the range equation:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

For a specific projectile launch, the initial velocity ($v_0$) and the acceleration due to gravity ($g$) are constants. The only variable changing the range is the launch angle ($\theta$). Therefore, we want to maximize the function $R$ with respect to $\theta$.



---

### Method 1: The Trigonometric Approach (Logical Deduction)

**1. Isolate the variable component:**
In the formula $R(\theta) = \frac{v_0^2}{g} \cdot \sin(2\theta)$, the term $\frac{v_0^2}{g}$ is a positive constant. To make $R(\theta)$ as large as possible, we must make $\sin(2\theta)$ as large as possible.

**2. Identify the maximum value of the sine function:**
The sine of any angle always falls within the range of $-1$ to $1$. Therefore, the absolute maximum value that $\sin(2\theta)$ can output is exactly $1$.
$$\sin(2\theta) = 1$$

**3. Solve for the angle:**
We know from trigonometry that the sine of $90^\circ$ (or $\frac{\pi}{2}$ radians) is $1$.
$$2\theta = 90^\circ$$

Divide by 2:
$$\theta = 45^\circ$$

---

### Method 2: The Calculus Approach (First Derivative Test)

**1. Take the first derivative of the range function:**
To find the local maximums or minimums of a function, we take the derivative with respect to our variable ($\theta$) and set it equal to zero. 

Using the chain rule, the derivative of $\sin(2\theta)$ is $2\cos(2\theta)$.
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}[\sin(2\theta)]$$
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta)$$

**2. Set the derivative to zero:**
To find the critical point (where the slope of the function is flat, indicating a peak or valley), we set the equation to 0:
$$0 = \frac{2v_0^2}{g} \cos(2\theta)$$

**3. Solve for $\theta$:**
Since $v_0$ and $g$ are non-zero constants, the only way this equation can equal zero is if the cosine term itself equals zero:
$$\cos(2\theta) = 0$$

The cosine function equals zero at $90^\circ$ (and $270^\circ$, etc., but we are restricted to physical launch angles between $0^\circ$ and $90^\circ$).
$$2\theta = 90^\circ$$
$$\theta = 45^\circ$$

**4. Verify it is a maximum (Second Derivative Test):**
To prove this critical point is a *maximum* (and not a minimum), the second derivative must be negative.
$$\frac{d^2R}{d\theta^2} = \frac{d}{d\theta} \left[ \frac{2v_0^2}{g} \cos(2\theta) \right]$$
$$\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g} \sin(2\theta)$$

Plug in our critical point $\theta = 45^\circ$:
$$\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g} \sin(90^\circ) = -\frac{4v_0^2}{g} \cdot 1$$

Since $v_0^2$ and $g$ are always positive, the whole expression is negative. A negative second derivative confirms that $\theta = 45^\circ$ yields the absolute maximum range.

---
