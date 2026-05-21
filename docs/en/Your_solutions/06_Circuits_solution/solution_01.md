**Given Values:**
* $R_1 = 15 \\, \\Omega$
* $R_2 = 30 \\, \\Omega$
* $R_3 = 50 \\, \\Omega$
* Voltage ($V$) = **12 V**

---

### Case 1: Resistors in Series

When resistors are connected in series, the total equivalent resistance is simply the sum of all individual resistances. 

**1. Equivalent Resistance**
$$R_{eq} = R_1 + R_2 + R_3$$
$$R_{eq} = 15 + 30 + 50$$
$$R_{eq} = 95 \\, \\Omega$$

**2. Total Current**
Using Ohm's Law ($I = \\frac{V}{R}$), we divide the battery's voltage by the equivalent resistance to find the current flowing from the battery.
$$I_{series} = \\frac{12}{95}$$
$$I_{series} \\approx 0.126\\text{ A} \\quad \\text{(or 126 mA)}$$

---

### Case 2: Resistors in Parallel

When resistors are connected in parallel, the reciprocal of the total equivalent resistance is the sum of the reciprocals of each individual resistance.

**1. Equivalent Resistance**
$$\\frac{1}{R_{eq}} = \\frac{1}{R_1} + \\frac{1}{R_2} + \\frac{1}{R_3}$$
$$\\frac{1}{R_{eq}} = \\frac{1}{15} + \\frac{1}{30} + \\frac{1}{50}$$

To add these fractions, find the common denominator, which is 150:
$$\\frac{1}{R_{eq}} = \\frac{10}{150} + \\frac{5}{150} + \\frac{3}{150}$$
$$\\frac{1}{R_{eq}} = \\frac{18}{150}$$

Now, take the reciprocal to find $R_{eq}$:
$$R_{eq} = \\frac{150}{18}$$
$$R_{eq} \\approx 8.33 \\, \\Omega$$

**2. Total Current**
Again, use Ohm's Law with the parallel equivalent resistance. For the most precise result, use the exact fraction ($\\frac{150}{18}$) rather than the rounded decimal.
$$I_{parallel} = \\frac{V}{R_{eq}}$$
$$I_{parallel} = \\frac{12}{\\frac{150}{18}}$$
$$I_{parallel} = 12 \\cdot \\frac{18}{150}$$
$$I_{parallel} = \\frac{216}{150}$$
$$I_{parallel} = 1.44\\text{ A}$$

---

| Configuration | Equivalent Resistance ($R_{eq}$) | Total Current ($I$) |
| :--- | :--- | :--- |
| **Series** | **95 $\\Omega$** | **$\\approx$ 0.126 A** |
| **Parallel** | **$\\approx$ 8.33 $\\Omega$** | **1.44 A** |
