## Frequency Response Analysis

### First Circuit (from recorded notes)

| Frequency            | Vout/Vs |
|----------------------|---------|
| $f \to 0\,\text{Hz}$ | 0       |
| $f \to 1\,\text{GHz}$| 0.632   |
| $f \to \infty\,\text{GHz}$ | 0 |

---

#### Calculation at 1 GHz

At $1\,\text{GHz}$:  
$P_{50\Omega} = P_{80\Omega}$

$$(V_s - V_s/2)^2 / 50 = V_\text{out}^2 / 80$$

$$(V_s^2) / (4 \times 50) = V_\text{out}^2 / 80$$

$$\frac{V_\text{out}}{V_s} = \sqrt{\frac{80}{4 \times 50}} = 0.632$$

**Gain:**  
$20 \log_{10}(0.632) = -3.97\,\text{dB}$

---

### Second Circuit

| Frequency            | Vout/Vs |
|----------------------|---------|
| $f \to 0\,\text{Hz}$ | 0       |
| $f = 1\,\text{GHz}$  | 0.632   |
| $f \to \infty$       | 0.615   |

At $f \to \infty$:

As capacitors block DC and allow AC, and inductors block AC and allow DC, the circuit becomes a potential divider:

$$\frac{V_\text{out}}{V_s} = \frac{80}{50 + 80} = 0.615$$

**Gain:**  
$20 \log_{10}(0.615) = -4.22\,\text{dB}$

[[Gaining more information about frequency response]]