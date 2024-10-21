Input is a step with magnitude R

$$r\left(t\right)=Ru\left(t\right)$$
By Laplace:

$$R\left(s\right)=\frac{R}{S}$$
The steady state error for this type of input is given by:

$$e_{gs}=\frac{R}{1+\lim_{s\to0}G\left(s\right)}$$
[[Workingssestep]]

Define the position error constant $Kp=\lim_{s\to0}G\left(s\right)$, then the steady state error is given by:

$$e_{gs}=\frac{R}{1+Kp}$$
If $G\left(s\right)$ is of type 0, then $Kp=K$ and $e_{gs}=\frac{R}{1+K}$

If $G\left(s\right)$ is of type 1, then $Kp=\infty$ and $e_{gs}=0$
