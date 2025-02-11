Why do we use op-amps?

$signal_1=useful_1+noise_1$
$signal_2=useful_2+noise_2$
$signal_1-signal_2=useful_1-useful_2+0$


An op-amp amplifies the differential signal, and eliminates the common signal (**Common Mode Signal**)

This allows it to filter out noise very effectively, as the noise is typically common across $V^{+}$ and $V^{-}$, so they cancel out.

An **operational amplifier** (op-amp) has two **input** terminals, and one **output** terminal:

![[Pasted image 20250211101811.png]]

Two signals: $V^{+}$ and $V^{-}$, are applied to the input terminal and voltage $V_o$ develops as the output where: $$V_{o}=A\left(V^{+}-V^{-}\right)$$
where A is called the open loop voltage gain.
Equation 1 can be written as: 
$$V_{o}=AV_d$$
where $V_{d}$ is called the differential input voltage: $\left(V^{+}-V^{-}\right)$.

The objective of an ideal op amp is to amplify the differential input voltage and reject voltages what are common to both inputs.


[[Properties of an Ideal op-amp]]
[[Properties of a Practical op-amp]]

In an ideal op-amp, only the differential input signal is amplified while the common mode input signal (a signal such as noise which is common to both inputs) will be eliminated

in a practical op-amp the common mode signal is not rejected completely.

CMRR

The common mode rejection ration is the parameter which indicates how well an op-amp rejects common-mode signals

CMRR = input differential signal voltage gain/ input common-mode voltage gain (4)

In an ideal op-amp,  $CMRR\to\infty$

For a practical op-amp, CMRR should still be high.

In practice, CMRR is given in Decibels where:
$$CMRR\left(dBs\right)=20\log\left(CMRR\right)$$