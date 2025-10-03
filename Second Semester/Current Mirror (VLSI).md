In IC design, a reference current is generated at one location and mirrored to another part of the circuit to provide DC biasing currents required at different stages.

## Simple Current Mirror

In a simple current mirror:

- Two transistors, **M1** and **M2**, have their gates and sources connected together, so $V_{GS2} = V_{GS1}$.
- The transistor generating the reference current ($I_{in}$) is **diode-connected** (gate shorted to source).
- Both transistors must operate in **pinchoff** (saturation region).

**M1** is diode-connected and therefore in pinchoff. We must ensure that **M2** also remains in pinchoff. The current $I_{in}$ is then mirrored as $I_{out}$.

Since both transistors are in pinchoff:

$$
I_{in} = \frac{k'}{2} \left(\frac{W}{L}\right)_1 (V_{GS1} - V_T)^2 \quad \text{for M1}
$$

$$
I_{out} = \frac{k'}{2} \left(\frac{W}{L}\right)_2 (V_{GS2} - V_T)^2 \quad \text{for M2}
$$

For the current ratio:

$$
\frac{I_{out}}{I_{in}} = \frac{\left(\frac{W}{L}\right)_2}{\left(\frac{W}{L}\right)_1}
$$

since $V_{GS2} = V_{GS1}$ for ideal transistors.

> [!note]  
> In practice, channel-length modulation effects must be considered.

---

### Performance Characteristics of Current Mirrors

- The current ratio $I_{out}/I_{in}$ should depend only on the aspect ratios of the transistors.
- The AC output resistance should tend to infinity.
- The AC input resistance should tend to zero.
- $V_{min}$ should be as low as possible.

#### Effect of Channel-Length Modulation

For the simple current mirror, considering channel-length modulation:

For **M1**:
$$
I_{in} = \frac{k'}{2} \left(\frac{W}{L}\right)_1 (V_{GS1} - V_T)^2 (1 + \lambda V_{DS1})
$$

For **M2**:
$$
I_{out} = \frac{k'}{2} \left(\frac{W}{L}\right)_2 (V_{GS2} - V_T)^2 (1 + \lambda V_{DS2})
$$

Thus,
$$
\frac{I_{out}}{I_{in}} = \frac{\left(\frac{W}{L}\right)_2}{\left(\frac{W}{L}\right)_1} \cdot \frac{1 + \lambda V_{DS2}}{1 + \lambda V_{DS1}}
$$

**AC output resistance:**  
The AC output resistance of M2 ($r_{out}$) is approximately $r_{ds2}$.

**AC input resistance:**  
The AC input resistance of M1 (since M1 is diode-connected) is:
$$
r_{in} = \frac{1}{g_{m1}}
$$
Therefore, the AC input resistance is low.

**$V_{min}$:**  
The minimum voltage for M2 to remain in pinchoff (saturation) is:
$$
V_{DS2} \geq V_{GS2} - V_T
$$
So,
$$
V_{min} = V_{GS2} - V_T
$$
