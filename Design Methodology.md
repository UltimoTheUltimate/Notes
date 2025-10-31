Specifications:
Let:

GBW = 10MHz
Always design assuming:

VGS-VTN approx 0.2V
VSG - |VTP|approx 0.5V

Sm2 = 2piCc.GBW
Cc is known, or else assume:
gm2 = sqrt2kn'(W/L)2 IB/2
using ID = k`/2 W/L (VGS-VT)^2
gm=dId/dVgs = K'n(W/L)2(Vgs-VTN)

Slew Rate
The Slew Rate of the Miller OTA can be limited either internally or externally 

Consider internal limitation:

SR = dVo/dVi = IB/CC

Note: M1 On, M2 Off
Ib flows through M1

Consider now M1 off M2 On
i.e. all of Ib flows through M2:
