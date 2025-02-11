The inverting amplifier has the following circuit diagram:


Now begins Math Time$^{TM}$

Our end goal is to arrive at a **transfer function:** $\frac{V_{out}}{V_{in}}$

**It is very essential to start with the rule** $V^{+}=V^{-}$, as in this case, $V^{+}=0=V^{-}$ due to $V^{+}$ being **grounded**.

Looking at the node marked as **A** in the circuit: $$I_1=I_{F}+I_{in}$$
where as $V_{in}\to0$  becomes:$$I_1=I_{F}$$
Now: $$I_{1}=\frac{V_{in}-V^{-}}{R_1}=\frac{V_{in}}{R_1}$$
$$I_{f}=-\frac{V^{-}-V_{o}-}{R_{f}}=-\frac{V_{o}}{R_{f}}$$
But: $I_1=I_{f}$

Thus:

$$\frac{V_{in}}{R_{in}}=-\frac{V_{o}}{R_{f}}$$

and finally for the **transfer function:**
$$\frac{V_{o}}{V_{in}}=\frac{-R_{f}}{V_{o}}$$

For the love of god
Derive this thing.
Its not hard.


Thus, The closed loop voltage gain of the inverting amplifier is given by:$$A_{CE}=-\frac{R_{f}}{Ri}$$And thus, for a sinusoidal input signal, the output signal is phase-shifted by $180\degree$. 
Also the **inverting input** provides **negative feedback**.

Now imagine the same scenario with an **practical op-amp** where **A is not infinite** but $R_{in}$ is **still infinite**

$V_{o}=A\left(V_{}^{+}-V^{-}\right)$
$V^{+}=0$
and thus:

$$V_{o}=-AV^{-}$$
or, usefully:

$$V^{-}=\frac{V_{o}}{-A}$$
Since $R_{in}=\infty$ then $I_{in}=0$ we can define $I_1$ and $I_f$

$I_1=\frac{V_{i}-V^{-}}{R_1}=\frac{V_{i}-\frac{V_{o}}{-A}}{R_1}$

$I_{f}=\frac{V^{-}-V_{o}}{R_{f}}=\frac{\frac{V_{o}}{A}+V_{o}}{R_{f}}$

$\frac{V_{o}}{A}+V_{o}=-\frac{R_{f}}{R_1}\left(V_1+\frac{V_{o}}{A}\right)$

And **FINALLY**, **transfer function**

$$\frac{V_{o}}{V_{\in}}=-\frac{R_{f}}{R_1}\centerdot\frac{A}{\left(1+\frac{R_{f}}{R_1}\right)+A}$$
This is also easily derivable using first principles (mainly ohm's law and one of the op-amp properties).