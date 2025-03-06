Consider the MOS transistor with the gate shorted to the drain.

$$V_{DG}=0V$$

Since the condition for n-channel to be in pinch off is $V_{DG}\ge-V_T$
or 
$V_{DS}\ge V_{GS}-V_T$ 

and since $V_T\approx +0.8V$
then the transistor operates in pinchoff
$$\therefore I_D=\frac{K'}{2}\frac{W}{L}\centerdot(V_{GS}-V_T)^2$$
which becomes:
$$I=\frac{K'}{2}\frac{W}{L}\centerdot(V_-V_T)^2$$
or:
$$V=V_T+\sqrt{\frac{2I}{K'\frac{W}{L}}}$$
The transistor with the gate shorted wit hthe drain is thus a non-linear resister where $I=f(V-V_T)^2$ on the voltage V developed across the two-terminal component $V=\frac{f}{\sqrt{I}}$ 
$\therefore$ for dc signals the transistor behaves as a two-terminal non-linear resistance

Consider now an AC signal.

Draw the AC equivalent circuit

MOS transistor in pinch-off with gate shorted to drain 

Using the [[Source absorption theory]] we get the following AC equivalent circuit

Thus the MOS transistor with gate shorted to drain behaves as a resistance $r_{ds}//\frac{1}{g_m}$

Since $\frac{1}{g_m}<<r_ds$ then the ac source absorption theorem resistance of the transistor is approximately $\frac{1}{gm}$ 

i.e.: $$\frac{1}{\sqrt{2K'\frac{W}{L}I}}$$
Since the value of the resistance is a non-linear function of the current I following through the transistor, the resistance value changes with the current and thus the MOS transistor with gate shorted to drain is called an active resistor

The MOS transistor with gate shorted to drain is also called the "diode connected" transistor