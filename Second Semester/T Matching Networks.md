Skeleton Notes Example:

Design a T-type matching network that transforms a load impedance Z_l=60-j30/Omega into an input inpedance of 10+j20/Omega and has a maximum nodal quality factor of 3.

Z_L = 60-j30/Omega
Zs^* = 10+j20/Omega

Normalizing impedances by 50\Omega:

Z_L' = 60-j30\Omega/50\Omega = 1.2-j0.6

Z_S*' = 10+k20\Omega/50\Omega = 0.2+j0.4

from smith chart:

C1: 1.2-j0.6 -> 1.2-j1.0
\Delta = 0.4 x 50 = 1/2pifC1

C1 = 1/2pifx0.4x50
C1 = 7.96pF
C2:

0.5-j0.4 -> 0.5 - j1.5
\Delta = 1.1

1/1.1x50 (as it is on admittance circles) = 1/2pifC2

C2 = 1.1/2pifx50
C2 = 3.5pF


L3 => 0.2 -j0.6 -> 0.2 + j0.4
\Delta = 1 1x50 = 2pifL3
L3 = 50/2pix1GHz
L3 = 7.96nH

