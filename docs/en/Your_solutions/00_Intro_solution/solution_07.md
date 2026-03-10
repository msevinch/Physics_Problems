# 7. Logic & Series

This document outlines the solution to a classic mathematical puzzle involving relative motion and infinite series.

---

## 1. Theory and Concepts

**The "Time" Approach vs. The Infinite Series**
This famous problem is designed to trick you into setting up a complex infinite geometric series (calculating the distance of the fly's first trip to the wall, then the return trip to the moving bike, and so on). However, there is a much simpler, logical approach:
1.  Determine the **total time** the bicycle is in motion before it hits the wall.
2.  Since the fly is in continuous motion for that exact same duration, you can calculate the fly's total distance by simply multiplying its constant speed by that total time.



### Fundamental Formula
For an object moving at a constant velocity, distance is the product of velocity and time:
$$d = v \cdot t$$

---

## 2. Step-by-Step Determination

**Given Data:**
* Initial distance to the wall ($D$) = **10 m**
* Velocity of the bicycle ($v_b$) = **1 m/s**
* Velocity of the fly ($v_f$) = **2 m/s**

### Step 1: Calculate total time
Find out how long it takes for the bicycle to reach the wall.
$$t = \frac{D}{v_b}$$
$$t = \frac{10}{1} = \mathbf{10 \text{ s}}$$
*(The bicycle travels for exactly 10 seconds before hitting the wall.)*

### Step 2: Calculate the fly's total distance
The fly is flying at a constant speed of **2 m/s** for those entire **10 seconds**, regardless of how many times it turns around.
$$d_f = v_f \cdot t$$
$$d_f = 2 \cdot 10 = \mathbf{20 \text{ m}}$$

---

## 3. Summary Table

| Entity | Speed | Time in Motion | Total Distance |
| :--- | :--- | :--- | :--- |
| **Bicycle** | **1 m/s** | **10 s** | **10 m** |
| **Fly** | **2 m/s** | **10 s** | **20 m** |

**Conclusion:** The fly travels a total distance of **20 meters** before the bicycle reaches the wall.
