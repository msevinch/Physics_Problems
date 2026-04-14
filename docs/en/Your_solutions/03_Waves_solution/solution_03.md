
This problem perfectly illustrates how two traveling waves—one moving left, one moving right—interact to create a wave that appears to stand perfectly still.

### The Underlying Theory: Superposition
The Principle of Superposition states that when two or more waves occupy the same space at the same time, the total displacement at any point is simply the algebraic sum of the displacements of the individual waves. 

Mathematically, we express this as:
$$y_{total}(x,t) = y_1(x,t) + y_2(x,t)$$

We are given two identical waves traveling in opposite directions:
* $y_1(x,t) = A\sin(kx - \omega t)$  (traveling to the right)
* $y_2(x,t) = A\sin(kx + \omega t)$  (traveling to the left)

---

### Step 1: Setting Up the Equation
To find the resulting wave, we add the two equations together:
$$y(x,t) = A\sin(kx - \omega t) + A\sin(kx + \omega t)$$

To combine these terms, we need to use a standard trigonometric identity for the sum of two sine functions:
$$\sin(\alpha) + \sin(\beta) = 2\sin\left(\frac{\alpha + \beta}{2}\right)\cos\left(\frac{\alpha - \beta}{2}\right)$$

---

### Step 2: Applying the Trigonometric Identity
Let's define our $\alpha$ and $\beta$ from our wave equations:
* $\alpha = kx - \omega t$
* $\beta = kx + \omega t$

Now, let's calculate the two parts of our identity:

**1. The Sine part (addition):**
$$\frac{\alpha + \beta}{2} = \frac{(kx - \omega t) + (kx + \omega t)}{2}$$
$$\frac{\alpha + \beta}{2} = \frac{2kx}{2} = kx$$

**2. The Cosine part (subtraction):**
$$\frac{\alpha - \beta}{2} = \frac{(kx - \omega t) - (kx + \omega t)}{2}$$
$$\frac{\alpha - \beta}{2} = \frac{-2\omega t}{2} = -\omega t$$

---

### Step 3: The Standing Wave Equation
Now we substitute these simplified parts back into our trigonometric identity, remembering to include our original amplitude $A$:
$$y(x,t) = 2A\sin(kx)\cos(-\omega t)$$

Because cosine is an even function, meaning $\cos(-\theta) = \cos(\theta)$, we can drop the negative sign to clean up the equation:
$$y(x,t) = 2A\sin(kx)\cos(\omega t)$$

**This is the equation of the resulting standing wave.** Notice how it separates the space component ($\sin(kx)$) from the time component ($\cos(\omega t)$). The wave is no longer moving forward or backward; instead, every point $x$ oscillates in place with an amplitude of $2A\sin(kx)$.

---

### Step 4: Identifying the Nodes
Nodes are specific positions on a standing wave that **never move**. Their displacement is always zero, regardless of the time $t$. 

For $y(x,t)$ to always equal zero, the spatial part of the amplitude must be zero:
$$\sin(kx) = 0$$

The sine function equals zero whenever its argument is an integer multiple of $\pi$. Therefore:
$$kx = n\pi$$ 
*(where $n = 0, 1, 2, 3, \dots$)*

Now, we solve for position $x$:
$$x = \frac{n\pi}{k}$$

To make this physically intuitive, we can express the wave number ($k$) in terms of wavelength ($\lambda$). The definition of the wave number is $k = \frac{2\pi}{\lambda}$. Substituting this in:
$$x = \frac{n\pi}{\frac{2\pi}{\lambda}}$$
$$x = \frac{n\lambda}{2}$$

### Final Summary
* **The Standing Wave Equation:** $y(x,t) = 2A\sin(kx)\cos(\omega t)$
* **The Positions of the Nodes:** Nodes occur at $x = 0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}, \dots$ (every half-wavelength along the medium).
