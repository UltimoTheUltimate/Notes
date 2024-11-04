![[Pasted image 20241028122113.png]]
Not shown: U(s) in between Controller and Plant, E(s) feeding into controller and B(s) as H(S) output.


$$OLTF=\frac{B\left(s\right)}{E\left(s\right)}=G\left(s\right)H\left(s\right)$$
$$CLTF=\frac{C\left(s\right)}{R\left(S\right)}=\frac{G\left(s\right)}{1+G\left(s\right)H\left(s\right)}$$
OLTF is the open loop transfer function and CLTF is the closed loop transfer function.

[[Closed loop poles ]]

The root locus is a plot of the location of the closed loop poles on the s-plane as a function of the open loop gain $k$. Root loci therefore provide important information about stability of closed loop systems based on open loop information.
- The closed loop transfer function of a canonical feedback control system is given by:
$$\frac{C}{R}=\frac{G}{1+GH}$$
- Let the open loop transfer function $GH$ be represented by:$$GH=\frac{kN}{D}$$
- where N and D represent the numerator and denominator polynomials of the open loop transfer function and K in the open loop gain. The closed loop transfer function can be rewritten as:
$$\frac{C}{R}=\frac{G}{1+\frac{kN}{D}}=\frac{GD}{D+kN}$$
- The closed loop poles are the root of the characteristic equation:
$$D+kN=0$$
- For $k=0$, the roots of the characteristic equation are the roots of $D=0$ which are the poles of the open loop transfer function. For k approaching $\infty$, the roots approach those of $N=0$, the open loop zeros.
	- Thus as $k$ increases, from zero to infinity, the loci of the closed loop poles originate from the open loop poles and terminate at the open loop zeros. 

The root locus therefore helps the designer to predict the closed loop poles for a specific gain value and indicate how the closed loop poles and zeros are to be modified to meet the desired system performance specifications.

Ex. plot the root locus analytically for the system with OLTF given by: 
$$GH=\frac{k}{s\left(s+4\right)}$$
The characteristic equation is given by:

$$1+GH=0$$
$$1+\frac{k}{s\left(s+k\right)}=0$$
$$s^2+4s+k=0$$
$$s=-2\pm\sqrt{4-k}$$

| k   | S2    | S2    |
| --- | ----- | ----- |
| 0   | $0$   | -4    |
| 0.5 | 0.13  | -3.87 |
| 1   | -0.27 | -3.73 |
| 3   | -1    | -3    |
| 4   | -2    | -2    |
| 5   | -2+i  | -2-i  |
- for all values of $k>0$, the closed loop system is stable as both poles lie on the left hand side of the plane. 
- For $0\le k\le4$ the poles are real and hence we have non oscillatory response.
- For $k>4$ poles are complex which implies an oscillatory response with a decaying effect since the real part is negative.
- as $k$ increases, the imaginary part increases, therefore the frequency of oscillations increases.
[[Construction Rules]]
