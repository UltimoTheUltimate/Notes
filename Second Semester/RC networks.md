## Series RC Impedance

$$
Z_\text{series} = R_s + \frac{1}{j\omega C_s}
$$

## Parallel RC Admittance

$$
Y_\text{parallel} = \frac{1}{R_p} + j\omega C_p
$$

where  
$\omega$ = angular frequency

---

## Equivalence Between Series and Parallel

$$
Z_\text{series} = \frac{1}{Y_\text{parallel}}
$$

So,

$$
R_s + \frac{1}{j\omega C_s} = \frac{1}{\frac{1}{R_p} + j\omega C_p}
$$

Expanding the parallel admittance:

$$
\frac{1}{R_p} + j\omega C_p = \frac{1 + j\omega R_p C_p}{R_p}
$$

So,

$$
Z_\text{parallel} = \frac{R_p}{1 + j\omega R_p C_p}
$$

Set equal to series:

$$
R_s + \frac{1}{j\omega C_s} = \frac{R_p}{1 + j\omega R_p C_p}
$$

---

## Matching Real and Imaginary Parts

Let

$$
Q_s = \frac{1}{\omega C_s R_s}
$$
*(quality factor)*

**Imaginary part:**

$$
C_p = \frac{C_s}{1 + (\omega R_s C_s)^2}
$$

Or, in terms of $Q_s$:

$$
C_p = \frac{Q_s^2 C_s}{1 + Q_s^2}
$$

**Real part:**

$$
R_p = (1 + Q_s^2) R_s
$$

---

## Summary

- $Q_s = \frac{1}{\omega C_s R_s}$
- $C_p = \frac{Q_s^2 C_s}{1 + Q_s^2}$
- $R_p = (1 + Q_s^2) R_s$

---

## Parallel Quality Factor $Q_p$

$$
Q_p = \frac{R_p}{|X_p|} = R_p \cdot \omega C_p
$$

Substitute $R_p = (1 + Q_s^2) R_s$ and $C_p = \frac{Q_s^2 C_s}{1 + Q_s^2}$:

$$
Q_p = (1 + Q_s^2) R_s \cdot \omega \frac{Q_s^2 C_s}{1 + Q_s^2} = R_s \omega Q_s^2 C_s
$$

But $Q_s = \frac{1}{\omega C_s R_s}$, so:

$$
Q_p = Q_s
$$