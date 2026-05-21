When combining exactly three $1\\,\\Omega$ resistors, there are four distinct circuit configurations you can build.

---

* **Series Connection:** Resistors are connected end-to-end in a line. The total resistance is found by adding them together.
* **Parallel Connection:** Resistors are connected side-by-side across the same two points. The total resistance decreases because current has multiple paths to flow through.

---

### 1. All Three in Series
[All three resistors are connected end-to-end in a single line.](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsEECsqYIiSeATAVQOx0DM2AHFQGwCcndqIARoiLZUAB0EIALI1QA3CENQBbTEICmAWiQoAfACgoUYLKgAPRBvaSojdiyiXrSdiNgV2qAO7wErpQENTWUUAen1DYGhzBEcoZ2woFgT41B9XBWRCBDCDIyjEJLiXKBp7FLdfVAzKAmzwvLNEUqKExhoW1JwqiiyciM9GhDbk4uGbO07KvqMB6LHbe1iFyZEc4BDwCH0gA) 

* **Explanation:** Since the electricity must flow through each resistor one after the other, you simply add the resistance values together.
* **Calculation:** $$R_{\\text{eq}} = 1\\,\\Omega + 1\\,\\Omega + 1\\,\\Omega = 3\\,\\Omega$$

### 2. All Three in Parallel
[All three resistors are connected side-by-side across the same two common nodes.](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsEECsqYIiSeATAVQOx0DM2AHFQGwCcndqIARoiLZUAB0EIALI1QA3CENQBbTEICmAWiQoAfACgoUYNAAeiFtihIqLKPSpWbqeAhFQFyQggD0+w8agzBAsrTgd7UKpnHFQPSgIfPyNTc0sqInY7OnCM6NdYii9fAyMAd0DUx1sQpDC8kWL-cqCasKgQ9PZ6xJLgZsQI61tButgYxrKKhBHw7LtcsfyJvqmOjPbLRhpu5dlVzZoshy23FyQuqFKXNyUAQxNZRWX+6bnOo6gTnf1gb3AIfRAA)

* **Explanation:** Because there are three identical, equal paths for the current to take, flowing through the circuit becomes three times easier than through a single resistor. Thus, the total resistance is one-third of a single resistor.
* **Calculation:** $$\\frac{1}{R_{\\text{eq}}} = \\frac{1}{1\\,\\Omega} + \\frac{1}{1\\,\\Omega} + \\frac{1}{1\\,\\Omega} = 3 \\implies R_{\\text{eq}} = \\frac{1}{3}\\,\\Omega \\approx 0.33\\,\\Omega$$

### 3. Two in Parallel, with One in Series
[Two resistors are wired side-by-side (in parallel), and this pair is connected in line (in series) with the third resistor.](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsEECsqYIiSeATAVQOx0DM2AHFQGwCcndqIARoiLZUAB0EIALI1QA3CENQBbTEICmAWiQoAfACgoUYNAAeiDYypQkddtaRWb7VPAQioC5IQQB6fYeMoMwQLK3pHByhwlxxUT0oCX38jUwpIqipJKMlsKMyYtziKbz8DIwB3ILTHW3sw-NhY0oDK4O16rPaouioCkWaKqpDLbqtQ61s+pLLgWSHM3MYiMZGl3sbkZyhy13clAEMTWUUB4FbEBbysy7Wp0-PhsJ6ocduN-v1gH3AIfSA)

* **Explanation:** First, find the combined resistance of the parallel pair. Since they are identical and side-by-side, their resistance halves to $0.5\\,\\Omega$. Then, add the third resistor that sits in line with them.
* **Calculation:** * Parallel pair: $R_{\\text{parallel}} = \\frac{1\\,\\Omega \\times 1\\,\\Omega}{1\\,\\Omega + 1\\,\\Omega} = 0.5\\,\\Omega$
  * Total resistance: $R_{\\text{eq}} = 0.5\\,\\Omega + 1\\,\\Omega = 1.5\\,\\Omega$ (or $\\frac{3}{2}\\,\\Omega$)

### 4. Two in Series, with One in Parallel
[Two resistors are connected end-to-end (in series) to form a $2\\,\\Omega$ branch, and this entire branch is placed side-by-side (in parallel) with the remaining third resistor.](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsEECsqYIiSeATAVQOx0DM2AHFQGwCcndqIARoiLZUAB0EIALI1QA3CENQBbTEICmAWiQoAfACgoUYNAAeOKEiosLli1dTwEIqAuSEEAen2HjUM8ltLaypJbDsWBxxUV0oCT28jU3MqEKgQsJTJSKdoincvAyMAdz9EdPC00LSQ7JECnxL-MKCoDJrYKPri0qdqyVaoRhpa+MLgWR6woYyq6eykdlQix2clAEMTWUUu4EayqszKqeGOnILgD3AIfSA)

* **Explanation:** First, combine the two resistors in series, which gives $2\\,\\Omega$. Now you have a $2\\,\\Omega$ branch in parallel with a single $1\\,\\Omega$ resistor. 
* **Calculation:** $$R_{\\text{eq}} = \\frac{R_{\\text{branch}} \\times R_3}{R_{\\text{branch}} + R_3} = \\frac{2\\,\\Omega \\times 1\\,\\Omega}{2\\,\\Omega + 1\\,\\Omega} = \\frac{2}{3}\\,\\Omega \\approx 0.67\\,\\Omega$$
