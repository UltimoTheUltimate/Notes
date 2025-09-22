Internally in the MOS transistor, three unwanted capacitances arise: 

C_{gs} is the parasitic capacitance between gate and source that arises due to misalignment, and hence overlap between the gate and the source.

C_{gd} is the paracitic capacitance between gate and drain, again arising due to misalignment between gate and drain;

C_{ds} is the paracitic capacitance between drain and source, resulting from the depletion refions along the pn junction perimeter.

These parasitic capacitances effect the frequency response of the MOS transistor and need to be added to the model for the MOS transistor in pinchoff

![[Pasted image 20250327103452.png]]

Since $X=\frac{1}{2\pi fC}$ and $C\rightarrow fF$ 

at low frequencies $X_c\rightarrow \infty$,  i.e. open circuit 


The maximum effect of these parasitic capacitances is to reduce the AC voltage gain in an amplifier as the frequency increases.

A_{v_o} is the low-frequency voltage gain f_T is the unity-gain frequency

f_{3dB} is the 3-db frequency, i.e. the frequency at which |AV| is less than the low frequency voltage A_v, by 3db.

At the 3db frequency the phase shift \ro between an output signal and an input signal is -45 degrees

Each node which is not at ac ground will result in a pole. Each pole results in the decrease of |A_V| and a phase shift of -90\deg. Each pole has its own 3dB frequency, where the phase shift is -45\deg, its own unity gain frequency. The decrease of |A_v| produced by each pole is 20dB\dec 

