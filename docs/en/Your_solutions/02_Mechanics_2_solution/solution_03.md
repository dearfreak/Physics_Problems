## Pendulum

Given a pendulum with a length $L = 1.0 \, \text{m}$ released from an initial angle $\theta = 15^\circ$, we need to find its velocity $v$ at the lowest point of the swing.

## 1. Conservation of Energy Approach

To find the speed at the bottom, we use the principle of conservation of mechanical energy. The potential energy at the release height is converted into kinetic energy at the bottom.



### Step 1: Determine the vertical height ($h$)
The vertical height $h$ that the bob descends can be found using the length of the string and the release angle:
$$h = L - L\cos(\theta) = L(1 - \cos(\theta))$$

**Calculation:**
1.  **Convert angle if necessary:** $\theta = 15^\circ$
2.  **Plug in values:**
    $$h = 1.0 \cdot (1 - \cos(15^\circ))$$
    $$h \approx 1.0 \cdot (1 - 0.9659)$$
    $$h \approx 0.0341 \, \text{meters}$$

---

### Step 2: Equating Potential and Kinetic Energy
At the bottom of the swing, the potential energy ($mgh$) is zero, and the kinetic energy ($\frac{1}{2}mv^2$) is at its maximum.

$$mgh = \frac{1}{2}mv^2$$



The mass $m$ cancels out, allowing us to solve for $v$:
$$v = \sqrt{2gh}$$

**Calculation:**
1.  **Use $g \approx 9.81 \, \text{m/s}^2$:**
    $$v = \sqrt{2 \cdot 9.81 \cdot 0.0341}$$
2.  **Simplify:**
    $$v = \sqrt{0.669}$$
3.  **Result:**
    $$v \approx 0.818 \, \text{m/s}$$

**Answer:** The speed of the pendulum bob at the bottom of its swing is approximately **0.82 m/s**.
