## Problem

Design a low pass $\Pi$ type matching network that matches $Z_L = 100 - j50/\Omega$ to a source impedance $Z_s = 20 - j40/\Omega$ at a nodal quality factor of $Q = 4$. Calculate the values at $900\,\text{MHz}$.

---

### Normalizing $Z_L$ and $Z_s^*$

- $Z_L' = \dfrac{100 - j50}{50} = 2 - j$
- $Z_s^{'*} = \dfrac{20 + j40}{50} = 0.4 + j0.8$

$Q = \dfrac{|B|}{G}$

---

### Calculations

#### $C_1$ Calculation

$\Delta \rightarrow 0.4 - 0.2 \rightarrow 0.4 - 0.6 = 1.4$

$\dfrac{1}{1.4 \times 50} = \dfrac{1}{2\pi f C_1}$

$C_1 = 4.95\,\text{pF}$

---

#### $L_2$ Calculation

$-0.6 + 0.5$

$\Delta = 1.1 \times 50 = 2\pi f L_2$

$L_2 = 9.73\,\text{nH}$

---

#### $C_3$ Calculation

$\Delta \rightarrow 1.8 \rightarrow 1 = 0.8$

$\dfrac{1}{0.8 \times 50} \times \dfrac{1}{2\pi f C_3}$

$C_3 = 2.8\,\text{pF}$
