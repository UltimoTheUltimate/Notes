![[Pasted image 20250403101134.png]]
There are two nodes in the circuit which are not at AC ground. Node 1 at the input side and node 2 at the output side. Each node contains a pole which in turn affects the frequency response of the amplifier.

Consider node 1:  
The pole frequency, i.e., the 3-dB frequency, that results from node 1 is obtained by:  
$$f_{p_1} = \frac{1}{2\pi R_{\text{eff}}C_{\text{eff}}}$$  
where $R_{\text{eff}}$ is the AC resistance from node 1 to ground and $C_{\text{eff}}$ is the effective capacitance from node 1 to ground.  

$$R_{\text{eff}} = R_s$$  

$$C_{\text{eff}} = C_{gs1} + C_{gs2} + (C_{gd1} + C_{gd2})A_v$$  
$$\approx (C_{gd1} + C_{gd2})A_v$$  

where:  
$$A_v = (g_{m1} + g_{m2})(r_{ds1} \parallel r_{ds2})$$  
$$A_v = \frac{g_{m1} + g_{m2}}{g_{ds1} + g_{ds2}}$$  

$$\therefore f_{p_1} = \frac{1}{2\pi R_s(C_{gd1} + C_{gd2}) \cdot A_v} = \frac{g_{ds1} + g_{ds2}}{2\pi (C_{gd1} + C_{gd2})(g_{m1} + g_{m2})}$$  

Consider node 2:  
$$f_{p_2} = \frac{1}{2\pi R_{\text{eff}}C_{\text{eff}}}$$  
where $R_{\text{eff}}$ is the output resistance from node 2 to ground.  

$$R_{\text{eff}} = r_{ds1} \parallel r_{ds2}$$  
$$C_{\text{eff}} = C_L + C_{ds1} + C_{ds2} + C_{gd1} + C_{gd2}$$  
$$= C_L + C_{m2}$$  

where $C_{m2}$ is the total parasitic capacitance at node 2.

in general, $C_{m2} \ll C_L$.  

$$\therefore C_{\text{eff}} \approx C_L$$  

$$\therefore f_{p_2} = \frac{g_{ds1} + g_{ds2}}{2\pi C_L}$$  

$$f_{p_1} = \frac{g_{ds1} + g_{ds2}}{2\pi R_s(C_{gd1} + C_{gd2})(g_{m1} + g_{m2})}$$

In order to understand if the frequency response of the amplifier is a dominant response or a non-dominant response, only one pole $f_{p1}$ or $f_{p2}$, must be below $f_t$, the unity gain frequency.

[[Gain Bandwidth]]
[[Phase Response]]
