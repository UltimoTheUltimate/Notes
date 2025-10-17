## Transmission Parameters

### Equations

```markdown
V₁ = A·V₂ - B·I₂  
I₁ = C·V₂ - D·I₂
```

### Transmission Matrix

**Port 1:**  
$$
\begin{bmatrix}
V_1 \\
I_1
\end{bmatrix}
=
\begin{bmatrix}
A & B \\
C & D
\end{bmatrix}
\begin{bmatrix}
V_2 \\
- I_2
\end{bmatrix}
$$

### Parameter Definitions

- **A**: $A = \frac{V_1}{V_2} \Big|_{I_2 = 0}$  
    *Inverse of the voltage gain when the network is not loaded ($I_2 = 0$); open circuit test.*

- **B**: $B = \frac{V_1}{-I_2} \Big|_{V_2 = 0}$

- **C**: $C = \frac{I_1}{V_2} \Big|_{I_2 = 0}$

- **D**: $D = \frac{I_1}{-I_2} \Big|_{V_2 = 0}$

inverse of the circuit gain when the network is loaded with a short circuit on part 2
(V2 = 0) -> short circuit test

