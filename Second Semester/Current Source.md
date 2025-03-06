(or current sink)

A current source/ current sink provides  a constant DC biasing current for a circuit. 

The simplest current source is an ideal MOS transistor operating in pinch-off.

In a practical MOS  operating in pinchoff, the AC output resistance is not infinite but close to M$\Omega$. This is represented by $r_{ds}$ 

The target of a current Source is toi have $r_{out}\rightarrow \infty$

The AC output resistance $r_{out}$ can be increased by connecting a resistance $R$ between source and ground. 

In order to find the AC output resistance, draw the AC equivalent circuit of the current source:

Next: apply an ac external voltage  $v_x$ at the output node () and find the current $i_x$ drawn by the circuit 

with two conditions:
1. any external voltage source must be short-circuited
2. any external current source must be open-circuited


then the ac output resistance is obtained from:
$$r_{out}=\frac{v_x}{i_x}$$



(insert math)

if R can be replaced by a transistor M2, hence, $R_{out}=(1+g_{m1}R)r_{ds2}$   