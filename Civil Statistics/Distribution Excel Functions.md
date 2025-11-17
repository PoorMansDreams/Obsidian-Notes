![[Pasted image 20250924102239.png]]


###### calculate the probability of exactly 4 successes in 100 trials, with a 0.5% chance of success on each trial.

`=BINOM.DIST(4, 100, 0.005, FALSE)`
`=BINOM.DIST(successes, Trials, Probability, T/F)` 
`=BINOM.DIST.RANGE(Trials, Probability, a, b)` 

Use Cumulative if X<=x

###### What is the probability that you will need to interview exactly 15 unqualified candidates before you find all 10 qualified ones? Probability to find a qualified person is 30%

 `=NEGBINOM.DIST(15, 10, 0.3, FALSE)`
 `=NEGBINOM.DIST(fails, success, probability sucess, T/F)`
 
###### finding the probability of drawing exactly 3 black cards (K=26) in a 5-card hand (k=3, n=5) from a standard 52-card deck (N=52). The Excel/Sheets formula would be 

ww(3, 5, 26, 52, FALSE)`

###### in a basket of 10 red and 5 blue balls, find the probability of drawing exactly 3 red balls when selecting 4 balls without replacement

`HYPGEOM.DIST(3, 4, 10, 15, FALSE)`
`HYPGEOM.DIST(success, sample size, success size, fail size, FALSE)`

###### Poisson Dist Tells us Number of events in a fixed interval of time or space  

`=POISSON.DIST(x,mean,T/F)`
`=POISSON.DIST(Number of Events, Expected numeric Value ,T/F)`
