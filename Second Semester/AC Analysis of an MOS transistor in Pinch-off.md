MOS transistor in pinchoff:

$$ID=\frac{K'}{2}\frac{W}{L}\centerdot(V_{GS}-V_T)^2 $$

Trans-conductance $g_m=\frac{\partial I_D }{\partial V_{GS}}$

By differenciating the pinchoff equation we get:

$$ K'\centerdot \frac{W}{L}\centerdot(V_{GS}-V_T) $$
But $V_{GS}-V_T=\sqrt{\frac{2I_D}{K'+\frac{W}{L}}}$

$$\therefore \sqrt{2K'\centerdot \frac{W}{L}I_D } $$

Consider an AC signal $V_{GS}$ applied at the gate, superimposed on the DC V_{GS}. pinch off equation becomes

$$I_D=\frac{K'}{2}\frac{W}{L}\centerdot(V_{GS}+v_{GS}-V_T)^2$$
$$=\frac{K'}{2}\frac{W}{L}[(V_{GS}-V_T)+V_{GS}]^2$$
$$I_D=\frac{K'}{L}\frac{W}{L}[(V_{GS}-VT)^2+2V_{GS}(V_{GS}-V_T)+V_{GS}^2]$$

To ensure that the AC output current waveform is still a sine wave, we need to apply this condition: 
$$v_{GS}<<2v_{GS}(V_{GS}-V_T)$$

and therefore:

$$V_{GS}<<2(V_{GS}-V_T)$$
Thus $$I_D=I_D+i_d$$
$$\therefore i_d=K'\frac{W}{L}(V_{GS}-V_T)\centerdot v_{gs}$$
but $g_m=K'\centerdot\frac{W}{L}(V_{GS}-V_T)$
$\therefore i_d=g_m-v_{gs}$
Thus under the ac small-signal condition, when an ac signal $v_{gs}$ is applied at the input, (i.e. the gate) an ac current $i_d$ results at the output, where $i_d=g_mv_{gs}$ 
Thus the output is an ideal current source.
The ideal MOS transistor model for an ac input signal is thus: 
![[Pasted image 20250225114017.png]]
Taking into consideration the channel length modulation effect, the MOS transistor in pinch off becomes:
![[Pasted image 20250225114045.png]]

The ac current source $g_mv_{gs}$ is most not ideal, but thus, some finite ac output resistance $r_{out}$, denoted by $r_{ds}$ 
$$r_{ds}=\frac{1}{\lambda I_D}$$
Weak inversion

In weak inversion the n-channel electron concentration is low. The pinch off equation in the ideal MOS transistor is:

$$I_D=I_{D0}\centerdot\frac{W}{L}e^{\frac{V_{GS-V_T}}{nV_T}}$$
where $I_{D0}$ is in m
$V_t=\frac{kt}{Q}$ thermal volt equivalence
$n=$ constant around $2$

$$I_D=I_{D0}\frac{W}{L}\centerdot e^\frac{V_{GS}-V_T}{nV_T}e^{-\frac{V_{DS}}{V_T}}e^{-V_{BS}[\frac{1}{nV_t}-\frac{1}{V_t}]}$$

Next time: Active Resistances