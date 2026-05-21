To find the currents $I_1$, $I_2$, and $I_3$, we use two fundamental rules of physics known as [**Kirchhoff's Laws**](https://www.electronicspecifier.com/wp-content/uploads/2025/11/AdobeStock_498668731.jpeg):

1. **Kirchhoff's Current Law (KCL):** Total current entering any junction must equal total current leaving it (what goes in must come out).
2. **Kirchhoff's Voltage Law (KVL):** The sum of all electrical potential differences (voltages) around any closed loop must equal zero.

---

### Step 1: Label the Current Directions

Let's define the paths and directions of the currents based on the circuit components:
- **$I_1$ (Left Branch):** Flows through the left loop containing $R_1$, ammeter $A$, and the battery $\mathcal{E}_1$. Let's assume it flows **clockwise**, coming out of the positive terminal of $\mathcal{E}_1$
- **$I_3$ (Right Branch):** Flows through the right loop containing the internal resistance $r_w$ and the battery $\mathcal{E}_2$. Let's assume it flows **clockwise**, coming out of the positive terminal of $\mathcal{E}_2$.
- **$I_2$ (Shared Center Branch):** Flows through the center resistor $R_2$. At the top junction, both $I_1$ and $I_3$ meet and flow downward together. Therefore, the downward current is:
  $$\text{Junction Equation: } I_2 = I_1 + I_3$$

---

### Step 2: Apply Voltage Law (KVL) to the Loops

When traversing a loop:
- Moving through a resistor in the direction of the current causes a voltage drop ($-$ value).
- Moving from the negative to the positive terminal of a battery causes a voltage boost ($+$ value).

#### **Left Loop (Traversing Counter-Clockwise):**
Starting from the bottom junction and going up through the left branch, then down through the center:
1. Boost from battery $\mathcal{E}_1$: $+4.5\text{ V}$
2. Drop across internal resistance $r_w$: $-(I_1 \times 1\ \Omega)$
3. Drop across top resistor $R_1$: $-(I_1 \times 20\ \Omega)$
4. Drop across middle resistor $R_2$: $-(I_2 \times 10\ \Omega)$

Equating the total loop voltage to zero:
$$4.5 - 1\cdot I_1 - 20\cdot I_1 - 10\cdot I_2 = 0$$
$$4.5 - 21I_1 - 10I_2 = 0 \implies 21I_1 + 10I_2 = 4.5$$

#### **Right Loop (Traversing Clockwise):**
Starting from the bottom junction and going up through the right branch, then down through the center:
1. Boost from battery $\mathcal{E}_2$: $+9\text{ V}$
2. Drop across internal resistance $r_w$: $-(I_3 \times 1\ \Omega)$
3. Drop across middle resistor $R_2$: $-(I_2 \times 10\ \Omega)$

Equating the total loop voltage to zero:
$$9 - 1\cdot I_3 - 10\cdot I_2 = 0 \implies I_3 + 10I_2 = 9$$

---

### Step 3: Solve the System of Equations

We now have three simple equations:
1. $I_2 = I_1 + I_3$
2. $21I_1 + 10I_2 = 4.5$
3. $I_3 + 10I_2 = 9 \implies I_3 = 9 - 10I_2$

Substitute $I_3$ from equation (3) into equation (1):
$$I_2 = I_1 + (9 - 10I_2)$$
$$11I_2 - 9 = I_1 \implies I_1 = 11I_2 - 9$$

Now, substitute this expression for $I_1$ into equation (2):
$$21(11I_2 - 9) + 10I_2 = 4.5$$
$$231I_2 - 189 + 10I_2 = 4.5$$
$$241I_2 = 193.5$$
$$I_2 = \frac{193.5}{241} \approx \mathbf{0.803\text{ A}}$$

---

### Step 4: Calculate $I_1$ and $I_3$

Using our value of $I_2 \approx 0.803\text{ A}$:

- **For $I_1$:**
  $$I_1 = 11(0.803) - 9 = 8.833 - 9 = \mathbf{-0.167\text{ A}}$$
  *(The negative sign simply means the actual current flows in the opposite direction to our initial assumption—so it actually flows clockwise).*

- **For $I_3$:**
  $$I_3 = 9 - 10(0.803) = 9 - 8.03 = \mathbf{0.967\text{ A}}$$

---

### Final Answers:
* **Current through $R_1$ ($I_1$):** $\mathbf{-0.167\text{ A}}$ (or $0.167\text{ A}$ flowing clockwise)
* **Current through $R_2$ ($I_2$):** $\mathbf{0.803\text{ A}}$ (flowing downward)
* **Current through $r_w$/$\mathcal{E}_2$ ($I_3$):** $\mathbf{0.967\text{ A}}$ (flowing clockwise)
