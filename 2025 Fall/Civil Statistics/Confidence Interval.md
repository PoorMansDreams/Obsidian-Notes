#probability 

the equation for a 2-sided confidence interval is
$$
\begin{align}
&\bar{x} \pm z_{\alpha/2}\left( \frac{\sigma}{\sqrt{ n }} \right) \\
&\bar{x} \pm z_{\alpha/2} se(\bar{x})
\end{align}

$$
The $\bar{x}$ is the average/mean of the equation, and $z_{\alpha/2}$ is simply the probability $\alpha$ divided by 2, and then run in `norm.s.inv(alpha/2)` this will give us a z value given probability. Our upper bound will be our mean/average plus the right side, and our lower bound will be the mean/average minus the right side. 

A one sided confidence interval looks very similar, 
$$
{x} \pm z_{\alpha}\left( \frac{\sigma}{\sqrt{ n }} \right)
$$
If we wanted a 95% confidence interval, our $\alpha$ will be $1-0.95=0.05$

we can use `=CONFIDENCE.NORM(alpha,stndDev,SampleSize)` 

Note that excel will automatically do a 2 sided interval, so keep alpha as is. 