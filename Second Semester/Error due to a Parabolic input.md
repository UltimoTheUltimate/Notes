Input is a parabolic with magnitude $R$:
$$r\left(t\right)=Rt^2u\left(t\right)$$
By Laplace:
$$R\left(s\right)=\frac{R}{S^3}$$
The steady state error for this type of input is given by:
$$e_{gs}=\lim_{s\to0}\frac{sR\left(s\right)}{1+G\left(s\right)}=\lim_{s\to0}s.\frac{R}{s^3}\frac{.1}{1+G\left(s\right)}=\frac{R}{\lim_{s\to0}S^2G\left(s\right)}$$
Define the acceleration error constant $Ka=\lim_{s\to0}S^2G\left(s\right)$ then the steady state error is given by:

$e_{gs}=\frac{R}{Ka}$

If $G\left(s\right)$ is of type 0 or type 1 then $Ka=0$,$e_{gs}=\infty$
If $G\left(s\right)$ is of type 2 then $Ka=K$ and $e_{gs}=\frac{R}{K}$
If $G\left(s\right)$ is of type 3 or higher, then $Ka=\infty$, $e_{gs}=0$

