![[Pasted image 20251014131956.png]]

Consider the differential amplifier circuit, consisting of 2 matched transistors M1 and M2 with their sources connected together, and having matched loads. The transistors are DC biased by a current $I_B$ provided by a current sink M7.

Two signals $V_{I1}$ and $V_{I2}$ are applied at the gate of M1, M2 respectively.

> **Note:** $V_{I1}$ and $V_{I2}$ will have both a useful AC signal $v_i$ and a noise signal, the common mode signal $V_{CM}$.

Assuming perfect ideal matching between the left hand side and the right hand side, the DC biasing current in both sides should be $I_B/2$.

Two input signals $v_{I1}$ and $v_{I2}$ can be composed into a differential signal $V_{ID}$ and a common mode signal $V_{CM}$, where:

- $$ V_{ID} = V_{I1} - V_{I2} $$
- $$ V_{CM} = \frac{V_{I1} + V_{I2}}{2} $$

The objective of a differential amplifier is to amplify the differential signal and reject the common mode signal.

The common-mode rejection ratio (CMRR) is the ratio between the differential voltage gain and the common mode voltage gain $A_{CM}$:

- $$ \text{CMRR} = \frac{A_{vd}}{A_{cm}} $$

which ideally is $\infty$ since $A_{CM} = 0$. For a general purpose opamp, the CMRR is about 60dB to 80dB.

The differential amplifier has the possibility of 2 outputs: $v_{o1}$ and $v_{o2}$. The output from a differential amplifier can be either single-ended (i.e. $v_{o1}$ or $v_{o2}$) or differential, where 

$$ v_{od} = v_{o1} - v_{o2} $$

---

#### Example of single-ended output

The opamp:

![[Pasted image 20251014134144.png]]

#### Example of a differential output

The differential opamp:

![[Pasted image 20251014134304.png]]

---

For an MOS transistor, if VGS changes, while the dc biasing current remains constant then V_DS must change.

Thus, from the output characteristics, ID vs V_DS for various values of VGS:

- when VGS increases, VDS decreases.
- when VGS decreases, VDS increases.

The common mode input range refers to the common mode input signal limits such that the dc biasing transistor M7 remains in pinchoff. (VGS1, VGS2, VDS7 and so on), the other side, M1, M2 must remain in pinchoff (VGS1, VGS2, VDS1, VDS2).

---

### Small Signal Operation

Consider the small signals $v_{i1}$ and $v_{i2}$ applied at the gate of M1 and M2, and consider the differential-mode operation where $v_{id} = v_{i1} + v_{i2}$.

Let $v_x$ be the ac potential at node X (the point before the resistor, note: the proper diagram has a transistor there with source to GND acting as a current source, todo).

Then:

- $v_{i1} = v_{gs1} + v_x$
- $v_{i2} = -v_{gs2} + v_x$

So,

- $v_{gs1} = v_x - v_{i1}$
- $v_{gs2} = v_x - v_{i2}$

$V_x = -\frac{v_{gs1} + v_{gs2}}{2} + \frac{v_{i1} + v_{i2}}{2}$

And since $v_{gs1} = \frac{v_{id}}{2}$, $v_{gs2} = -\frac{v_{id}}{2}$,

$V_x = -\frac{v_{gs1} + v_{gs2}}{2} + v_{cm}$

Consider now $v_{i1} = -v_{i2}$:

- $v_{id} = v_{i1} - v_{i2} = 2v_{i1}$
- $v_{cm} = 0$ ($\frac{v_{i1} + v_{i2}}{2}$)

Therefore $v_x = 0$, since $v_{gs1} = -v_{gs2}$.

Two currents result,
$id_1 = gm_1 v_{gs1}$
$id_2 = gm_2 v_{gs2}$
and assuming ideal matched transistors,

$gm_1 = gm_2$

therefore ac current flowing in the differential amplifier is $2gm v_{gs1}$

$id = gm_1 v_{id}$

**AC differential voltage gain:**

$A_{vdd}$ = differential output voltage gain/differential input voltage

$A_{vdd} = \frac{v_{o1} - v_{o2}}{v_{i1} - v_{i2}}$

Draw the ac equivalent circuit:
add img

![[Pasted image 20251014144511.png]]

$v_{gs1} = \frac{v_{id}}{2}$
$v_{o1} = -gm_1 \frac{v_{id}}{2}(r_{ds1} \parallel R)$
$v_{o2} = -gm_2 \left(-\frac{v_{id}}{2}\right)(r_{ds2} \parallel R)$

Since M1 and M2 are matched, $gm_1 = gm_2$, $r_{ds1} = r_{ds2}$

Therefore $v_{o1} - v_{o2} = -gm_1 (r_{ds1} \parallel R) v_{id}$

Therefore the differential voltage gain $A_{vdd} = -gm_1 (r_{ds1} \parallel R)$

**Single-ended output**

$A_{vds} = \frac{v_{o1}}{v_{i1} - v_{i2}} = \frac{v_{o2}}{v_{i1} - v_{i2}}$

Therefore the single ended output voltage is:

$A_{vds} = -\frac{1}{2} gm_1 (r_{ds1} \parallel R)$

**AC output resistance**

The differential ac output resistance $r_{out}$ would be:

$r_{out} = r_{out1} + r_{out2} \rightarrow r_{ds1} \parallel R + r_{ds2} \parallel R$

For a single ended output:

$r_{out} = (r_{ds1} \parallel R) = (r_{ds2} \parallel R)$

[[Common Mode Gain in Single ended output]]
[[Differential Amplifier with Active Load]]
