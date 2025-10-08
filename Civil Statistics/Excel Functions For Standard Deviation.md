#probability 
```
=STANDARDIZE(X, mean, standard_deviation)
```
Gives us $Z$ in $Z=\frac{X-\mu}{\sigma}$

```
=NORM.S.DIST(Z,TRUE)
```
Gives us the Probability when we input $Z$


```
=NORM.DIST(X, mean, stardard_deviation, TRUE)
```
Gives us probability directly, given $X$ 
(basically combines standardize and norm.s.dist funct)

```
=NORM.S.INV(Probability)
```
Gives us $Z$ when we give probability

```
=NORM.INV(probability, mean, standard_deviation)
```
Gives us $X$ directly given probability
(0.955-0.683)/2=