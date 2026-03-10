This is a **classic optimization problem in calculus**. We maximize the **area of a rectangle under a curve** using derivatives.

---

# Step 1: Understand the Geometry

The curve is:

[
y = 3 - x^2
]

We are working in the **first quadrant**, so:

[
x \ge 0, \quad y \ge 0
]

A rectangle is placed **under the curve**, with:

* one corner at the origin ((0,0))
* the upper-right corner on the curve.

So if the top-right corner is ((x,y)), then:

[
y = 3 - x^2
]

### Rectangle dimensions

* **Width** = (x)
* **Height** = (y = 3 - x^2)

---

# Step 2: Area Function

Area of rectangle:

[
A = \text{width} \times \text{height}
]

Substitute:

[
A(x) = x(3 - x^2)
]

Simplify:

[
A(x) = 3x - x^3
]

This is the **area function we want to maximize**.

---

# Step 3: Theory of Optimization

In calculus:

1. A **maximum or minimum** occurs at **critical points**
2. Critical points occur where

[
A'(x) = 0
]

or derivative is undefined.

Here the derivative exists everywhere, so we solve:

[
A'(x) = 0
]

---

# Step 4: Compute the Derivative

Differentiate:

[
A(x) = 3x - x^3
]

[
A'(x) = 3 - 3x^2
]

---

# Step 5: Find Critical Points

Set derivative equal to zero:

[
3 - 3x^2 = 0
]

Divide by 3:

[
1 - x^2 = 0
]

[
x^2 = 1
]

[
x = 1
]

(We only take **positive** value because first quadrant.)

---

# Step 6: Find the Height

Substitute (x=1) into the curve:

[
y = 3 - x^2
]

[
y = 3 - 1
]

[
y = 2
]

---

# Step 7: Dimensions of the Rectangle

* **Width** = (x = 1)
* **Height** = (y = 2)

---

# Step 8: Maximum Area

[
A = x \cdot y
]

[
A = 1 \cdot 2 = 2
]

---

# ✅ Final Answer

The rectangle with **maximum area** has dimensions:

[
\boxed{\text{Width} = 1, \quad \text{Height} = 2}
]

Maximum area:

[
\boxed{A_{\max} = 2}
]

---

✅ **Upper corner of rectangle:**
[
(1,2)
]

---


