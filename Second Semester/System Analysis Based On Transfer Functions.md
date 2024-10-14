$$G\left(s\right)=\frac{K\left(s+z_1\right)\left(s+z\right)\ldots\left(s+z_{n}\right)}{\left(s+p_1\right)\left(s+_{}p_2\right)\ldots\left(s+p_{n}\right)}$$

This, is a transfer function with numerator and denominator consisting of polynomials:

The roots at the **Numerator** are called Zeroes
The roots at the **Denominator** are called Poles

To get **Zeros**, Equate **Numerator** to Zero and **Solve**
To get **Poles**, Equate **Denominator** to Zero and **Solve**

Poles And Zeros can be real, imaginary or complex, and each type has an affect on the system itself

Consider This example:
$$G_{\left(s\right)}=\frac{a}{s+6}$$
There are **no zeroes** as s is not present
However, there is **one pole** at $s = - 6$ 

How about This example:

$$G_{\left(s\right)}=\frac{s+2}{\left(s+3+j\sqrt6\right)\left(s+3-j\sqrt6\right)}\frac{}{}$$
There is **one zero** at $s = -2$
There are **2 poles** at $s=-3+j\sqrt6$ **and** $s=-3-j\sqrt6$

[[System Behaviour Based On Poles]]

In first order systems the transfer function is:
$$\frac{Out_{\left(s\right)}}{In_{\left(s\right)}}=\frac{a}{s+b}$$ There is only **one pole**: $b$ 