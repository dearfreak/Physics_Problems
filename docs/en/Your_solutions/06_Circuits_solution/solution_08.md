To find the voltage equation across the resistor, we can look at how current and voltage behave together in a simple circuit.

### 1. Understanding the Given Information
We are given two pieces of information about our alternating current (AC) circuit:
* **The Current Equation:** <span class="math">I(t) = 2\sin(120\pi t)</span>. This tells us how the electrical current flows back and forth over time. The number **2** before the sine function represents the peak current (<span class="math">I_{max}</span>).
* **The Resistance:** <span class="math">R = 50\ \Omega</span>. This is the measure of how much the resistor opposes the flow of current.

### 2. The Relationship Between Voltage and Current
In a purely resistive AC circuit (a circuit with only a resistor), the voltage and the current are perfectly in sync. This means that when the current reaches its maximum value, the voltage does too. 

Because they change together in the exact same pattern, the voltage equation will have the exact same mathematical shape as the current equation—specifically, it will also use <span class="math">\sin(120\pi t)</span>. 

To connect the actual values of voltage and current, we use **Ohm's Law**. This fundamental law states that voltage (<span class="math">V</span>) is always equal to the current (<span class="math">I</span>) multiplied by the resistance (<span class="math">R</span>):

<div style="text-align:center; margin:1em 0; font-size:1.1em;"><span class="math">V = I \times R</span></div>

### 3. Calculating the Peak Voltage
To find the maximum or peak voltage (<span class="math">V_{max}</span>) across the resistor, we simply multiply the peak current by the resistance:

<div style="text-align:center; margin:1em 0; font-size:1.1em;"><span class="math">V_{max} = I_{max} \times R</span></div>
<div style="text-align:center; margin:1em 0; font-size:1.1em;"><span class="math">V_{max} = 2\text{ A} \times 50\ \Omega = 100\text{ V}</span></div>

### 4. Writing the Final Equation
Now we can construct our final voltage equation <span class="math">V(t)</span>. We take the peak voltage we just calculated (100) and pair it with the exact same time-dependent sine wave from our current equation:

<div style="text-align:center; margin:1em 0; font-size:1.1em;"><span class="math">V(t) = 100\sin(120\pi t)</span></div>

**Final Answer:**
The equation for the voltage across the resistor is **<span class="math">V(t) = 100\sin(120\pi t)</span>** (measured in Volts).
