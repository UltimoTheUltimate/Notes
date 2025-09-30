## Skeleton Notes Example

### Problem Statement
Design a T-type matching network to transform a load impedance of $Z_L = 60 - j30~\Omega$ into an input impedance of $10 + j20~\Omega$, with a maximum nodal quality factor of 3.

- **Load Impedance:** $Z_L = 60 - j30~\Omega$
- **Input Impedance (Conjugate):** $Z_S^* = 10 + j20~\Omega$

### Normalizing Impedances (by $50~\Omega$)

- $Z_L' = \dfrac{60 - j30~\Omega}{50~\Omega} = 1.2 - j0.6$
- $Z_S^{*'} = \dfrac{10 + j20~\Omega}{50~\Omega} = 0.2 + j0.4$

---

### Smith Chart Steps

#### Capacitor $C_1$
- $1.2 - j0.6 \rightarrow 1.2 - j1.0$
- $\Delta = 0.4 \times 50 = 20$
- $C_1 = \dfrac{1}{2\pi f \times 20}$
- $C_1 = 7.96~\text{pF}$

#### Capacitor $C_2$
- $0.5 - j0.4 \rightarrow 0.5 - j1.5$
- $\Delta = 1.1$
- $C_2 = \dfrac{1.1}{2\pi f \times 50}$
- $C_2 = 3.5~\text{pF}$

#### Inductor $L_3$
- $0.2 - j0.6 \rightarrow 0.2 + j0.4$
- $\Delta = 1 \rightarrow 1 \times 50 = 50$
- $L_3 = \dfrac{50}{2\pi \times 1~\text{GHz}}$
- $L_3 = 7.96~\text{nH}$

---

### Alternative Solution

#### Inductor $L_1$
- $1.2 - j0.6 \rightarrow 1.2 + j$
- $\Delta = 1.6 \times 50 = 80$
- $1.6 \times 50 = 2\pi f L_1$
- $L_1 = 12.7~\text{nH}$

#### Inductor $L_2$
- $0.5 + j0.4 \rightarrow 0.5 + j1.5$
- $\Delta = 1.1$
- $1.1 \times 50 = 2\pi f L_2$
- $L_2 = 7.23~\text{nH}$

#### Capacitor $C_3$
- $0.2 + j0.6 \rightarrow 0.2 + 0.4$
- $\Delta = 0.2$
- $0.2 \times 50 = \dfrac{1}{2\pi f C_3}$
- $C_3 = 15.9~\text{pF}$

---

**Note:** Use the Smith chart for graphical impedance/admittance transformations and component value calculations.
