This is an algebraic method that provides information on the **absolute stability** of an LTI system that has a characteristic equation with constant coefficients. This criterion **tests if any root lies on the right half of the s-plane** and also indicates the **number of roots lying on the j$\omega$ axis** and in the right half s-plane

I have a transfer function with the following denominator:

$$2s^4+s^3+3s^2+5s+10=0$$
![[Pasted image 20241125121226.png]]
In this example there were 2 changes in sign in the first column, and therefore 2 unstable poles. 



Is this system **stable**?

You can stop till the row $s^2$ because there is a change in sign from $-1$ to $-7$ and thus is unstable.

here is another case with zeros:

![[Pasted image 20241125122610.png]]

When you get a zero in the first column, replace with $\epsilon$
Assume $\epsilon$ is a very VERY small negative number. For $s^1$ $2-\frac{3}{\epsilon}$ becomes a very very large negative number (as $\frac{1}{0}$ ) tends to $\infty$ 

In the case where you get an all zero row, Consider the previous row and populate it with the row's respective power, skipping one power for each term

In this case the row for $s^1$ becomes $4s^2 + 4$ 
next, calculate the derivative:
$$\frac{d}{ds}[4s^2+4]=8s^{'}$$ Then substitute the result into the next term.
![[Pasted image 20241125124600.png]]


I have a transfer function, and I want to find the values of k for which system is stable.

$\frac{C}{R}=\frac{K}{s\left(s^2+s+1\right)\left(s+2\right)+K}$

Take denominator to form the characteristic equation
$$s^4+3s^3+3s^2+2s+K =0$$
For a system to be stable, $K> 0$ 

 $$\frac{\frac{14}{3}-3k}{\frac{7}{3}}>0$$
 
 $$\frac{14 - 9k}{7}>0 $$
 $$14-9k>0 $$
 $$\frac{14}{9}>k$$
 