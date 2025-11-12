The steps to take to do a hypothesis test,
given that 
$\bar{x}=75.48$
$\sigma=14.71$
$n=33$

1. Write Null and alternative hypotheses
$$
\begin{gather}
&H_{0}:\mu=80 \\ &H_{A}:\mu \neq 80
\end{gather}
$$
2. Establish a normal distribution centerd about the null value in $H_0$, with a width of $se(\bar{x})$. $\mu=80$ 
$$
se(\bar{x})=\frac{14.71}{\sqrt{ 33 }}
$$
3. Indicate $\bar{x}$ on the figure $\bar{x}=75.48$
4. Find the area past $\bar{x}$ in the direction of $H_{A}$ inequality $(\neq \text{is } < \text{ and }>)$. This area is $\alpha$ or the p-value.
	1. If the p-value is < 0.05, this constitutes sufficient evidence to reject the null in favor of the alternative.
	2. If the p-value is > 0.05, the likelihood of a type I error is too great and we fail to reject the null.

---


![[Pasted image 20251112094135.png]]
![[Pasted image 20251112094224.png]]
small p-value means we should go with the alternative, since we have a higher chance of being right, (Reject the null in favor of the alternative)

A large p-value means that the data does not strongly support the alternative, and we should stay with null. (Fail to reject the null)

###### Example 1
The claim is that the average is less than 80. 
$$
\begin{gather} 
H_{0}:&\mu=80 \\
H_{A}:&\mu<80 \\
P(\bar{x}<75.48)&=0.039
\end{gather}
$$
since the p value is 0.039, and is less than 0.05, we can say that we reject the null in favor of the alternative. The evidence supports the claim that the mean is less than 80. The likelihood we are wrong in the our claim is p=0.039

###### Example 2
The claim is that the average is more than 80
$$
\begin{gather} 
H_{0}:&\mu=80 \\
H_{A}:&\mu>80 \\
P(\bar{x}>75.48)&=0.961
\end{gather}
$$
since the p value is vert high, we fail to reject the null. The likelihood we are wrong when we claim the mean is greater than 80 is quite high, p=0.961 