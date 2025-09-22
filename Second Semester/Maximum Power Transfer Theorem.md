Let the source impedance be $$ Z_S = R_S + jX_S $$ and the load impedance be $$ Z_L = R_L + jX_L $$.

- $$ X > 0 $$: inductive
- $$ X < 0 $$: capacitive

Let $$ I_s $$ be the current across the series circuit:

$$
I_s = \frac{V_s}{Z_S + Z_L}
$$
$$
I_s = \frac{V_s}{R_S + jX_S + R_L + jX_L}
$$
$$
I_s = \frac{V_s}{(R_S + R_L) + j(X_S + X_L)}
$$

The real power transferred to the load ($$ P_L $$) is:

$$
P_L = |I_s|^2 R_L
$$
$$
P_L = \frac{|V_s|^2 R_L}{(R_S + R_L)^2 + (X_S + X_L)^2}
$$

For maximum power transfer, set $$ X_L = -X_S $$:

$$
P_L = \frac{|V_s|^2 R_L}{(R_S + R_L)^2}
$$

To maximize $$ P_L $$ with respect to $$ R_L $$, differentiate the denominator:

Let $$ f(R_L) = (R_S + R_L)^2 $$

$$
\frac{df}{dR_L} = 2(R_S + R_L)
$$

Set the derivative to zero for maximum power transfer:

$$
2(R_S + R_L) = 0 \implies R_S + R_L = 0 \implies R_L = -R_S
$$

Since negative resistance is not physical, the maximum occurs at:

$$
R_L = R_S
$$

Maximum power transfer occurs when $$ Z_L = Z_S^* $$, i.e., the load impedance is the complex conjugate of the source impedance.

**Therefore, for maximum power transfer:**
- The load reactance must be the negative of the source reactance ($$ X_L = -X_S $$)
- The load resistance must equal the source resistance ($$ R_L = R_S $$)
