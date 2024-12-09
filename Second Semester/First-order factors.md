**Magnitude** $\left|\frac{1}{j\omega}\right|_{dB}=\left|\left(j\omega\right)^{-1}\right|_{dB}=20\log\left|\left(j\omega\right)^{-1}\right|=20\log\left(\omega\right)$
![[Pasted image 20241202125645.png]]
This gives a straight line with a gradient of -20dB/dec passing through $\omega$ =1rad/s
**Phase** $\angle\frac{1}{j\omega}=\angle1-\angle j\omega=-\angle j\omega=-\tan^{-1}\left(∞\right)=-90$
![[Pasted image 20241202125657.png]]
$\left(j\omega+A\right)$ Factor
In this case factor out the constant such that $$A\left(1+\frac{j\omega}{A}\right)=A\left(1+j\omega T\right)$$where $T=\frac{1}{A}$
constant A will be grouped together with any other constants in $H\left(\omega\right)$
Therefore, we are now interested in the Bode Plot of $1+j\omega T)$

- **Magnitude**: 
- $20\log\left|1+j\omega T\right|=20\log\left|\sqrt{1+\omega^2+T^2}\right|$
- For $\omega T\ll1\left|1+j\omega T\right|_{dB}\approx20\log1=0dB$
- For $\omega T\gg1\left|1+j\omega T\right|dB=20\log\sqrt{\omega^2T^2}=20\log\left(\omega T\right)$
- $\left|1+j\omega T\right|_{dB}=20\log\left(\omega\right)+20\log\left(T\right)$

this represents the equation of a line having a gradient of 20dB/dec and a y intercept at$20\log\left(T\right)$ 
This line cuts the $x$ axis when: $20\log\left(\omega\right)+20\log\left(T\right)=0$
$\log\left(\omega\right)=-\log\left(T\right)=\log\left(T^{-1}\right)$
$\omega=\frac{1}{T}$

This frequency represents the intersection between the two asymptotes and is generally called the break or corner freq.

![[Pasted image 20241202132150.png]]
The magnitude resp of $\left(1+j\omega T\right)$ is given by the bode plot is just on asymptotic approximation

**Phase**$\angle\left(1+j\omega T\right)=\tan^{-1}\left(\frac{\omega T}{1}\right)=\tan^{-1}\left(\omega T\right)$

$\omega T\ll1\longrightarrow{}\angle\left(1+j\omega T\right)\approx\tan^{-1}\left(0\right)=0\degree$
$\omega T\gg1\longrightarrow{}\angle\left(1+j\omega T\right)\approx\tan^{-1}\left(\infty\right)=90\degree$
$\omega T=1\longrightarrow{}\angle\left(1+j\omega T\right)\approx\tan^{-1}\left(\frac{1}{T}\cdot T\right)=45\degree$
![[Pasted image 20241202132947.png]]
$\frac{1}{1+j\omega T}$ Factor

**Magnitude** $\left|\frac{1}{1+j\omega T}\right|_{dB}=20\log\left|\left(1+j\omega T\right)^{-1}\right|=-20\log\sqrt{1+\omega^2T^2}=-10\log\left(1+\omega^2T^2\right)$

If $\omega T\ll1\longrightarrow{}\left|\frac{1}{1+j\omega T}\right|_{dB}=-10\log\left(1\right)=0dB$
If $\omega T\gg1\longrightarrow{}\left|\frac{1}{1+j\omega T}\right|_{dB}=-10\log\left(\omega^2T^2\right)=-20\log\left(\omega T\right)$
If $\omega T=1\longrightarrow{}\left|\frac{1}{1+j\omega T}\right|_{dB}=-20\log\left(\omega\right)-20\log\left(T\right)$

This line cuts the $x$ axis when $$-20\log\left(\omega\right)-20\log\left(T\right)=0$$
$$\omega=\frac{1}{T}=\omega cf$$
![[Pasted image 20241202134412.png]]
**Phase** $\angle\frac{1}{1+j\omega T}=-\tan^{-1}\left(\omega T\right)$

If $\omega T\ll1\longrightarrow{}\angle\frac{1}{1+j\omega T}\approx-\tan^{-1}\left(0\right)=0\degree$
$\omega T\gg1\longrightarrow{}\angle\frac{1}{1+j\omega T}=-\tan^{-1}\left(\infty\right)=-90\degree$
$\omega T=1\longrightarrow{}\angle\frac{1}{1+j\omega T}=-\tan^{-1}\left(1\right)=-45\degree$

![[Pasted image 20241202134425.png]]

[[exampleBode]]
