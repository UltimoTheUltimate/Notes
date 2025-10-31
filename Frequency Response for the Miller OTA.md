draw the ac equivalent circuit:

ins img

pole frequency at node 2:

fp2 = 1/2piReffCeff
where Reff = ac resistane from node 2:
therefore reff = rds2//rds4=1/gds2+gds4
Ceff is the effective capacitance from node 2 to gnd. Ceff = CcAv2


Non Dominant Pole:
Consider the non dominant pole at the output node 2:
Assuming that fnondominant is at a high frequency, the reactance of Cc -> 0\ohm, i.e. consider Cc as a short circuit.

f_nd = 1/2piReffCeff

At node 3: Ceff = C_L + C_C + Cn3
However at fnd, Cc is a short circuit and Ceff \approx C_L
(Cn3 << CL)

Reff is the ac resistance from node 3 to ground

Draw the AC equivalent Circuit:

ins img.
To find rout at node 3, apply Vx at the node and find the current ix drawn by the node. Then, with the condition that the external voltage source (vi1-vi2) is shorted and remembering that Cc is shorted

Vx = (ix-gm6Vgs6)/gds2+gds4+gd5+gds6

From the AC equivalent circuit it can be seen that
V1 = Vx
Vx = ix - gmvx/gds2+gds4+gds5+gds6

ix = vx(gds2+gds4+gds5+gds6)+vxgm6
therefore rout = vx/ix=1/gds2+gds4+gds5+gds6+gm6

but gm >> gds  therefore rout = 1/gm6

therefore fp3 = 1/2pi.1/gm6.C_l=gm6/2piCL

where fp3 = fnd

A more Exact Analysis yields:
fp3=gm6/2piCL(1/1+Cn2/CL+Cn2/Cc)

Gain Bandwidth GBW = Avo x fd
where
Avo equiv low frequency voltage gain
avo=gm2/gds2+gds4.gm6+gds5+gds6
fd=gds2+gds4/2piCcAv
GBW=gm2/wpiCc

Phase Margin:
PM = 90deg-tan-1(GBW/fnd)

Taking into consideration the zero that arises with differential amplifiers:

PM = 90deg - tan-1(GBW/fnd)+tan-1(GBW/2fnd) <--zero
