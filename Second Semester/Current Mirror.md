Consider the circuit of the simple current mirror shown.

It consists of two transistors with their gates connected together and their sources connected also together such that $V_{GS1}=V_{GS2}$ in addition the transistor at the input side is diode connected.

This ensures that $M_1$ operates in pinch-off.

For a constant $I_D$ when $V_{GS}$ increases $V_{DS}$ decreases, when $V_{GS}$ decreases, $V_{DS}$ increases.

by using a current mirror we need to ensure that the transistor $M_2$ always operates in pinch-off. The limit for $M_2$ to operate in pinch-off is given by $$V_{DG2} = -V_T$$ $$V_{DS2}=V_{GS2}-V_T $$
The minimum value of $V_{out}$ which ensures that $M_2$ operates in pinch-off is called $V_{min}$  Note that $V_o=V_{DS2}$ 

including $V_{SS}$: 

$$V_o=V_{DS2}+V_{SS}$$
If the aspect ratios of $M_1$ and $M_2$ are equal, then for ideal transistors:

$$I_{in}=\frac{K'}{2}\frac{W}{L}_1(V_{GS1}-V_T)^2$$
$$I_{in}=\frac{K'}{2}\frac{W}{L}_2(V_{GS2}-V_T)^2$$
$$\therefore \frac{I_{out}}{I_{in}}=\frac{\frac{W}{L}_2}{\frac{W}{L}_1}$$
But since aspect ratios are equal then

$$I_{out}=I_{in}$$
since $V_{GS1}=V_{GS2}$ for a current mirror

In the general case where $\frac{W}{L}_2 \neq \frac{W}{L}_1$

for ideal transistors:

$$\frac{I_{out}}{I_{in}}=\frac{\frac{W}{L}_2}{\frac{W}{L}_1}$$

Characteristics of a current mirror

Four parameters characterise the operation of a current mirror:

Ideally the ratio of output to input should depend only on $\frac{W}{L}_1$ $\frac{W}{L}_2$

AC input resistance should be low --> zero
ac output resistance should be high
$V_{min}$ should be as low as possible


In practice:

$$\frac{I_{out}}{I_{in}}=\frac{\frac{K'}{2}_2(V_{GS2}-V_T)^2(1+\lambda V_{DS2})}{\frac{K'}{2}_1(V_{GS1}-V_T)^2(1+\lambda V_{DS1})}$$
$$\therefore \frac{\frac{I_{out}}{I_{in}}=\frac{W}{L}_2(1+\lambda V_{DS2})}{\frac{I_{out}}{I_{in}}=\frac{W}{L}_1(1+\lambda V_{DS1})}$$

AC input resistance $r_{in}$

The AC resistance of a "diode connected" MOS transistor is R_DS in parallel with $\frac{1}{g_m}$ and since $\frac{1}{g_m}<<r_{ds}$ then:
$$r_{in}\approx \frac{1}{g_m}$$
AC output resistance $r_{out}$


V_{Min}
Limiting current for $M_2$ to current in pinch-off: $V_{DS2_{sat}}$

$$V_{DS2_{sat}}=V_{GS2}-V_T$$

$V_{min}$ is the limit of $V_o$ to remain in pinch-off 

\begin{centre} $\therefore$ for $V_{SS}=0V$$ 
\end{centre}
$V_o=V_{DS2_{sat}}$

$I_{out}=\frac{K'}{2}\frac{W}{L}_2(V_{GS}-V_T)^2$

to a first approximation (the ideal simulation)

$$V_{GS2}-V_T=\sqrt{\frac{2I_{Out}}{K!\frac{W}{L}_2}}$$

Alternatively,

$$(V_{GS2}-V_T)^2=(V_{GS1}-V_T)$$

and

$$V_{GS1}-V_T=\sqrt{\frac{2I_{in}}{K!\frac{W}{L}}}$$
In practice the simple current mirror operates with $V_{DS2}\neq V_{DS1}$ 

In order for $V_{DS2}\rightarrow V_{DS1}$


The cascode current mirror is used
[[Cascode Current Mirror]]
[[Current Mismatches]]
