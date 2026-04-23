When two waves of the same frequency and amplitude travel in opposite directions, they interfere to form a standing wave.

## 1. Derivation of the Standing Wave Equation
Given the two wave equations:
* $y_1(x,t) = A \sin(kx - \omega t)$ (Right-traveling wave)
* $y_2(x,t) = A \sin(kx + \omega t)$ (Left-traveling wave)

Where:
* **$A$** = Amplitude
* **$k$** = Wave number ($k = \frac{2\pi}{\lambda}$)
* **$\omega$** = Angular frequency ($\omega = 2\pi f$)

Using the trigonometric identity:
$$\sin(\alpha) + \sin(\beta) = 2 \sin\left(\frac{\alpha + \beta}{2}\right) \cos\left(\frac{\alpha - \beta}{2}\right)$$

Let $\alpha = kx + \omega t$ and $\beta = kx - \omega t$:
* $\frac{\alpha + \beta}{2} = \frac{(kx + \omega t) + (kx - \omega t)}{2} = kx$
* $\frac{\alpha - \beta}{2} = \frac{(kx + \omega t) - (kx - \omega t)}{2} = \omega t$

**The resulting standing wave equation is:**
$$y(x,t) = [2A \sin(kx)] \cos(\omega t)$$



---

## 2. Identifying the Positions of the Nodes
**Nodes** are points where the displacement is always zero ($y = 0$). For this to happen, the spatial part of the equation must equal zero:
$$\sin(kx) = 0$$

This occurs when the argument $kx$ is an integer multiple of $\pi$:
$$kx = n\pi \quad \text{where } n = 0, 1, 2, 3, \dots$$

Since $k = \frac{2\pi}{\lambda}$, we can solve for $x$:
$$\left(\frac{2\pi}{\lambda}\right)x = n\pi$$
$$x = n \frac{\lambda}{2}$$

**Positions of the nodes:**
Nodes occur at $x = 0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}, \dots$

---

## Summary Table

| Feature | Description | Condition |
| :--- | :--- | :--- |
| **Equation** | $y(x,t) = 2A \sin(kx) \cos(\omega t)$ | Result of superposition |
| **Amplitude** | $2A \sin(kx)$ | Varies with position $x$ |
| **Nodes** | Points of zero motion | $x = n \frac{\lambda}{2}$ |
