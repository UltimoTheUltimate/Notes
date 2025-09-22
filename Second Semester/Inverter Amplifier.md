Consider the amplifier shown: 

where:

M1 is the driving transistor

M2 is the diode-connected transistor

and acts as an active lead

![[Pasted image 20250313100450.png]]
Both M1 and M2 are n-channel transistor

M2 is "diode connected"


$V_{Do}=V_{DS_2}+V_{out}$
$V_{out}=V_{DD}-V_{DS2}$

or

$V_{out}=V_{DS1}$

consider a DC sweep at the input:

Vin per from GND to $V_{DD}$
$V_{in}<V_{T}$
Since $V_{in}=V_{GS}<V_T$
M1 is off.

$\therefore V_{out}=V_{DD}-V_{T}$
- $V_{in}=V_T^+$
M1 switches on, in pinchoff.

- when $V_{in}$ is much higher
$I_{D}$ is much higher

$\therefore$ The "IR" drop (in $V_{DS_2}$)

across M2 ^^

V_{out} goes down
V_{DS1} goes down

when vds1 <= VGS1 - VT
m1 goes into the ohmic region
therefore vout keeps decreasing

vin = vdd

still in the ohmic region
Vout -> a few mV

Thus, the circuit operates as an inverter since when V_in is logic 0, V_out is logic 1 and when V_in is logic 1, V_out is logic 0,

When V_in = 0, V_out = V_DD - V_T
therefore note that logic 1 \ne go to VDD

when both M1 and M2 are in pinchoff, i.e. in the linear part of the transfer characteristic, the circuit is used as an analogue amplifier

The circuit operates as an analogue operator amplifier


[[Ac analysis of MOS inverting amplifier]]



