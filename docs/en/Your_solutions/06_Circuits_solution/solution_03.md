To find the total (equivalent) resistance between the two main terminals at the bottom, we can break the circuit down step-by-step into simpler **series** and **parallel** sections.

---

### **Step 1: Simplify the Upper Left Path**
Look at the path starting from the middle-left junction, going up the left side, and turning right across the top to the upper-middle junction. 
* Since the current has only one path to flow through these two resistors, they are in **series**.
* **Calculation:** $$R_{\\text{top-left}} = 5\\,\\Omega + 5\\,\\Omega = 10\\,\\Omega$$

---

### **Step 2: Simplify the Inner Middle Path**
Now look at the inner path starting from that same middle-left junction, going right through the horizontal resistor, and then going up through the two vertical resistors.
* These three resistors are connected end-to-end in a single line, so they are also in **series**.
* **Calculation:** $$R_{\\text{inner}} = 5\\,\\Omega + 5\\,\\Omega + 5\\,\\Omega = 15\\,\\Omega$$

---

### **Step 3: Combine the Two Parallel Paths**
Notice that both the **Upper Left Path** ($10\\,\\Omega$) and the **Inner Middle Path** ($15\\,\\Omega$) start at the same left junction and meet at the same top-right junction. This means they are in **parallel**.
* To combine two parallel resistors, we multiply their values and divide by their sum:
* **Calculation:** $$R_{\\text{combined}} = \\frac{10 \\times 15}{10 + 15} = \\frac{150}{25} = 6\\,\\Omega$$

---

### **Step 4: Simplify the Far-Right Path**
Look at the branch on the far right containing two vertical resistors.
* These two resistors are in **series** with each other.
* **Calculation:** $$R_{\\text{right}} = 5\\,\\Omega + 5\\,\\Omega = 10\\,\\Omega$$

---

### **Step 5: Find the Total Upper Network Resistance**
The combined middle block ($6\\,\\Omega$ from Step 3) is connected directly in line with the far-right branch ($10\\,\\Omega$ from Step 4) as you move toward the right terminal. Therefore, they are in **series**.
* **Calculation:** $$R_{\\text{upper\\_network}} = 6\\,\\Omega + 10\\,\\Omega = 16\\,\\Omega$$

---

### **Step 6: Calculate the Final Equivalent Resistance**
Finally, the entire upper network ($16\\,\\Omega$) and the single horizontal resistor at the very bottom ($5\\,\\Omega$) are connected across the exact same two main external terminals. This makes them in **parallel**.
* **Calculation:** $$R_{\\text{eq}} = \\frac{16 \\times 5}{16 + 5} = \\frac{80}{21} \\approx 3.81\\,\\Omega$$

---

### **Final Answer**
The total equivalent resistance of the circuit is **$\\approx 3.81\\,\\Omega$** (or exactly $\\frac{80}{21}\\,\\Omega$).
[VISUAL](https://i.ibb.co/211SgdGT/image-2026-05-21-154628369.png)
