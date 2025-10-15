#probability 
If we are given something like, 3 test are equally weighted, and all the tests are normally distributed, with the following recorded:
Test 1: $X_{1}:\mu=70\text{ and } \sigma=8$
Test 2: $X_{2}:\mu=65\text{ and } \sigma=12$
Test 3: $X_{3}:\mu=68\text{ and } \sigma=6$

If a student is selected at random, what is the probability that they pass the course with at least a 70?

so since there are 3 tests with normal distributions, we can say that the total probability is simply
$$
Y=\frac{1}{3}X_{1}+\frac{1}{3}X_{2}+\frac{1}{3}X_{3}
$$
and we want $P(Y\geq 70)$
to do this, we can do Linear Transformation, which is like adding up all the variance and means
$$
\mu_{Y}=c_{1}\mu_{1}+c_{2}\mu_{2}+c_{3}\mu_{3}
$$
$$
\mu_{Y}=\frac{1}{3}(70)+\frac{1}{3}(65)+\frac{1}{3}(68)=67.67
$$

$$
\sigma^2_{Y}=c_{1}^2\sigma_{1}^2+c_{2}^2\sigma_{2}^2+c_{3}^2\sigma_{3}^2
$$
$$
\sigma^2_{Y}=\left( \frac{1}{3} \right)^2(8^2)+\left( \frac{1}{3} \right)^2(12^2)+\left( \frac{1}{3} \right)^2(6^2)=27.11
$$
$$
\sigma_{Y}=\sqrt{ 27.11 }=5.21
$$
$$
\mu_{Y}=67.67
$$
now we simply calculate in excel,
![[Pasted image 20251015132834.png]]