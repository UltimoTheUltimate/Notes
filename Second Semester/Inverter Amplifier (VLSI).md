## Inverter Amplifier

The inverter amplifier consists of:

---

### DC Operation

Consider $V_{in}$ as it increases from 0V to $V_{DD}$ (typically $V_{DD} \approx 3V$ or $5V$).

- $M_1$ is n-channel, $M_2$ is p-channel.
- $g_{ds1} = \lambda_n I_D$
- $g_{ds2} = \lambda_p I_D$
- Voltage gain: $A_v = -\frac{\sqrt{2 K'_n (W/L)_1 I_D}}{(\lambda_n + \lambda_p) I_D}$
- $g_{m1} v_{gs1} = 0$

#### Key Voltages

- $V_{GS1} = V_{in}$
- $V_{out} = V_{DD} - V_{SD2}$
- $V_{out} = V_{DS1}$

#### When $V_{in} < V_T$ ($V_{GS1} < V_T$)
- $M_1$ is **OFF** $\rightarrow$ $I_D = 0$
- $V_{out} = V_{DD}$
- $V_{SD2} = 0V$

#### When $V_{in} = V_T^+$
- $V_{GS1} = V_T^+$
- $M_1$ switches **ON** and enters pinch-off ($V_{DS1} \equiv V_{out} \equiv V_{DD}$)
- Current $I_D$ starts to flow

#### As $V_{in}$ increases
- $V_{GS1}$ increases $\rightarrow$ $I_D$ increases
- "$I_D R$" drop across $M_2$ increases
- $V_{out} = V_{DD} - V_{SD2}$
- Both $M_1$ and $M_2$ are in pinch-off

#### As $V_{in} \rightarrow V_{DD}$
- $V_{out} \rightarrow$ a few mV
- $M_1$ enters the ohmic region

> The circuit is used when both $M_1$ and $M_2$ are in pinch-off (active region of the transfer characteristic).

---

## AC Analysis

Apply an AC signal $v_i$ at the gate of $M_1$ (the driving transistor).

**Key AC properties:**
- AC voltage gain ($A_v$)
- AC output resistance ($r_{out}$)

### AC Voltage Gain

From the AC equivalent circuit:

$$
A_v = \frac{v_o}{v_i}
$$

$$
v_o = -g_{m1} v_{gs1} (r_{ds1} \parallel r_{ds2})
$$

$$
v_i = v_{gs1}
$$

So,

$$
A_v = -g_{m1} (r_{ds1} \parallel r_{ds2})
$$

Where:

$$
r_{ds1} \parallel r_{ds2} = \frac{1}{g_{ds1} + g_{ds2}}
$$

$$
g_{ds1} = \lambda_n I_D
$$

$$
g_{ds2} = \lambda_p I_D
$$

($M_1$ is n-channel, $M_2$ is p-channel)

So:

$$
A_v = -\frac{g_{m1}}{g_{ds1} + g_{ds2}}
$$

In terms of design parameters:

$$
g_{m1} = \sqrt{2 K'_n \left(\frac{W}{L}\right)_1 I_D}
$$

So:

$$
A_v = -\frac{\sqrt{2 K'_n (W/L)_1 I_D}}{(\lambda_n + \lambda_p) I_D}
$$

---

### AC Output Resistance ($r_{out}$)

$r_{out}$ is the AC resistance from the output node to AC ground. To find $r_{out}$, short all external voltage sources ($v_{gs1} = 0$):

$$
g_{m1} v_{gs1} = 0
$$

So,

$$
r_{out} = r_{ds1} \parallel r_{ds2} = \frac{1}{g_{ds1} + g_{ds2}}
$$
