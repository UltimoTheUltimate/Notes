The phase margin $PM$ is defined at the unity gain frequency $f_T$ and is defined as how far away the phase shift of the circuit at $f_T$ is from $-180^\circ$.

From the phase shift bode plot:

$$\phi_2 + PM = 90^\circ$$

where:
$$\phi_2 = \tan^{-1} \left(\frac{f}{f_{3dB}}\right)$$ 
$$\phi_2 = \tan^{-1} \left(\frac{f_T}{f_{nd}}\right)$$
$$\therefore \phi_2 = \tan^{-1} \left(\frac{GBW}{f_{nd}}\right)$$

To avoid stability issues in circuits with feedback, the PM should be positive. As is a rule of thumb the PM should be at least $30^\circ$.