## Overall Quality Factor

$$
\text{Overall Quality Factor} = \frac{f_\text{res}}{\Delta f}
$$

where:  
- $\Delta f$ is the bandwidth  
- $f_\text{res}$ is the resonant frequency

Alternatively,

$$
\text{Overall Quality Factor} = \frac{\text{Maximum Nodal Quality Factor}}{2}
$$

---

## Nodal Quality Factor

$$
Q_n = \frac{|X|}{R}
$$

### At $Z_L$:
$$
Q_n = \frac{1.2}{1.6} = 0.75
$$

### When Adding the Capacitor:
$$
Q_n = \frac{1.2}{1} = 1.2 \to \text{Maximum nodal quality factor}
$$

### When Adding the Inductor:
$$
Q_n = \frac{0}{1} = 0
$$
**Therefore:**

$$
\text{Overall Quality Factor} = \frac{1.2}{2} = 0.6
$$


## Recall

- $R_p = [1 + Q_s^2] R_s$
- $C_p = \frac{Q_s^2}{1 + Q_s^2} C_s$

Where:

- $Q_s = \frac{1}{\omega C_s R_s} = \frac{1}{2\pi \times 1\,\text{GHz} \times 2.65\,\text{pF} \times 80}$
- $Q_s = 0.75$

Calculations:

- $R_p = [1 + (0.75)^2] \times 80 = 125.09\,\Omega$
- $C_p = 0.954\,\text{pF}$

Rp = (1+Qs)^2Rs
Lp = (1+Qs^2)/Qs^2
Qs = \omegaL/Rs 2/pi x 1GHz x 9.55nA/50
=1.2

R_p = (1+1.2^2)50 =122/Omega
Lp = [1+1.2^2]/1.2^2 x 9.55nH = 16.18nH

Q = (122//125)/2\pix16.18nHx1GHz = 0.6073


Qp = Rp/|Xp|


Qoverall = 0.6 = fres/\Delfaf
\Deltaf=1GHz/0.6 = 1.67GHz