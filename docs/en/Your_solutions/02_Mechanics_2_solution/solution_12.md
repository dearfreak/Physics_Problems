Given constants:
* **Mass ($m$):** $2 \, \text{kg}$
* **Force ($\vec{F}$):** $[6, 2] \, \text{N}$
* **Initial Velocity ($\vec{v}(0)$):** $(1, -1) \, \text{m/s}$
* **Initial Position ($\vec{r}(0)$):** $(0, 0) \, \text{m}$

---

## 1. Determine $\vec{a}(t)$
Using Newton's Second Law ($\vec{F} = m\vec{a}$):
$$\vec{a} = \frac{\vec{F}}{m} = \frac{[6, 2]}{2}$$
**Answer:** $\vec{a}(t) = (3, 1) \, \text{m/s}^2$

---

## 2. Determine $\vec{v}(t)$
Velocity is the integral of acceleration: $\vec{v}(t) = \int \vec{a} \, dt + \vec{v}(0)$
$$\vec{v}(t) = (3t, t) + (1, -1)$$
**Answer:** $\vec{v}(t) = (3t + 1, t - 1) \, \text{m/s}$

---

## 3. Determine $\vec{r}(t)$
Position is the integral of velocity: $\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}(0)$
$$\vec{r}(t) = \left( \frac{3}{2}t^2 + t, \frac{1}{2}t^2 - t \right) + (0, 0)$$
**Answer:** $\vec{r}(t) = (1.5t^2 + t, 0.5t^2 - t) \, \text{m}$

---

## 4. Trajectory of Motion
The trajectory is a **parabola**. You can visualize this by plotting the $x$ and $y$ coordinates over time. Since both components are quadratic in $t$, the body moves in a curved path starting at the origin, initially dipping into the fourth quadrant before moving primarily in the direction of the force.


---

## 5. Calculate Work Done at $t = 3 \, \text{s}$
Work done by a constant force is $W = \vec{F} \cdot \Delta\vec{r}$.

1.  **Find position at $t = 3$:**
    $$\vec{r}(3) = (1.5(3)^2 + 3, 0.5(3)^2 - 3) = (13.5 + 3, 4.5 - 3) = (16.5, 1.5)$$
2.  **Calculate Dot Product:**
    $$W = [6, 2] \cdot (16.5, 1.5)$$
    $$W = (6 \cdot 16.5) + (2 \cdot 1.5) = 99 + 3 = 102 \, \text{J}$$

**Answer:** The work done is **$102$ J**.

---

## 6. Check Consistency with Work-Energy Theorem
The theorem states $W = \Delta K = K_f - K_i$.


1.  **Initial Kinetic Energy ($K_i$):**
    $$v(0)^2 = 1^2 + (-1)^2 = 2$$
    $$K_i = \frac{1}{2} m v(0)^2 = \frac{1}{2} (2)(2) = 2 \, \text{J}$$
2.  **Final Kinetic Energy at $t = 3$ ($K_f$):**
    $$\vec{v}(3) = (3(3) + 1, 3 - 1) = (10, 2)$$
    $$v(3)^2 = 10^2 + 2^2 = 104$$
    $$K_f = \frac{1}{2} m v(3)^2 = \frac{1}{2} (2)(104) = 104 \, \text{J}$$
3.  **Change in Kinetic Energy:**
    $$\Delta K = 104 - 2 = 102 \, \text{J}$$

**Conclusion:** Since $W = 102 \, \text{J}$ and $\Delta K = 102 \, \text{J}$, the results are **consistent**.
