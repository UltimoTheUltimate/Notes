Consider M3 and M4, which are diode connected as the active loads, Differential Mode Analysis

The differential mode ac voltage gain is:

Avdd = vo1 - vo2/vi1-vi2 equiv vo1-vo2/vid
recalling previous result:
Avdd = -gm1(rds1//rds3//1/gm3)

and since 
1/gm << rds
then Avdd = -gm1/gm3

Avdd = -sqrt(2K'n(w/L)1 (IB/2))/sqrt(2K'p(W/L)3(IB/2))
Avdd = -sqrt(k'n/k'p(W/L1)/(W/L3))
AC output resistance for differential output rout  = rout1 + rout2, where rout1 = rds1 // rds2 // 1/gm3
approx 1/gm3
therefore rout = 1/gm3 + 1/gm4
rout = 2/gm3
M3 and M4 are matched

Current Sources as active loads:

M3 and M4 are now transistors in pinchoff acting as current-source active loads, again, M3 and M4 are matched.
Differential mode operation, i.e. differential input differential output.
![[Pasted image 20251017112020.png]]
Avdd = -gm1(rds1//rds3)
= -gm1/gds1+gds3


in terms of design parameters:

A_vdd = -sqrt(2k'nw/l(IB/2))/lambdan(IB/2)+lambdap(IB/2)

= -sqrt(2K'nW/L1/IB/2)/lambdan+lambdap
 
 Therefore:
 Av prop sqrt W/L1
 and 
 Av prop 1/sqrtIB
in order to increase avdd, w/L1 can be increased resulting in larger silicon and/or dc biasing current Ib decreased. 

 Note that decreasing Ib results also in decreasing the dc power dissipation needed for the differential amplification to operate
 P_dc = Vdc . Idc
 Pdc = Vdc . IB
 ac output resistance differential output rout = rout1 + rout2
 where rout1 = rout2 = rdc1//rds2
 Common mode voltage gain Acs = -gm1

 Acs = V_O1/V_CM
 =-gm1R/1+2gm1rds7
 Acs is now given by:

 acs approx -rds3/2rds7(21) 

 CMRR = |Avds|/|Acs|
 Where avds is the differential input single-ended output voltage gain, 
 and thus Avds = 1/2Avdd
 therefore Avds = -1/2(gm1/gds1+gds2)
 CMRR = 1/2 gm1/gds1+gds3 . 2rds7/rds3

 CMRR  approx gm1gds3rds7/gds1+gds3


 Differential Amplifier with current Mirror Load
 ![[Pasted image 20251017114302.png]]
 M3,M4 form a  current mirror acting as the active load of M1,M2. Note that the output is now single-ended.

 AC Voltage gain:
 Avd = vo/vi1-vi2 = vo/vid
 Draw the AC equivalent circuit:
![[Pasted image 20251017115927.png]]

 M1 matched with M2, M3 matched with M4
 also Vgs4 = Vgs3

 Vo = -(gm2Vgs2+gm4Vgs4)(rds2//rds4)

 remember: for a differential input Vid, vgs1 = vid/2, vgs2=-vid/2

 Also: Vgs4= -gm1vgs1(rds1//rds3//1/gm3) approx eq -gm1vgs1/gm3

 therefore vo = -[gm2(-vid/2)+gm4(-gm1/gm3. vid/2)](rds2//rds4)
 = gm2vid/gds2+gds4

Avd = gm2/gds2+gds4
In terms of design parameters:
Avd = sqrt(2k'nw/L2IB/2)/(lambdan+lambdap)(IB/2)


