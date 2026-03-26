## 1. Projectile Motion
Given $v_0 = 100\text{ m/s}$, $\theta = 37^\circ$. (Approximations: $\sin 37^\circ \approx 0.6$, $\cos 37^\circ \approx 0.8$).

* **Differential Equations of Motion:**
    * Horizontal: $m\frac{d^2x}{dt^2} = 0 \implies a_x = 0$
    * Vertical: $m\frac{d^2y}{dt^2} = -mg \implies a_y = -g$
* **Time of Flight ($t_f$):** Found when $y(t) = 0$.
    $$t_f = \frac{2v_0\sin\theta}{g} = \frac{2 \cdot 100 \cdot 0.6}{9.81} \approx \mathbf{12.23\text{ s}}$$
* **Maximum Height ($H$):** Occurs when $v_y = 0$.
    $$H = \frac{(v_0\sin\theta)^2}{2g} = \frac{60^2}{19.62} \approx \mathbf{183.49\text{ m}}$$
* **Range ($R$):**
    $$R = (v_0\cos\theta)t_f = 80 \cdot 12.23 \approx \mathbf{978.4\text{ m}}$$



---

## 2. Range Optimization
The range formula is $R(\theta) = \frac{v_0^2\sin(2\theta)}{g}$. 
To find the maximum, we take the derivative with respect to $\theta$:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \cos(2\theta) \cdot 2 = 0$$
For this to be true, $\cos(2\theta) = 0$, which means $2\theta = 90^\circ$.
Therefore, **$\theta = 45^\circ$** yields the maximum range.

---

## 3. Path Intersection
* **Alice:** $x_A(t) = 2+t$, $y_A(t) = 8-3t$
* **Bob:** $x_B(t) = 2t-1$, $y_B(t) = 2t+2$

**Collision Check:** We need $x_A(t) = x_B(t)$ and $y_A(t) = y_B(t)$ at the same time $t$.
1.  $2+t = 2t-1 \implies t = 3\text{ s}$.
2.  Check $y$ at $t=3$: $y_A = 8 - 3(3) = -1$; $y_B = 2(3) + 2 = 8$.
Since $y_A \neq y_B$, they **do not collide**.

**Minimum Distance:** $D^2 = (x_A-x_B)^2 + (y_A-y_B)^2 = (3-t)^2 + (6-5t)^2$
$D^2 = 26t^2 - 66t + 45$. 
Setting the derivative to zero: $52t - 66 = 0 \implies \mathbf{t \approx 1.27\text{ s}}$.
$D_{min} = \sqrt{26(1.27)^2 - 66(1.27) + 45} \approx \mathbf{1.76\text{ m}}$.

---

## 4. Vector Calculus
$\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$
* **Velocity $\vec{v}(t)$:** $\frac{d\vec{r}}{dt} = \mathbf{(6t)\hat{i} + (5 - 16t)\hat{j}}$
* **Acceleration $\vec{a}(t)$:** $\frac{d\vec{v}}{dt} = \mathbf{6\hat{i} - 16\hat{j}}$ (Constant acceleration).

---

## 5. Relative Velocity
* **Direction:** To travel due North, the boat's eastward velocity component must cancel the river's flow ($2\text{ m/s}$ East).
    $\sin\theta = \frac{v_{river}}{v_{boat}} = \frac{2}{5} = 0.4$.
    $\theta = \arcsin(0.4) \approx \mathbf{23.58^\circ}$ **West of North**.
* **Time:** The resultant velocity North is $v_N = 5\cos(23.58^\circ) \approx 4.58\text{ m/s}$.
    $t = \frac{200\text{ m}}{4.58\text{ m/s}} \approx \mathbf{43.67\text{ s}}$.

---

## 6. Variable Velocity
$v(t) = t^2 + 2t - 5$ with $x(0) = 4$.
* **Acceleration:** $a(t) = \frac{dv}{dt} = 2t + 2$. At $t=3$, **$a(3) = 8\text{ m/s}^2$**.
* **Position:** $x(t) = \int (t^2 + 2t - 5) dt = \frac{1}{3}t^3 + t^2 - 5t + C$.
    $x(0) = 4 \implies C = 4$.
    $x(3) = \frac{1}{3}(27) + 9 - 15 + 4 = 9 + 9 - 15 + 4 = \mathbf{7\text{ m}}$.

---

## 7. Elimination of Time
$x(t) = 2t^2 \implies t = \sqrt{x/2}$
$y(t) = 3t^3 \implies y = 3(\sqrt{x/2})^3 = \mathbf{\frac{3}{2\sqrt{2}}x^{3/2}}$
* $\vec{v}(t) = (4t, 9t^2) \implies |\vec{v}(t)| = \mathbf{t\sqrt{16 + 81t^2}}$
* $\vec{a}(t) = (4, 18t) \implies |\vec{a}(t)| = \mathbf{\sqrt{16 + 324t^2}}$
* **Is acceleration constant?** **No**, it increases over time.

---

## 8. Circular Motion
$a_c = \frac{v^2}{R} = \omega^2 R$.
$\omega = \frac{2\pi}{24 \cdot 3600} \approx 7.27 \times 10^{-5}\text{ rad/s}$.
$R = 6,378,000\text{ m}$.
$a_c = (7.27 \times 10^{-5})^2 \cdot 6,378,000 \approx \mathbf{0.0337\text{ m/s}^2}$.

---

## 9. Momentum Comparison
$p = mv$.
* **Fly:** $0.002\text{ kg} \cdot 10\text{ m/s} = 0.02\text{ kg}\cdot\text{m/s}$
* **Tennis Ball:** $0.060\text{ kg} \cdot 1\text{ m/s} = 0.06\text{ kg}\cdot\text{m/s}$
The **tennis ball** has greater momentum.

---

## 10. Kinematics (Helix)
$\vec{r}(t) = (a\cos(\omega t), b\sin(\omega t), bt)$
* **Trajectory:** The $x$ and $y$ components form an ellipse ($\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$). Since $z$ increases linearly, it is an **elliptical helix**.
* **Path Length ($s$):**
    $s = \int_0^{t_0} \sqrt{(-a\omega\sin\omega t)^2 + (b\omega\cos\omega t)^2 + b^2} dt$
    If $a=b$, it simplifies to $s = \int_0^{t_0} \sqrt{b^2\omega^2 + b^2} dt = \mathbf{t_0\sqrt{b^2(\omega^2+1)}}$.
