When combining exactly three $1\\,\\Omega$ resistors, there are four distinct circuit configurations you can build. Here is a breakdown of each configuration and its resulting total (equivalent) resistance.

---

### Core Concepts Reminder
* **Series Connection:** Resistors are connected end-to-end in a line. The total resistance is found by adding them together.
* **Parallel Connection:** Resistors are connected side-by-side across the same two points. The total resistance decreases because current has multiple paths to flow through.

---

### 1. All Three in Series
All three resistors are connected end-to-end in a single line. 

* **Explanation:** Since the electricity must flow through each resistor one after the other, you simply add the resistance values together.
* **Calculation:** $$R_{\\text{eq}} = 1\\,\\Omega + 1\\,\\Omega + 1\\,\\Omega = 3\\,\\Omega$$

### 2. All Three in Parallel
All three resistors are connected side-by-side across the same two common nodes.

* **Explanation:** Because there are three identical, equal paths for the current to take, flowing through the circuit becomes three times easier than through a single resistor. Thus, the total resistance is one-third of a single resistor.
* **Calculation:** $$\\frac{1}{R_{\\text{eq}}} = \\frac{1}{1\\,\\Omega} + \\frac{1}{1\\,\\Omega} + \\frac{1}{1\\,\\Omega} = 3 \\implies R_{\\text{eq}} = \\frac{1}{3}\\,\\Omega \\approx 0.33\\,\\Omega$$

### 3. Two in Parallel, with One in Series
Two resistors are wired side-by-side (in parallel), and this pair is connected in line (in series) with the third resistor.

* **Explanation:** First, find the combined resistance of the parallel pair. Since they are identical and side-by-side, their resistance halves to $0.5\\,\\Omega$. Then, add the third resistor that sits in line with them.
* **Calculation:** * Parallel pair: $R_{\\text{parallel}} = \\frac{1\\,\\Omega \\times 1\\,\\Omega}{1\\,\\Omega + 1\\,\\Omega} = 0.5\\,\\Omega$
  * Total resistance: $R_{\\text{eq}} = 0.5\\,\\Omega + 1\\,\\Omega = 1.5\\,\\Omega$ (or $\\frac{3}{2}\\,\\Omega$)

### 4. Two in Series, with One in Parallel
Two resistors are connected end-to-end (in series) to form a $2\\,\\Omega$ branch, and this entire branch is placed side-by-side (in parallel) with the remaining third resistor.

* **Explanation:** First, combine the two resistors in series, which gives $2\\,\\Omega$. Now you have a $2\\,\\Omega$ branch in parallel with a single $1\\,\\Omega$ resistor. 
* **Calculation:** $$R_{\\text{eq}} = \\frac{R_{\\text{branch}} \\times R_3}{R_{\\text{branch}} + R_3} = \\frac{2\\,\\Omega \\times 1\\,\\Omega}{2\\,\\Omega + 1\\,\\Omega} = \\frac{2}{3}\\,\\Omega \\approx 0.67\\,\\Omega$$

---

### Summary of Unique Equivalent Resistance Values

The four unique equivalent resistance values you can create using exactly three $1\\,\\Omega$ resistors are:

1. **$\\frac{1}{3}\\,\\Omega$** (or $0.33\\,\\Omega$)
2. **$\\frac{2}{3}\\,\\Omega$** (or $0.67\\,\\Omega$)
3. **$\\frac{3}{2}\\,\\Omega$** (or $1.5\\,\\Omega$)
4. **$3\\,\\Omega$**
