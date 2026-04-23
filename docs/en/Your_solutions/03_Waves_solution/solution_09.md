## 1. General Solution
The motion of a damped harmonic oscillator is governed by the second-order linear differential equation:
$$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = 0$$

Dividing by the mass ($m$), we rewrite it in the standard form:
$$\frac{d^2x}{dt^2} + 2\gamma \frac{dx}{dt} + \omega_0^2x = 0$$

Where:
* **$\omega_0 = \sqrt{\frac{k}{m}}$**: The undamped natural angular frequency.
* **$\gamma = \frac{b}{2m}$**: The damping coefficient.

The characteristic equation is $r^2 + 2\gamma r + \omega_0^2 = 0$. The roots determine the system's behavior:
$$r_{1,2} = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}$$

---

## 2. Classification of Damping Cases
The behavior of the system depends on the relationship between $\gamma$ and $\omega_0$.

| Case | Condition | Physical Behavior |
| :--- | :--- | :--- |
| **Underdamped** | $\gamma < \omega_0$ | The system oscillates with a frequency $\omega_d = \sqrt{\omega_0^2 - \gamma^2}$, but the amplitude decays exponentially over time. |
| **Critically Damped** | $\gamma = \omega_0$ | The system returns to equilibrium in the shortest possible time without any oscillation. |
| **Overdamped** | $\gamma > \omega_0$ | The system returns to equilibrium without oscillating, but more slowly than in the critically damped case due to high resistance. |



---

## 3. Numerical Solution (RK4 Method)
To solve the equation numerically, we break the second-order ODE into a system of two first-order ODEs:
1.  $\frac{dx}{dt} = v$
2.  $\frac{dv}{dt} = -\frac{b}{m}v - \frac{k}{m}x$

The **Runge-Kutta 4th Order (RK4)** method calculates four intermediate slopes ($k_1$ through $k_4$) to estimate the next state $(x_{n+1}, v_{n+1})$ with high accuracy.

To solve this numerically, we convert this second-order ODE into a system of two first-order ODEs by introducing velocity ($v$):

1.  $$\\frac{dx}{dt} = v$$
2.  $$\\frac{dv}{dt} = \\frac{-bv - kx}{m}$$

We define our state vector as $y = [x, v]$ and our derivative function as $f(t, y) = [v, \\frac{-bv - kx}{m}]$.

---

## 2. The RK4 Algorithm
To find the state at the next time step $y_{n+1}$ from the current state $y_n$, we calculate four intermediate "slopes":

### Step 1: Calculate Slopes
* **$k_1 = f(t_n, y_n)$**
    * The slope at the beginning of the interval.
* **$k_2 = f(t_n + \\frac{h}{2}, y_n + \\frac{h}{2}k_1)$**
    * The slope at the midpoint using $k_1$.
* **$k_3 = f(t_n + \\frac{h}{2}, y_n + \\frac{h}{2}k_2)$**
    * The slope at the midpoint using $k_2$.
* **$k_4 = f(t_n + h, y_n + hk_3)$**
    * The slope at the end of the interval using $k_3$.

### Step 2: Weighted Average Update
The next state is calculated using a weighted average of these slopes:
$$y_{n+1} = y_n + \\frac{h}{6}(k_1 + 2k_2 + 2k_3 + k_4)$$

---

## 4. Investigating Parameter $b$
* **Low $b$:** Results in many oscillations before stopping. The phase portrait shows a **spiral** winding into the origin.
* **Increasing $b$:** Reduces the number of oscillations and the "size" of the spiral.
* **At $b = 2\sqrt{mk}$:** The system hits critical damping. The phase portrait becomes a direct path to the origin without circling it.
* **High $b$:** The "sluggish" return to equilibrium. The phase portrait shows a very slow approach to $(0,0)$.

---

## 5. Visualizing the Phase Portrait
The phase portrait plots velocity ($v$) on the y-axis against displacement ($x$) on the x-axis. 
* In an **undamped** system, this would be a perfect circle or ellipse (conservation of energy).
* In a **damped** system, energy is lost, so the trajectory spirals inward toward the equilibrium point $(0,0)$.
