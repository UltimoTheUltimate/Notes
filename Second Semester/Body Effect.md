The main idea of the MOS transistor is to apply a vertical electric field, via $V_{GS}$ and get a lateral current $I_D$. Vertical currents need to be avoided. In the vertical directions, PN junctions along the whole perimeter from source to channel to drain, under to avoid any vertical current across the p-n junction, a fourth terminal, the bulk terminal B is introduced, and then the bulk and source terminals are shorted, so that $V_{BS} = 0V$ (see diagrams below for 4-terminal symbols)

![[Pasted image 20250225103511.png]]

If $V_{BS}=0V$ then the body effect results. The body effect makes it the fact that when $V_{GS}\not= 0$ the threshold voltage $V_T$ increases

This is a desired voltage, as it reduces the headroom for AC signals in, for example amplifiers. The increase in threshold voltage is given by:

$$V_T=V_{T0}+\gamma[\sqrt{\phi-V_{BS}}-\sqrt{\phi}]$$


