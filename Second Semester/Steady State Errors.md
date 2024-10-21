diagram 2

The steady state error for stable system is given by:
$$e_{gs}=\lim_{t\to\infty}e\left(t\right)$$
by Laplace transform:

$$E\left(s\right)=R\left(S\right)-Y\left(s\right)$$
$$E\left(s\right)=R\left(s\right)-G\left(s\right)E\left(s\right)$$
And hence in the S domain it is given by:
$$E(s)=\lim_{s\to0}\frac{sR\left(s\right)}{1+G\left(s\right)}$$
[[WorkingSSE]]

Thus, the steady state error $e_{gs}$ depends on:

The feed forward transfer $f_{n}G(s)$  or more specifically it depends on the [[System Type]] of $G_{\left(s\right)}$  (order) that is the number of poles on the open loop transfer function $G_{\left(s\right)}$ located at $s=0$
The input signal R(S)

[[Testing signals for steady state error analysis]]
