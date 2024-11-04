**Rule 1:** Locus End points
- The root locus starts from the poles of GH and ends at zeros of GH. If there are more poles ($n$) than zeros ($m$), then the ($n-m$) branches of the locus end at $\infty$ 
- **Proof:** 
	- Characteristic equation:
$$1+G_{\left(s\right)}H_{\left(s\right)}=0$$
$$G_{\left(s\right)}H_{\left(s\right)}=-1$$
Taking the magnitude:
$$\frac{\left(k\left|s+z_1\Vert s+z_2\right|\ldots\left|s+z_{n}\right|\right)}{}$$
**Rule 2:** Number of branches
- The number of branches in the root locus is equal to the number of poles in GH (the root locus is always symmetric about the real axis -> as complex poles exist as complex pairs)
- Proof:
	- If branches start from the poles of GH then there are as many branches as there are poles.

**Rule 3:** Real Axis 
- Any parts of the root locus on the real axis lie on the left of the odd number of poles and zeros of GH (that lie on the real axis.)

**Rule 4:**
- For large distances from the origin in the complex plane, the branches of the root locus approach a set of straight line asymptotes. The number of asymptotes is given by the difference between the number of poles n and the number of zeros m
	- number of asymptotes $=n-m$
- The angle of these asymptotes with real axis is given by $$\beta=\frac{\left(2l+1\right)}{n-m}\cdot180\degree$$
- Where $l=0,1,2,n,m-1$
- And the Intercept of the asymptotes with real axis is:
$$\sigma=\frac{\sum_{i=1}^{n}p_{i}-\sum_{i=1}^{m}z_{i}}{n-m}$$

**Rule 5:** Break-away or break-in points
- A break-point $\sigma_{b}$ is a point on the real axis where two or more branches of the root locus depart. (break away) or arrive (break-in) at the real axis. The location of the break-point can be determined by solving the following equation:
$$\sum_{i=1}^{n}\frac{1}{\sigma_{b}=p_{i}}=\sum_{i=1}^{m}\frac{1}{\sigma_{b}=z_{i}}$$
**Rule 6:** Departure and arrival angles
- The departure angle of the root locus from a complex pole is given by:
$$\theta_{D}=180\degree+\angle GH^{D}$$
Where $\angle GH^{D}$ is the phase angle of $GH$ computed at the complex pole but ignoring the contribution of that pole. The departure angle can be calculated as follows:

- $\theta_{D}=180\degree-$ (sum of all the angles of vectors to the complex pole in question from other poles) + Sum of angles of vectors to the complex pole in question of all zeros)

- Similarly, the arrival angle of the root locus at a complex zero is given by:
$$\theta_{A}=180\degree-\angle GH^{A}$$
- Where $\angle GH^{A}$ is the phase angle of $GH$ computed at the complex zero but ignoring the contribution of that zero. The phase angle can be calculated as follows:
- $\theta_{A}=180\degree-$ (Sum of angles of vectors to the complex pole in question from other zeros)+(sum of angles of vectors to the complex pole in question from all poles)

**Rule 7:** Angle and magnitude criteria
- This rule gives the possibility of identifying:
	- Whether a point on the s-plane is on the root locus RL, for some value of k
	- The value of k at any point on the RL
- Use of **Angle Criterion** for a branch of the root locus to pass through a particular point $s_i$ in the s-plane, it is necessary that $s_i$ be a root of the characteristic equation for some real value of $k$ 
- The characteristic equation equation $GH\left(s_{i}\right)=-1$ 
- Has a phase of $\angle GH\left(s_{i}\right)=\pm l\left(180\degree\right)$ for $l=1,3,5$ 
	- Thus, a point on the s-plane is a point on the root locus, if and only if it satisfies the angle criterion. For $s_i$, to be a closed loop system, it must satisfy the magnitude criterion as well.
- Use of **Magnitude Criterion**:
	- A particular point on the root locus is a closed loop pole if the value of k at that point satisfies the magnitude condition. Conversely, the absolute value of k at any point $s_i$ on the root locus can be determined through the criterion as follows:
$$\left|k\right|=\left|\frac{1}{G\left(s_{i}\right)H\left(s_{i}\right)}\right|$$
$$\left|k\right|=\frac{\left|s_{i}+p_1\right|\left|s_{i}+p_2\right|\ldots\left|s_{i}+p_{n}\right|}{\left|s_{i}+z_1\right|\left|s_{i}+z_2\right|\ldots\left|s_{i}+z_{n}\right|}$$
**Summary:**
1. Determine the number of branches of the root locus
2. Determine the portion of the root locus on the real axis
3. Compute the centre and the angle of the asymptotes (and if any), draw them;
4. Determine the location of the break away or break in points (if any)
5. Determine the departure and arrival angles from complex poles and to complex zeros (if any)
6. Make a sketch of the branches of the root locus so that each branch of the locus originates at an open loop pole and either terminates at an open loop zero or approaches infinity along one of the asymptotes 
7. 
