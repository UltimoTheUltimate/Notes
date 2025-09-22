## Matching Networks: L-Type Example

There are 2 types of L-type Matching Networks: 

- Shunt-Series
- Series-Shunt

Below is an example of a Series Shunt L-type Matching network consisting of a capacitor in series with an inductor in parallel (Shunt)

![[Pasted image 20250922162453.png]]

Below is an example of a Shunt Series L-type Matching network consisting of a Shunt -Series L-Type Matching Network.

![[Pasted image 20250922162437.png]]

> **Note:** Resistors are avoided at all cost due to noise and odd behaviour.  
> Instead, the components used are **inductors** and **capacitors**.

There are **4 combinations** using these components as $X_A$ and $X_B$ being:

- Inductor Inductor
- Inductor Capacitor
- Capacitor Inductor
- Capacitor Inductor

---

### Mathematical Example

*(References Example 1 of Matching Networks sheet)*

**Diagram:**  
![[Pasted image 20250922163626.png]]

**Given:**  
- $Z_S = 150 + j75~\Omega$
- $Z_L = 75 + j15~\Omega$
- $f = 2~\text{GHz}$

Values are **not conjugates**, therefore we must use a matching network as shown above.

---

#### Calculations

$$
\frac{1}{Z_S^*} = \frac{1}{jX_A} + \frac{1}{jX_B} = \frac{1}{jX_B} + Z_L
$$

$$
\frac{1}{150 - j75} = \frac{1}{jX_A} + \frac{1}{75 + j15 + jX_B}
$$

Collect real and imaginary parts:

$$
\frac{1}{150 - j75} = \frac{1}{jX_A} + \frac{1}{75 + j(15 + X_B)}
$$

Rationalise:

$$
\frac{150 + j75}{150^2 + 75^2} = \frac{1}{jX_A} + \frac{75 - j(15 + X_B)}{75^2 + (15 + X_B)^2}
$$

---

##### Real Part

$$
\frac{150}{150^2 + 75^2} = \frac{75}{75^2 + (15 + X_B)^2}
$$

##### Imaginary Part

$$
\frac{75}{150^2 + 75^2} = -\frac{1}{X_A} - \frac{(15 + X_B)}{75^2 + (15 + X_B)^2}
$$

---

#### Solving for $X_B$

$$
75^2 + (15 + X_B)^2 = 14062.5
$$

$$
(15 + X_B)^2 = 8437.5
$$

$$
15 + X_B = \pm 91.856
$$

$$
X_B = 76.86~\Omega \quad (\text{inductor})
$$
**or:**
$$
X_B = -106.856~\Omega \quad (\text{capacitor})
$$

---

##### For Inductor

$$
76.86~\Omega = 2\pi f L_B \\
L_B = \frac{76.86}{2\pi \times 2\,\text{GHz}} = 6.12~\text{nH}
$$

##### For Capacitor

$$
106.856~\Omega = \frac{1}{2\pi f C_B} \\
C_B = \frac{1}{106.856 \times 2\pi \times 2\,\text{GHz}} = 0.745~\text{pF}
$$

---

#### Imaginary Part (when $X_B = 76.86~\Omega$)

$$
\frac{75}{150^2 + 75^2} = -\frac{1}{X_A} - \frac{15 + 76.86}{75^2 + (15 + 76.86)^2}
$$

$$
X_A = 108.71~\Omega
$$

$$
X_A = \frac{1}{2\pi f C_A} \\
C_A = \frac{1}{2\pi \times 2\,\text{GHz} \times 108.71} = 0.732~\text{pF}
$$

---

#### When $X_B = -106.85~\Omega$

$$
\frac{75}{150^2 + 75^2} = -\frac{1}{X_A} - \frac{15 - 106.856}{75^2 + (15 - 106.856)^2}
$$

$$
X_A = 258.71~\Omega
$$

$$
258.71~\Omega = 2\pi f L_A \\
L_A = \frac{258.71}{2\pi \times 2\,\text{GHz}} = 20.6~\text{nH}
$$

---

The two solutions can be presented as so:
**Diagrams:**  
![[Pasted image 20250922164411.png]]
![[Pasted image 20250922164430.png]]
Each solution is mathematically identical at 2GHz, however, the choice depends on component availability and frequency response.