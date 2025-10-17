## Frequency Response of an MOS Transistor

In the MOS transistor, there are internal unwanted parasitic capacitances:

- **Cgs**: between gate and source  
- **Cgd**: between gate and drain  
- **Cds**: between drain and source  

**Typical order of magnitude:** pF–fF

---

### AC Model in Pinchoff (Including Parasitic Capacitances)

![[Insert image of AC model with parasitic capacitances]]

---

### Full Amplifier Circuit

The full amplifier circuit includes:
- Input stage
- Inverter amplifier
- Capacitive load

To analyze the frequency response, consider the circuit nodes that are not at AC ground.

![[Insert image of full amplifier circuit]]

---

#### Parasitic Capacitances on the Circuit

> **Note:**  
> - *Cgs2* and *Cgd2* are not included since there is no AC signal at the gate of M2.
> - There are **2 nodes** not at AC ground:  
>   - **Node 1:** Input  
>   - **Node 2:** Output

---

### Poles and Frequency Response

- Every node produces a **pole**.
- Every pole results in a decrease of the AC voltage gain.
- The frequency at which the AC voltage gain is reduced by 3dB is called the **3dB frequency** or **pole frequency**.

#### Pole Frequency Formula

$$
f_p = \frac{1}{2\pi R_\text{eff} C_\text{eff}}
$$

Where:
- $$R_\text{eff}$$ = effective resistance to ground
- $$C_\text{eff}$$ = effective capacitance to ground

---

### Miller's Theorem

#### Pole Frequency at Node 1

$$
f_{p1} = \frac{1}{2\pi R_s (C_{GS1} + C_{GD1} A_v)}
$$

Approximation:

$$
f_{p1} \approx \frac{1}{2\pi R_s C_{GD1} A_v}
$$

---

#### Pole Frequency at Node 2

To find $$f_{p2}$$ at node 2:

- $$R_\text{eff} = r_\text{out} = r_{ds1} \parallel r_{ds2}$$
- $$C_\text{eff} = C_{ds1} + C_{ds2} + C_{gd1} + C_L$$

In practice, $$C_L \gg$$ parasitic capacitance, so:

$$
C_\text{eff} \approx C_L
$$

Therefore,

$$
f_{p2} = \frac{1}{2\pi (r_{ds1} \parallel r_{ds2}) (C_{ds1} + C_{ds2} + C_{gd1} + C_L)}
$$

Approximation:

$$
f_{p2} \approx \frac{g_{ds1} + g_{ds2}}{2\pi C_L}
$$

---

### Frequency Response of $$|A_v|$$

- Both poles could occur at a frequency below the unity gain frequency $$f_T$$.
- Alternatively, one pole could occur below $$f_T$$ and the second pole above $$f_T$$.
- In this case, $$f'_p$$ is called the **dominant pole** ($$f_D$$), and $$f''_p$$ is the **non-dominant pole**.
- This second frequency response plot is referred to as a **dominant-pole frequency response**. This is the response that a good amplifier design should have.
- The first type of frequency response (non-dominant) can lead to instability.

---

### Parallel Input Inverter Amplifier

Consider the circuit below, where the input is applied to the gates of both M1 and M2:

Since $$v_i$$ is applied to both M1 and M2, the AC voltage gain $$A_v = v_o / v_i$$ is now given by:

$$
A_v = -\frac{g_{m1} + g_{m2}}{g_{ds1} + g_{ds2}}
$$

Comparing to previous equation:  
The AC voltage gain of the parallel input inverting amplifier is greater than that of the single input inverter amplifier analyzed previously in terms of design parameters.

$$
A_v = \frac{\sqrt{2K'_n(W/L)_1} + \sqrt{2K'_p(W/L)_2}}{(\lambda_n + \lambda_p)\sqrt{I_D}}
$$

The AC output resistance:

$$
r_{out} = r_{ds1} \parallel r_{ds2} = \frac{1}{g_{ds1} + g_{ds2}}
$$

The AC frequency response is carried out in a similar manner to the single input inverting amplifier, since there are again 2 nodes: node 1 at the input and node 2 at the output.

Calculate $$f_{p1}$$ and $$f_{p2}$$ using:

$$
f_p = \frac{1}{2\pi R_\text{eff} C_\text{eff}}
$$

Then determine the dominant pole.

