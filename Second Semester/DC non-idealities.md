The first stage of an op-amp is the differential amplifier. In a perfectly-matched differential amplifier, no dc non-idealities would arise. In practice the matching of the two branches of a differential amplifier will not be perfect. As a result, DC offset voltages arise.

Input Offset Voltage:

consider the circuit below:

For an ideal op-amp:
$$V_{o}=A\left(V^{+}-V^-\right)=0$$
The input voltage required to rearrange the output offset voltage to zero is called the input offset voltage $V_{io}$

If $V_{io}$ is only the offset voltage at the output voltage at the output, then $V_{io}=\frac{V_o}{A}$ 

recall: for inverting amplifier:

$$\frac{V_{o}}{V_i}=-\frac{Rf}{R_1}$$

but due to the input offset voltage:

$$V_{o}=-\frac{R_{f}}{R_1}\centerdot V_1-\frac{R_{F}}{R_1}\centerdot V_{in}$$


Input bias current:

The input resistance at an opamp terminal is not perfectly infinity, although still very large. As a result there is an input bias current, of the nature of $nA$, at each of the two inputs, $I_{B1}$ and $I_{B2}$

$$I_{B}=\frac{I_{B1}+I_{B2}}{2}$$

The input offset current $I_{io}$ is defined by:$$I_{io}=\left|I_{B1}-I_{B2}\right|$$
Temperature Drift

Since all semiconductor properties are temperature dependent, $V_{io}$, $I_B$ and $I_{io}$ are also temperature dependent. Each of these offsets will have temperature coefficients

$\frac{dV_{io}}{dT},\frac{dI_{B}}{dT}$ and $\frac{dI_{io}}{dT}$

The DC offsets can be balanced out using a thermostat connected to a specific pin inside an the opamp provided by the manufacturer. However note that $V_{io}$ will be zero at the temperature at which the balancing out is carried out, once the temperature changes, $V_{io}$ will start to appear again.