## Analysis of Functions

### a) $y(x,t) = A \cos(kx^2 - \omega t)$
To be a traveling wave, the argument must be in the form $(kx \pm \omega t)$. Here, the $x$ is squared ($x^2$).
* **Partial derivatives:** The second derivative with respect to $x$ will involve terms that depend on $x$, whereas the second derivative with respect to $t$ will not.
* **Conclusion:** This **cannot** describe a traveling wave because it does not satisfy the wave equation (the wave would change shape as it moves).

### b) $y(x,t) = A(x - vt)^2$
This function is in the form $f(u)$ where $u = x - vt$. Let's check the derivatives:
1.  **Space derivatives:**
    * $\frac{\partial y}{\partial x} = 2A(x-vt)$
    * $\frac{\partial^2 y}{\partial x^2} = 2A$
2.  **Time derivatives:**
    * $\frac{\partial y}{\partial t} = 2A(x-vt)(-v) = -2Av(x-vt)$
    * $\frac{\partial^2 y}{\partial t^2} = -2Av(-v) = 2Av^2$

**Check the wave equation:**
$$\frac{\partial^2 y}{\partial x^2} \stackrel{?}{=} \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}$$
$$2A = \frac{1}{v^2} (2Av^2)$$
$$2A = 2A$$
* **Conclusion:** This **can** describe a traveling wave (specifically a pulse that maintains its parabolic shape).

### c) $y(x,t) = A \log(x + vt)$
This is in the form $f(x + vt)$. 
* Any function of the form $f(x \pm vt)$ satisfies the wave equation, provided it is differentiable. While this satisfies the wave equation mathematically, it is physically limited because the value becomes undefined for $(x + vt) \le 0$. 
* **Conclusion:** Mathematically, it **can** describe a traveling wave in the region where the argument is positive.

---

## Final Result
The functions that can describe a traveling wave are **(b)** and **(c)**. 

> **Note:** Function **(b)** is the most common example of a non-sinusoidal traveling pulse. Function **(a)** fails because the spatial frequency changes with distance, meaning it is not a rigid translation of a shape.
