
![[Pasted image 20251028141127.png]]

## Overview

The CMOS Miller OTA consists of **two stages**:
- **First stage:** Differential amplifier
- **Second stage:** Inverter amplifier

The load of the differential amplifier is the current mirror **M3, M4**. The DC biasing currents **I7** and **I5** are obtained via the current mirrors **M8, M5** and **M8, M7** respectively.

For stabilizing purposes (since there are three poles), a compensation capacitor $C_c$ is connected between the input to the second stage (output of the first stage) and the output of the second stage.

The compensation capacitor acts as a **Miller capacitor**, resulting in a dominant pole frequency response.

---

## Small Signal Analysis

### AC Voltage Gain ($A_v$)

$$
A_v = A_{v1} \times A_{v2}
$$

Where:
- $A_{v1}$ is the differential voltage gain of the first stage
- $A_{v2}$ is the AC voltage gain of the second stage

---

## AC Equivalent Circuit

### First Stage Gain ($A_{v1}$)

$$
A_{v1} = \frac{V_1}{V_{id}}
$$

$$
V_1 = -\left[g_{m1}\left(-\frac{v_{id}}{2}\right) + g_{m2}v_{gs4}\right](r_{ds2} \parallel r_{ds4})
$$

$$
v_{gs4} = v_{gs3}
$$

From the AC equivalent circuit:

$$
v_{gs4} = -g_{m1} \frac{v_{id}}{2} [r_{ds1} \parallel r_{ds3} \parallel \frac{1}{g_{m2}}]
$$

$$
= -g_{m1}\frac{v_{id}}{2} \cdot \frac{1}{g_{m3}}
$$

Replacing $v_{gs4}$ in the equation for $V_1$:

$$
\frac{V_1}{V_{id}} = \frac{g_{m2}}{g_{ds2} + g_{ds4}}
$$

---

### Second Stage Gain ($A_{v2}$)

$$
A_{v2} = -g_{m6}(r_{ds5} \parallel r_{ds6})
$$

$$
A_{v2} = -\frac{g_{m6}}{g_{ds5} + g_{ds6}}
$$

---

## Overall Voltage Gain

$$
A_v = \frac{-g_{m2}}{g_{ds2} + g_{ds4}} \cdot \frac{g_{m6}}{g_{ds5} + g_{ds6}}
$$

[[Frequency Response for the Miller OTA]]
