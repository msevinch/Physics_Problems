# Systems of Equations: Theory and Step-by-Step Solution

This document outlines the process of solving a system of two linear equations with two variables:
1.  **Equation 1:** $2x + 3y = 12$
2.  **Equation 2:** $x - y = 1$

---

## 1. Underlying Theory

### Linear Systems
A **System of Equations** is a set of two or more equations with the same variables. To "solve" the system means finding the values of the variables that make **all** equations true simultaneously.

### Graphical Interpretation
On a 2D Cartesian plane, each equation represents a straight line. The solution to the system is the **intersection point** $(x, y)$ where the two lines meet.



---

## 2. Methodology: The Substitution Method

While there are several ways to solve this (Elimination, Graphing, or Matrix Algebra), we will use the **Substitution Method**. This involves expressing one variable in terms of the other and "plugging" it into the second equation.

### Formula Context
For a general system:
1.  $a_1x + b_1y = c_1$
2.  $a_2x + b_2y = c_2$

We isolate $x$ in equation (2): $x = \frac{c_2 - b_2y}{a_2}$ and substitute it into equation (1).

---

## 3. Step-by-Step Determination

### Step 1: Isolate one variable
Let's take the simpler equation, **Equation 2**, and solve for $x$:
$$x - y = 1$$
$$x = y + 1$$

### Step 2: Substitute into the other equation
Now, we take our new definition of $x$ and substitute it into **Equation 1**:
$$2(y + 1) + 3y = 12$$

### Step 3: Solve for $y$
Expand the brackets and combine like terms:
$$2y + 2 + 3y = 12$$
$$5y + 2 = 12$$
$$5y = 10$$
$$\mathbf{y = 2}$$

### Step 4: Solve for $x$
Now that we know $y = 2$, plug it back into our isolated equation from Step 1:
$$x = 2 + 1$$
$$\mathbf{x = 3}$$

---

## 4. Verification

To ensure the solution is correct, we substitute $(3, 2)$ back into both original equations:
* **Eq 1:** $2(3) + 3(2) = 6 + 6 = 12$ (Correct ✅)
* **Eq 2:** $3 - 2 = 1$ (Correct ✅)

---

## Summary Table

| Variable | Value |
| :--- | :--- |
| **$x$** | $3$ |
| **$y$** | $2$ |
| **Intersection Point** | $(3, 2)$ |
