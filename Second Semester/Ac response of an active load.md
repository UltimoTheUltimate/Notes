## AC Response of a Diode-Connected MOS Transistor

Consider the AC model of a MOS transistor in pinch-off:

- Since $v_{gs} \equiv v_{ds}$, the current source can be replaced by a resistance equal to $1/g_m$ (by the source absorption theorem).

Thus, the AC equivalent circuit becomes:

- For AC signals, the diode-connected transistor is equivalent to a resistance:
    - $r_{ac} = \frac{1}{g_m} \parallel r_{ds}$

Typically, $1/g_m \ll r_{ds}$, so:

- $\therefore\ r_{ac} \approx \frac{1}{g_m}$

This means the diode-connected transistor acts as a small resistance for AC signals.
