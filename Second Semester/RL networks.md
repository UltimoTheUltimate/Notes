## RL Networks: Series and Parallel Forms

### Series Form

Resistor $R_s$ in series with inductor $L_s$:

$$
Z_{\text{series}} = R_s + j\omega L_s
$$

---

### Parallel Form

Resistor $R_p$ in parallel with inductor $L_p$:

$$
Z_{\text{parallel}} = \frac{1}{\frac{1}{R_p} + \frac{1}{j\omega L_p}} = \frac{j\omega L_p R_p}{R_p + j\omega L_p}
$$

---

### Equating Series and Parallel Forms

Set $Z_{\text{series}} = Z_{\text{parallel}}$:

$$
R_s + j\omega L_s = \frac{j\omega L_p R_p}{R_p + j\omega L_p}
$$

---

### Rationalising the Denominator

Multiply numerator and denominator by the complex conjugate:

$$
\frac{j\omega L_p R_p}{R_p + j\omega L_p} \cdot \frac{R_p - j\omega L_p}{R_p - j\omega L_p}
$$

For coefficient comparison, expand denominator:

$$
R_p + j\omega L_p
$$

---

### Compare Coefficients

#### Real Part

$$
R_s = \frac{\omega^2 L_p^2 R_p}{R_p^2 + \omega^2 L_p^2}
$$

Let $Q_p = \frac{R_p}{\omega L_p}$:

$$
R_s = \frac{R_p}{Q_p^2 + 1}
$$

$$
R_p = (Q_p^2 + 1) R_s
$$

#### Imaginary Part

$$
\omega L_s = \frac{\omega L_p R_p^2}{R_p^2 + \omega^2 L_p^2}
$$

$$
L_s = \frac{L_p R_p^2}{R_p^2 + \omega^2 L_p^2}
$$

Express in terms of $Q_p$:

$$
L_s = \frac{L_p}{Q_p^2 + 1}
$$

$$
L_p = (Q_p^2 + 1) L_s
$$

#### Alternative Forms

$$
L_s = \frac{L_p}{\left(\frac{\omega L_p}{R_p}\right)^2 + 1}
$$

$$
L_p = L_s \left[\left(\frac{1}{Q_p}\right)^2 + 1\right]
$$

---

### Quality Factor

$$
Q_s = \frac{|X_s|}{R_s} = \frac{\omega L_s}{R_s}
$$

Since $R_s = \frac{R_p}{Q_p^2 + 1}$ and $L_s = \frac{L_p}{Q_p^2 + 1}$:

$$
Q_s = \frac{\omega L_s}{R_s} = \frac{\omega L_p / (Q_p^2 + 1)}{R_p / (Q_p^2 + 1)} = \frac{\omega L_p}{R_p} = \frac{1}{Q_p}
$$

So,

$$
Q_s = \frac{1}{Q_p}
$$

---

### Summary Relations

$$
R_p = (Q_p^2 + 1) R_s
$$

$$
L_p = (Q_p^2 + 1) L_s
$$

$$
R_p = (Q_s^2 + 1) R_s
$$

$$
L_p = (1 + Q_s^2) L_s
$$
