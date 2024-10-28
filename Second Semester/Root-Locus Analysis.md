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