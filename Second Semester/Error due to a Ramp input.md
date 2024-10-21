Input is a ramp with magnitude R:
$$r\left(t\right)=Rtu\left(t\right)$$ 
By Laplace:
$$R\left(s\right)=\frac{R}{S^2}$$
The steady state error of the input is given by:
$$e_{gs}=\lim_{s\to0}\frac{sR\left(s\right)}{1+G\left(s\right)}=\lim_{s\to0}s.\frac{R}{s^2}.\frac{1}{1+G\left(S\right)}=\lim_{s\to0}\frac{R}{S+SG\left(s\right)}=\lim_{s\to0}\frac{R}{SG\left(s\right)}$$
Define the velocity error constant $$K_{v}=\lim_{s\to0}sG\left(s\right)$$
Then, The steady state error is given by:
$$e_{gs}=\frac{R}{K_{v}}$$
	If $G\left(s\right)$ us of type 0, then $K_{v}=0$ and $e_{gs}=\infty$
	If $G\left(s\right)$ is of type 1, then $K_{v}=K$ and $e_{gs}=\frac{R}{K}$
	If $G\left(s\right)$ is of type 2 or higher, then $K_{v}=\infty$ and $e_{gs}=0$
