## 1. Physical Principles
According to **Newton's Second Law**, the relationship between force, mass, and acceleration is:
$$\vec{F}(t) = m \vec{a}(t)$$

To solve for the particle's state, we follow this integration chain:
1.  **Acceleration:** $\vec{a}(t) = \frac{\vec{F}(t)}{m}$
2.  **Velocity:** $\vec{v}(t) = \int \vec{a}(t) dt$
3.  **Position:** $\vec{r}(t) = \int \vec{v}(t) dt$

---

## 2. Given Parameters
* **Mass ($m$):** $3 \text{ kg}$
* **Force Field ($\vec{F}$):** $(15t, 3t - 12, -6t^2) \text{ N}$
* **Initial Velocity ($\vec{v}_0$):** $(2, 0, 1) \text{ m/s}$ at $t = 0$
* **Initial Position ($\vec{r}_0$):** $(5, 2, -3) \text{ m}$ at $t = 0$

---

## 3. Step-by-Step Solution

### Step A: Find Acceleration $\vec{a}(t)$
Divide the force vector by the mass ($3 \text{ kg}$):
$$\vec{a}(t) = \frac{1}{3} (15t, 3t - 12, -6t^2)$$
$$\vec{a}(t) = (5t, \, t - 4, \, -2t^2) \text{ m/s}^2$$

### Step B: Find Velocity $\vec{v}(t)$
We integrate the acceleration components with respect to time $t$:
$$\vec{v}(t) = \int (5t, \, t - 4, \, -2t^2) dt$$
$$\vec{v}(t) = \left( \frac{5}{2}t^2 + C_{vx}, \, \frac{1}{2}t^2 - 4t + C_{vy}, \, -\frac{2}{3}t^3 + C_{vz} \right)$$

Using initial condition $\vec{v}(0) = (2, 0, 1)$:
* $x$: $0 + C_{vx} = 2 \Rightarrow C_{vx} = 2$
* $y$: $0 - 0 + C_{vy} = 0 \Rightarrow C_{vy} = 0$
* $z$: $0 + C_{vz} = 1 \Rightarrow C_{vz} = 1$

**Velocity Equation:**
$$\vec{v}(t) = \left( 2.5t^2 + 2, \quad 0.5t^2 - 4t, \quad -\frac{2}{3}t^3 + 1 \right) \text{ m/s}$$

### Step C: Find Position $\vec{r}(t)$
We integrate the velocity components with respect to time $t$:
$$\vec{r}(t) = \int \left( 2.5t^2 + 2, \, 0.5t^2 - 4t, \, -\frac{2}{3}t^3 + 1 \right) dt$$
$$\vec{r}(t) = \left( \frac{2.5}{3}t^3 + 2t + C_{rx}, \, \frac{0.5}{3}t^3 - 2t^2 + C_{ry}, \, -\frac{2}{12}t^4 + t + C_{rz} \right)$$

Using initial condition $\vec{r}(0) = (5, 2, -3)$:
* $x$: $0 + 0 + C_{rx} = 5 \Rightarrow C_{rx} = 5$
* $y$: $0 - 0 + C_{ry} = 2 \Rightarrow C_{ry} = 2$
* $z$: $0 + 0 + C_{rz} = -3 \Rightarrow C_{rz} = -3$

**Position Equation:**
$$\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \quad \frac{1}{6}t^3 - 2t^2 + 2, \quad -\frac{1}{6}t^4 + t - 3 \right) \text{ m}$$

---

## 4. Final Results Summary

| Vector | Dependence on Time ($t$) |
| :--- | :--- |
| **Velocity** $\vec{v}(t)$ | $(2.5t^2 + 2, \, 0.5t^2 - 4t, \, -0.67t^3 + 1)$ |
| **Position** $\vec{r}(t)$ | $(0.83t^3 + 2t + 5, \, 0.17t^3 - 2t^2 + 2, \, -0.17t^4 + t - 3)$ |
