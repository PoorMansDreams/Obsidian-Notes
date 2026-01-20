#probability 

As of now we have assumed that $\sigma=s$, but this doesn't work well, especially if the sample size is less than 30. For small sample sizes, Mr. Gosset suggested using the t-distribution for better statistics. The **Student's T-Test**

The t-distribution looks a little something like this
$$
f(t)=\frac{\Gamma\left( \frac{v+1}{2} \right)}{\sqrt{ v\pi }\Gamma\left( \frac{v}{2} \right)}\left( 1+\frac{t^2}{v} \right)^{-\frac{v+1}{2}}
$$
In the image below, as $\nu\to \infty$ it approaches the standard normal z.
![[Pasted image 20251119091726.png]]

Normal distribution has a Z value that we can calculate and find through a table, but the t-distribution has more dimensions that we have to worry about. $Z=\frac{x-\mu}{\sigma}$ the normal distribution only has to worry about x. But the T-distribution also have $\nu$ and $x$. Solution is we have a table that looks like this. 

 ![[Pasted image 20251119092245.png]]

note that $\nu$ is also called degree of freedom

---

Our Confidence intervals will change because of this, with a new equation
$$
\bar{x}\pm t_{v}\left( \frac{s}{\sqrt{ n }} \right)
$$
everything is basically the same except that our $z$ value is replaced with $t$. 
and also, when finding what our $\nu$ value is, it is simply
$$
\nu=n-1
$$

We want a two sided confidence interval of 95%, given that;
$\bar{x}=702$ 
$s=54.7$
$n=5$
$\nu=5-1=4$
![[Pasted image 20251119094532.png]]

$$
\begin{align}
&702\pm 2.78\left( \frac{54.7}{5} \right) \\
&702 \pm 68
\end{align}
$$

Given $\alpha$ and the $\nu$ value, we can find $t_{v}$
`t.inv.2t(alpha,v)` 

Given $\alpha$ and the $\sigma$ and $n$ we can just calculate the complete confidence interval 
`CONFIDENCE.T(alpha, StndDev, SampleSize)`

Gives us the right tailed distribution
`=T.DIST.RT(T,v)`

Gives us the left tailed distribution
`T.DIST(T,v)`

---

We can also find a better way to hypothesis test as well, using the equation
$$
T_{0}=\frac{\bar{x}-\mu}{\frac{s}{\sqrt{ n }}}
$$
we can then put the T value $T_{0}$ into our table, and find the probability. Remember, when $p\leq0.05$ we reject the null and accept the alternate. when $p>0.05$ we cant trust the alternative so we default to the null. 

alternatively use the RT means (right side)
`=T.DIST.RT(T,v)`
function in excel, where $T_{0}$ is whatever calculated from above, and v is just $\nu$

We want a strength that is greater than 650, given
$\bar{x}=702$ 
$s=54.7$
$n=5$
$\nu=5-1=4$
$$
\begin{align}
H_{A}&: \mu>650 \\
H_{0}&:\mu \leq 650
\end{align}
$$
$$
T_{0}=\frac{702-650}{\frac{54.7}{\sqrt{ 5 }}}=2.126
$$
`=T.DIST.RT(2.126,4)`
this will give us 0.05033, we reject the null in favor of the alternative, close enough. 

---

Student's T-Test

The concrete canoe team has a second mix they are considering. First mix: $\bar{x}_{1}$ = 702 psi, $s_{1}$ = 54.7 psi  
for $n_{1}$ = 5 samples. Second mix: $\bar{x}_{2}$ = 784 psi, $s_{2}$ = 71.9 psi for $n_{2}$ = 4 samples. They would like to  
know if the second mix is statistically different from the first.

we want to test whether they are different or not, so we write our hypothesis
$$
\begin{align}
H_{0}&:\mu_{1}-\mu_{2}=0 \\
H_{0}&:\mu_{1}-\mu_{2}\not=0
\end{align}
$$
We then choose our minimum $\nu$ value, which in this case will be $\nu=4-1=3$

the t equation is long as fuck, it looks like this;
$$
t=\frac{\bar{x}_{1}-\bar{x}_{2}}{\sqrt{ \frac{s^2_{1}}{n_{1}}+\frac{s^2_{2}}{n_{2}} }}
$$
plugging in values, we get $|t|=1.88$ 

use `T.DIST.2T(1.88,3)` we get 0.156, as our p value. The p value is too high, we can't reject the null in time. 

---

To calculate the degrees of freedom from two sets, we need to use this equation
$$

df = \frac{\left(\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}\right)^2}{\frac{\left(\frac{s_1^2}{n_1}\right)^2}{n_1 - 1} + \frac{\left(\frac{s_2^2}{n_2}\right)^2}{n_2 - 1}}

$$
