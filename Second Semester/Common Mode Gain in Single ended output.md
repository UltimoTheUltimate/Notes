Consider the differential amplifier with an ac voltage V_c applied to both transistors M1 and M2.

![[Pasted image 20251017101119.png]]

The single ended output, common-mode input voltage gain A_CS = v_o1/v_c = vo_2/c 

Draw the ac equivalent circuit:
![[Pasted image 20251017103733.png]]
Note that in the case of a Common Mode input, v_x is not 0.
v_C = v_gs1 + v_x
or v_C = v_gs2 + v_x

Assume that rds1 and rds2 are significantly large.
therefore assume that no current flows.

The approxmiate ac equivalent circuit becomes:
![[Pasted image 20251017103749.png]]
considering the above circuit, vx becomes:

V_x = = gm1vgs1rds7 + gm2vgs2rds7 
and assuming M1 and M2 are matched: (gm1 = gm2)

and since vgs1 = vgs2
the vx = 2gm1vgs1rds7
But vgs1 = vc - vx
vc = vgs1 + vx
vc = vgs1 + 2gm1vgs1rds7
therefore vc = vgs1(1+2gm1rds7)
therefore vgs1 = vc/1+2gm1rds7
vo1 = -gm1vgs1R
= -gm1RVc/1+2gm1rds
