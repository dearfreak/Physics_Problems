## Given Data
* **Resistor 1 ($R_1$):** $15\ \Omega$
* **Resistor 2 ($R_2$):** $30\ \Omega$
* **Resistor 3 ($R_3$):** $50\ \Omega$
* **Battery Voltage ($V$):** $12\text{ V}$

---

## Case 1: Series Connection

In a **series circuit**, resistors are connected end-to-end in a single line. Because there is only one path for the electricity to flow, the total resistance is simply the sum of all individual resistances.

### 1. Find Total Equivalent Resistance ($R_{\text{series}}$)
To find the total resistance, we add them all up:
$$R_{\text{series}} = R_1 + R_2 + R_3$$

$$R_{\text{series}} = 15\ \Omega + 30\ \Omega + 50\ \Omega = 95\ \Omega$$

### 2. Find Total Current ($I_{\text{series}}$)
Using [**Ohm's Law**](<img width="872" height="273" alt="image" src="https://github.com/user-attachments/assets/ad6a84d3-9e4c-4bc1-997f-1a69c0efcdc5" />
), the total current flowing from the battery is the battery voltage divided by the total resistance ($I = \frac{V}{R}$):
$$I_{\text{series}} = \frac{12\text{ V}}{95\ \Omega} \approx 0.126\text{ A}\ (126\text{ mA})$$

---

## Case 2: Parallel Connection

In a **parallel circuit**, each resistor is connected across the same two points, creating multiple separate paths for the current. Because electricity has more paths to choose from, the overall total resistance decreases.

### 1. Find Total Equivalent Resistance ($R_{\text{parallel}}$)
To find the total parallel resistance, we add the reciprocals (flipped versions) of each resistance, and then flip the final answer:
$$\frac{1}{R_{\text{parallel}}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$$

$$\frac{1}{R_{\text{parallel}}} = \frac{1}{15} + \frac{1}{30} + \frac{1}{50}$$

Let's find a common denominator (which is $150$):
$$\frac{1}{R_{\text{parallel}}} = \frac{10}{150} + \frac{5}{150} + \frac{3}{150} = \frac{18}{150}$$

Now, flip this fraction to find $R_{\text{parallel}}$:
$$R_{\text{parallel}} = \frac{150}{18} \approx 8.33\ \Omega$$

### 2. Find Total Current ($I_{\text{parallel}}$)
Using **Ohm's Law** again, the total current leaving the battery is the voltage divided by this new, lower total resistance:
$$I_{\text{parallel}} = \frac{12\text{ V}}{8.33\ \Omega} \approx 1.44\text{ A}$$

---

## Summary

| Connection Type | Total Equivalent Resistance | Current from Battery |
| :--- | :--- | :--- |
| **Series** | $95\ \Omega$ | $0.126\text{ A}$ |
| **Parallel** | $8.33\ \Omega$ | $1.44\text{ A}$ |
