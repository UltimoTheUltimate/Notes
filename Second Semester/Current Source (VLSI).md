In general, a DC current source is required to provide the biasing current for the transistors in an IC.

![[insert-image-here.png]]

The ideal current source provides a constant DC biasing current, independent of the load.

Two important characteristics of an ideal current source are:

- **Minimum DC voltage ($V_\text{min}$)** across the current source. Typically, the output DC voltage $V_{DS}$ should be as low as possible. $V_\text{min}$ is the lowest possible output voltage for which the transistor remains in pinchoff.
- **AC output resistance** should ideally be infinite.

---

### Minimum DC Voltage ($V_\text{min}$)

The condition for pinchoff is:

$$
V_{DS} \geq V_{GS} - V_T
$$

$V_\text{min}$ occurs at the limit:

$$
V_{DS} = V_{GS} - V_T = V_\text{min}
$$

---

### AC Output Resistance ($r_\text{out}$)

Draw the AC equivalent circuit:  
![[insert-ac-equivalent-circuit.png]]

To find the AC output resistance, short-circuit external voltage sources (i.e., $v_{gs} = 0$), so $g_m v_{gs} = 0$.  
What remains is:

$$
r_\text{out} = r_{ds}
$$

---

To increase AC output resistance, negative feedback can be used. A resistance $R$ is connected between the source terminal and ground.

![[insert-feedback-resistor-image.png]]

To find the new $R_\text{out}$, draw the AC equivalent circuit:  
![[insert-new-ac-equivalent-circuit.png]]

Apply a voltage source $v_x$ at the output and find the current $i_x$ drawn by the circuit, with these conditions:

1. Short-circuit external voltage sources
2. Open-circuit external current sources

Then,

$$
r_\text{out} = \frac{v_x}{i_x}
$$

From the circuit:

$$
v_x = (i_x - g_m v_{gs}) r_{ds} + i_x R
$$

But $v_{sg} = i_x R$, so $v_{gs} = -i_x R$.

Therefore,

$$
v_x = [i_x + g_m i_x R] r_{ds} + i_x R \\
v_x = i_x (1 + g_m R) r_{ds} + i_x R
$$

So,

$$
r_\text{out} = \frac{v_x}{i_x} = (1 + g_m R) r_{ds} + R
$$

Assuming $r_{ds} \gg R$:

$$
r_\text{out} \approx (1 + g_m R) r_{ds}
$$
