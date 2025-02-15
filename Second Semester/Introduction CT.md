[[General Communications System]]

Data Can be **Analogue** or **Digital**

Here analogue can reference any value between your reference and saturation point (e.g. 0-5V)

Analogue data can be:
- Captured and converted to analogue
- sampled and converted to digital signal

Digital references either high or low (0V OR 5V or it can take up multiple levels to encode binary words)

Digital can be:
- converted to a digital signal
- modulated to an analogue signal


The goal is to transmit information to the receiver with **minimal** **distortion/deterioration**

However, we need to keep these in mind:
- Allowable transmission energy
- Available bandwidth
- Cost

For analogue, we measure performance using **SNR** (signal to noise ratio) at the receiver output

In digital systems we use probability of bit error (**bit error rate**) of the delivered data

The information sent from a digital source when the $j^{th}$ message is transmitted is given by:
$$I_{j}=\log_2\left(\frac{1}{P_j}\right)bits$$

Information changes with message since $P_{j}$'s are **not equal**

Definition: The average information measure of a digital source is:

$$H=\sum_{j=1}^{m}P_{j}I_{j}=\sum_{j=1}^{m}P_{j}\log_2\left(\frac{1}{P_{j}}\right)bits$$
where: 
- $m$ is the number of possible different source messages
- $P_{j}$ is the probability of sending the $j^{th}$ message

The **average information is called, entropy**

Example:
Consider a digital word which is **10 bits long** and each digit can take **2 possible values**. Further assume that the **probability of sending any of the two levels is equal** and that the level of each digit is **independent** of the values taken by previous digits. Find the information content of this message:

In a string of 10 symbols there are 2.2.2.2.2 = $2^{10}$

$P_{j}=\frac{1^{10}}{2}=\left(\frac12\right)^{10}$

$I_{j}=\log_2\left(\frac{1}{\left(\frac12\right)^{10}}\right)=10\log_2\left(2\right)=10$ bits $=H$

Note that all the 10 bit words give 10 bits of information because the words have the same $P_{j}$
If $P_{j}$ is not the same, some words will have more information than 10 bits while others less.

Assume half have $P_{j}=10^{-5}$ and the others have $P_{j}=1.94\centerdot10^{-3}$ find the Entropy

1024 words, 512 with $P_j = 10^{-5}$ and 512 with $Pj = 1.94\centerdot10{^-3}$
$I_1=\log_2\left(\frac{1}{10^{-5}}\right)=16.61$ bits
$H_1=512\centerdot16.61\centerdot10^{-5}=0.085$

$I_2=\log_2\left(\frac{1}{1.94\centerdot10^{-3}}\right)=9.01$ bits
$H_2=512\centerdot9.01\centerdot1.94\centerdot10^{-3}=8.95$ bits
$H=9.04$

**Maximum** entropy occurs when:
$P_1=P_2=P_3=\ldots=P_{n}=\frac{1}{n}$


Source efficiency is defined as $\frac{H}{H_{\max}}$
Observation: Entropy gives us the **minimum** number of bits needed to encode a symbol.
- Important in source coding to compress the message 
- if number of bits/symbol is less than H, then uncertainty increases and we will not be able to **distinguish** between symbols.


the source rate is given by:
$$R=\frac{H}{T}  bits/s$$
where:
$H$ is the entropy
$T$ is the time needed to send messages

- Note that these apply to **digital** sources. Analogue sources are more complex however we can approximate them using digital sources with accuracy dependent on the number of levels

$H=0$ if all $P_j = 0$ except one which has value 1 (we have no information)
The entropy when we have 2 events $x$ and $y$ is given by:
$$H\left(X,Y\right)=-\sum_{i,j}p\left(i,j\right)\log p\left(i,j\right)$$
- where $p(i,j)$ is the probability of the joint occurrence of i for the first and j for the second

$$H\left(X\right)=-\sum_{i,j}p\left(i,j\right)\log\sum_{j}p\left(i,j\right)$$
$$H\left(Y\right)=-\sum_{i,j}p\left(i,j\right)\log\sum_{i}p\left(i,j\right)$$
H(X) and H(Y) should be equal when the events are independent.


- Change to equalise probabilities increases H
- Assume that we have two chance events x and y. For a particular value i that x can take there is a conditional probability that y has value j, given by: (fix the equation)

$$p_{i}=\frac{p\left(i,j\right)}{\sum_{j}p\left(i,j\right)}$$

Conditional entropy is given by:
$$H\left(Y\left|X\right.\right)=-\sum_{i,j}p\left(i,j\right)\log p_{i}\left(j\right)$$
$$H\left(Y\left|X\right|\right)=-\sum_{i,j}p\left(i,j\right)\log p\left(i,j\right)+\sum_{i,j}p\left(i,j\right)\log\sum_{j}p\left(i,j\right)=H\left(x,y\right)-H\left(X\right)$$

How fast can we send data?

This depends on:
- Bandwidth available
- Number of levels of signals that can be used
- quality of the channel

The theoretical maximum bit rate is given by the **Nyquist** formula
$$Bit Rate=2B\log_2L\left(bits/sec\right)$$
- where B is the bandwidth of the channel (Hz) and L is the number of signal levels used to represent data

Example: Consider a noiseless channel with a bandwidth of 10kHz transmitting a signal using 8 levels. Find the maximum bit rate:


$$BitRate=2\centerdot\left(10k\right)\centerdot\log_28=60kbps$$

In practice, this maximum value will never be reached, why?

**n o i s e** 

Assume that we have only signal and white Gaussian noise

Shannon showed that channel capacity is:

$$C=B\log_2\left(1+\frac{S}{N}\right)\left(bits/sec\right)$$
where $B$ is the bandwidth in $Hz$  and $\frac{S}{N}$ is signal to noise power ratio at input of digital receiver

If the rate of information $R (bits/s)$ is less than $C$, then the probability of error approaches 0. 