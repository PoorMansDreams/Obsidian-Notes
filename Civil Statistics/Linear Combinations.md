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

##### Homework Examples
The width of a casing for a door is normally distributed with a mean of 24 inches and a standard deviation of 1/8 inch. The width of a door is normally distributed with a mean of 23-7/8 inches and a standard deviation of 1/16 inch.
1. Determine the mean of the difference between the width of the casing and the width of the door.
$$
24-23 \frac{7}{8}=\frac{1}{8}=0.125
$$
2. Determine the standard deviation of the difference between the width of the casing and the width of the door.
$$
\text{Var(C-D)}=\text{Var(C)}+\text{Var(D)}=\sigma^2_{C}+\sigma^2_{D}=\left( \frac{1}{8} \right)^2+\left( \frac{1}{16} \right)^2=\frac{5}{256}
$$
$$
\sigma_{C-D}^2=\frac{5}{256}
$$
$$
\sigma_{C-D}=\sqrt{ \frac{5}{256} }=0.139754
$$

The Combination we made describe the DIFFERENCE between the door and the casing. 

3. What is the probability that the width of the casing minus the width of the door exceeds 1/4 inch?

Use P(X>1/4), This is asking for the case in which the difference (X) is greater than 1/4 inches. 
Use previous terms, (Diff in width casing and door, Diff in standard deviation) and plug them into `=NORM.DIST(X, mean, stardard_deviation, TRUE)` With X being 1/4. We want when X is greater than, and the excel function gives us things in LESS THAN form, so we just subtract 1
$$
1-P\left( X< \frac{1}{4} \right)=1-0.814453=0.185547
$$
4. What is the probability that the door does not fit in the casing?
Only time the door does not fit the casing is when the door is bigger than the casing, if that's the case, the difference would be negative. so P(X<0), using excel, `=NORM.DIST(X, mean, stardard_deviation, TRUE)` 
$$
P(X<0)= 0.185547
$$

---

Assume that the weights of individuals are independent and normally distributed with a mean of 160 pounds and a standard deviation of 30 pounds. Suppose that 25 people squeeze into an elevator that is designed to hold 4300 pounds. 

1. What is the probability that the load (total weight) exceeds the design limit?

Question indicates that this wants the SUM of all the weights, so our mean would be sum of all the means, which is just 25 of the 160lb
$$
\mu_{T}=25\times 160=4000\text{ lb}
$$
Variance is the same, but remember that its squared
$$
\sigma_{T}^2=25\times 30^2
$$
$$
\sigma^2_{T}=\sqrt{ 25\times 30^2 }=150
$$
We need probability that exceeds 4300, P(X>4300)
using excel,
$$
1-P(X>4300)=0.02275
$$
2. What design limit is exceeded by 25 occupants with probability 0.0001?
Use excel function `=NORM.INV(probability, mean, standard_deviation)` = 4557.8 lb
for probability, we need to do 1-0.0001 to obtain the right side of the standard deviation curve.

---

A U-shaped component is to be formed from the three parts A, B, and C. The picture is shown below. The length of A is normally distributed with a mean of 10 millimeters and a standard deviation of 0.1 millimeter. The thickness of parts B and C is normally distributed with a mean of 2 millimeters and a standard deviation of 0.05 millimeter. Assume all dimensions are independent.



1.  Determine the mean of the length of the gap D (in mm).
The gap can be represented as 