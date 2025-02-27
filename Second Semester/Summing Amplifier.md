![[Pasted image 20250218110922.png]]
Note: let Va, Vb and Vc be V1,V2, V3, along with their resistances and currents (as my notes will go over them in this fashion)



Assuming Ideal opamps, 

Inputs track each other:

$V^{+}=V^{-}=0$

Comment on the inputs of the op-amp:

Assuming inverting mode:

$$I_1+I_2+I_3+\cdots=I_{F}$$
$I_1=\frac{V_1-V^{-}}{R_1}$  $I_2=\frac{V_2}{R_2}$  $I_3=\frac{V_3}{R_3}$

$$I_F=\frac{-V_o}{R_F}$$
$$\therefore I_{F}=-\frac{V_{o}}{R_{F}}=-(\frac{V_1}{R_1}+\frac{V_2}{R_2}+\frac{V_3}{R_3})$$
$$\therefore V_{o}=-R_{F}\left(\frac{V_1}{R_1}+\frac{V_2}{R_2}+\frac{V_3}{R_3}\right)$$



When:

$V_{o}=-\left(2V_1+3V_2+V_3\right)$
$$R_{F}=2R_1$$
$$R_{F}=3R_2$$
$$R_{F}=R_3$$
In the case one of the coefficients is negative, the source must have a negative voltage (resistances are always positive)