Resistors are avoided at all cost due to noise

instead the components used are:
insuctors
capacitors

4 combinations using these

mathematical example:

(references example 1 of matching networks sheet)

insert DIAG F1

Zs = 150+j75R
ZL = 75 + j15R
f = 2GHz

values are not conjugates.

so:

1/Zs^* = 1/jX_A + 1/JX_B = 1/jXb + ZL

1/150-j75 = 1/jXA + 1/75+j15+jXb

collect Re and Im

1/150-j75 = 1/jXA + 1/75 + j(15+XB)

Rationalise:

150+j75/150^2 + 75^2 = 1/jXA + 75-j(15+Xb/75^2+(15+XB)^2)


real:
150/150^2+75^2 = 75/75^2 + (15+XB)^2

Imaginary:
75/150^2+75^2 = -1/XA -(15+XB)/75^2+(15+XB)^2

Real:

75^2+(15+XB)^2 = 14062.5
15+XB^2 = 8437.5
15+XB^2 = +- 91.856 
XB^2 = 76.86R (inductor) or -106.856R (capacitor)

for inductor:

76.86R = 2pifLb
Lb = 76.86/2pi.2GHz = 6.12nH

106.856 = 1/2pifcb

CB = 1/106.856x2pix2GHZ = 0.745pF

imaginary:

75/150^2+75^2 = -1/X_A - 15.76.86/75^2 + (15+76.86)^2

when XB = 76.86R:
XA = 108.71R


XA = 1/2pifCA
CA = 1/2pix2Gx108.71 = 0.732pF

when XB = -106.85:
75/(150^2+75^2) = -1/XA - (15-106.856)/(75^2+(15-106.856)^2)
XA = 258.71R
258.71 = 2pifLA
LA = 20.6nH

INSERT DIAGS F2