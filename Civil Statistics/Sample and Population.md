
Adult females have a pulse rate that is normally distributed with a mean of 74.0 beats per minute and a standard deviation of 12.5 beats per minute. 

If 16 adult females are randomly selected, find the probability that they have pulse rates with a mean less than 80 beats per minute 

`=Norm.DIST(80,74,12.5,TRUE)` Pretty simple, 

 If 16 adult females are randomly selected, find the probability that they have pulse rates with a mean less than 80 beats per minute

Since we're being asked from a sample of 16, we need to adjust our Standard Deviation 
$$
\sigma_{x}=\frac{\sigma}{\sqrt{ n }}
$$
where $n$ is the population size, so 
$$
\sigma_{x}=\frac{12.5}{\sqrt{ 16 }}= 3.125
$$
`=Norm.DIST(80,74,3.125,TRUE)`
