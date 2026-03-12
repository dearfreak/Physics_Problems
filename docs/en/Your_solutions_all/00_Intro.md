# Section 0: Mathematical Foundations

---

Below it is just a copy of the tasks, so you can easily navigate to the task you want to solve. You can also use the links in the sidebar to navigate to the tasks.

## 1. Vector Algebra

Given two vectors in 3D space: $\vec{a} = [2, 1, -3]$ and $\vec{b} = [4, -2, 1]$. Calculate:

a) The magnitude of each vector. 

The magnitude is calculated using the formula: $|\vec{v}| = \sqrt{x^2 + y^2 + z^2}$

**Magnitude of $\vec{a}$:** $|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2} = \sqrt{4 + 1 + 9} = \sqrt{14} \approx 3.74$

**Magnitude of $\vec{b}$:** $|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2} = \sqrt{16 + 4 + 1} = \sqrt{21} \approx 4.58$



b) The dot product $\vec{a} \cdot \vec{b}$.

The dot product is the sum of the products of the components:

$$\vec{a} \cdot \vec{b} = (2 \cdot 4) + (1 \cdot -2) + (-3 \cdot 1)$$
$$\vec{a} \cdot \vec{b} = 8 - 2 - 3 = 3$$



c) The cross product $\vec{a} \times \vec{b}$.

| Component | Calculation | Result |
| :--- | :--- | :--- |
| **i** | $(1 \cdot 1) - (-3 \cdot -2)$ | $-5$ |
| **j** | $-((2 \cdot 1) - (-3 \cdot 4))$ | $-14$ |
| **k** | $(2 \cdot -2) - (1 \cdot 4)$ | $-8$ |

**Result:** $\vec{a} \times \vec{b} = [-5, -14, -8]$



d) The angle between vectors $\vec{a}$ and $\vec{b}$.

Using the formula $\cos(\theta) = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|}$:

**Cosine value:** $\cos(\theta) = \frac{3}{\sqrt{14} \cdot \sqrt{21}} \approx 0.175$

**Angle:** $\theta = \arccos(0.175) \approx 79.92^\circ$

## 2. Systems of Equations

Find the values of $x$ and $y$ that satisfy both equations: $2x + 3y = 12$ and $x - y = 1$.

$x - y = 1$ => $x = 1 + y$

$2(1+y) + 3y = 12$

$2 + 2y + 3y = 12$

$5y = 10$

$ y = 2 => x = 3$

## 3. Proportionality

Consider the Universal Law of Gravitation: $F = G \frac{m_1 m_2}{r^2}$, where $F$ is the gravitational force between two masses $m_1$ and $m_2$, $r$ is the distance between their centers, and $G$ is the gravitational constant. Determine the factor by which the force $F$ changes if the distance $r$ is *doubled* and both masses ($m_1$ and $m_2$) are *halved*.


$$F = G \frac{(\frac{1}{2}m_1)(\frac{1}{2}m_2)}{(2r)^2}$$
$$F = \left( \frac{1/4}{4} \right) \cdot G \frac{m_1 m_2}{r^2}$$
$$F = \frac{1}{16} F$$

The Gravitational force $F$ will change by a factor of **$1/16$** 

## 4. Rearranging Formulas

The formula for the period of a simple pendulum is $T = 2\pi \sqrt{\frac{L}{g}}$. Rearrange the equation give a formula for $g$ (acceleration due to gravity).

$$\frac{T}{2\pi} = \sqrt{\frac{L}{g}}$$
$$\left( \frac{T}{2\pi} \right)^2 = \frac{L}{g}$$
$$g \cdot \frac{T^2}{4\pi^2} = L$$
**$$g = \frac{4\pi^2 L}{T^2}$$**

## 5. Trigonometry

A vector $\vec{A}$ has a magnitude of $15$ and makes an angle of $\theta = 60^\circ$ with the horizontal axis. Calculate its horizontal and vertical components.

**Horizontal ($A_x$):** $|\vec{A}| \cos(\theta)$ $$A_x = 15 \cdot \cos(60^\circ)$$
$$A_x = 15 \cdot 0.5$$
$$A_x = 7.5$$

**Vertical ($A_y$):** $|\vec{A}| \sin(\theta)$

$$A_y = 15 \cdot \sin(60^\circ)$$
$$A_y = 15 \cdot \frac{\sqrt{3}}{2} \approx 15 \cdot 0.866$$
$$A_y \approx 12.99$$

## 6. Function Analysis

Consider the function $f(x) = 3x^2 - 12x + 7$. Identify any local maxima or minima.

1. Find the Critical Point
To find where the slope is zero, we take the first derivative $f'(x)$ and set it to $0$.

**First Derivative:**
$$f'(x) = 6x - 12$$

**Solving for $x$:**
$$6x - 12 = 0$$
$$6x = 12$$
$$x = 2$$


2. Determine the Nature of the Point
We use the **Second Derivative Test** to see if the point is a maximum or a minimum.

**Second Derivative:**
$$f''(x) = 6$$

* Since $f''(x) > 0$, the function is U-shaped.
* Therefore, the point at $x = 2$ is a local minimum.


3. Calculate the Minimum Value
Plug $x = 2$ back into the original function $f(x)$ to find the $y$-coordinate:

$$f(2) = 3(2)^2 - 12(2) + 7$$
$$f(2) = 12 - 24 + 7$$
$$f(2) = -5$$

No maxima due to function going infinetely up.

## 7. Logic & Series

A bicycle is 10 meters from a wall and moves towards it at a constant speed of $1\text{ m/s}$. A fly starts from the bicycle's front wheel and flies towards the wall at $2\text{ m/s}$. When it hits the wall, it instantly turns back and flies to the bicycle, and so on. What is the total distance the fly travels before being crushed?

It will take $10$ seconds $(10\text{ m}\cdot 1\text{ m/s})$ for bicycle to get to the wall.

And so the fly will be crushed in $10$ seconds because thats when bicycle will hit the wall.

$(10\text{ m}\cdot 2\text{ m/s})=20\text{ meters}$

## 8. Definite Integrals

Calculate the area under the curve of the function $f(x) = \sin(x)$ from $x=0$ to $x=\pi$.

$$Area = \int_{0}^{\pi} \sin(x) \, dx$$

Antiderivative:
The integral of $\sin(x)$ is $-\cos(x)$.
   $$\left[ -\cos(x) \right]_{0}^{\pi}$$


   $$(-\cos(\pi)) - (-\cos(0))$$
   $$-(-1) - (-1)$$
   $$1 + 1 = 2$$

## 9. Optimization Problem

A rectangle is under the curve $y = 3 - x^2$ in the first quadrant. What are the dimensions of the rectangle with the maximum area?

$A(x) = 3x - x^3$

$A'(x) = 3 - 3x^2$

$3 - 3x^2 = 0 => x = 1$

Width ($x$): $1$

Height ($y = 3 - 1^2$): $2$

Maximum Area: $2$

## 10. Infinite Series

Determine the final position of an ant that starts at the origin and moves according to the following pattern: 1 m east, 1/2 m north, 1/3 m west, 1/4 m south, 1/5 m east, and so on.

Pattern: $1$ E, $1/2$ N, $1/3$ W, $1/4$ S, $1/5$ E ...



The series for East/West movement is:

$x = 1 - \frac{1}{3} + \frac{1}{5} - \dots$

This matches the expansion for $arctan(1)$:

$x = \frac{\pi}{4} \approx 0.785\text{ m}$


The series for North/South movement is:

$y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \dots$

Factoring out $1/2$ gives $\frac{1}{2}(1 - \frac{1}{2} + \frac{1}{3} - \dots)$, which is $\frac{1}{2}\ln(2)$:

$y = \frac{\ln(2)}{2} \approx 0.347\text{ m}$ 


The ant ends at coordinates $(\frac{\pi}{4}, \frac{\ln(2)}{2}) \approx (0.785, 0.347)$
