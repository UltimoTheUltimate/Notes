Consider a closed loop system:

$$\frac{Y\left(s\right)}{R\left(s\right)}=\frac{G\left(s\right)}{Y+G\left(s\right)H\left(s\right)}$$

In this case:
$$\frac{\partial Y\left(s\right)}{\partial G\left(s\right)}=\frac{R\left(s\right)}{\left\lbrack1+G\left(s\right)H\left(s\right)\right\rbrack^2}$$

And the sensitivity function becomes:
$$S_{G}^{Y}=\frac{\frac{\partial Y\left(s\right)}{Y\left(s\right)}}{\frac{\partial G\left(s\right)}{G\left(s\right)}}=\frac{\partial Y\left(s\right)}{\partial G\left(s\right)}\cdot\frac{G\left(s\right)}{Y\left(s\right)}=\frac{R\left(s\right)}{\left\lbrack1+G\left(s\right)H\left(s\right)\right\rbrack^2}\cdot\frac{1+G\left(s\right)H\left(s\right)}{R\left(s\right)}=\frac{1}{1+G\left(s\right)H\left(s\right)}$$

In this case if $\vert G\left(s\right)H\left(s\right)\vert\gg1$ then $S_{G}^{Y}\thickapprox0$
In this case if $\vert G\left(s\right)H\left(s\right) \vert \ll1$ then $S_{G}^{Y}\thickapprox1$

Thus larger values for $\vert G\left(s\right)H\left(s\right)\vert$ are desirable to limit the output sensitivity to changes in the feed-forward transfer function

[[Numerical example CLS]]

 - Therefore the sensitivity of the closed loop system is reduced by a factor of $\frac{1}{1+G\left(s\right)H\left(s\right)}$ when compared to that of an open loop system.
- Similar sensitivity measures can be considered for changes in the feedback path transfer function $H\left(s\right)$
$$\frac{\partial Y\left(s\right)}{\partial H\left(s\right)}=\frac{-R\left(s\right)G^2\left(s\right)}{\left\lbrack1+G\left(s\right)H\left(s\right)]\right.}$$
And the sensitivity function becomes:
$$S_{H}^{Y}=\frac{\partial Y\left(s\right)}{\partial H\left(s\right)}\cdot\frac{H\left(s\right)}{Y\left(s\right)}=\frac{-R\left(s\right)G^2\left(s\right)}{\left\lbrack1+G\left(s\right)H\left(s\right)\right\rbrack^2}\cdot\frac{H\left(s\right)\left\lbrack1+G\left(s\right)H\left(s\right)\right\rbrack}{R\left(s\right)G\left(s\right)}=\frac{-G\left(s\right)H\left(s\right)}{1+G\left(s\right)H\left(s\right)}$$

- Thus to consider both $S_{G}^{Y}$ and $S_{^{}H}^{Y}$ the value for $\vert G\left(s\right)H\left(s\right)\vert$ must be chosen to balance out the effect of parameter changes on the system's stability
- In practice the feedback elements such as sensors can be chosen up to a level of required precision, thus limiting the variations in $H\left(s\right)$. High values of $\vert H\left(s\right)G\left(s\right)\vert$ are therefore usually used to limit the sensitivity of the system to variations in the physical system to be controlled.