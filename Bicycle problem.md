#transportation 

##### Problem 1

Determine the LDS for a 1.2m wide bicycle lane at A signalized intersection, with cycle length of 110s. The bicycle gets 50s of green and carries a peak flow rate of 120 bicycles per hour.

1. Calculate the bicycle capacity at approach, the 2000 comes from a manual (average for bicycles), Given
$$
c_{i}=2000\left( \frac{50}{110} \right)=909 \text{ Bicycles/hr}
$$
2. Calculate Average control lane delay
$$
\text{Average Delay}=\frac{1}{2}C\left( \frac{\left[ 1-\frac{g}{c} \right]^2}{\left[ 1-\left( \frac{g}{c} \right) \right(\frac{v}{c_{i}})]} \right) 
$$
calculating this we get
$$
\frac{1}{2}(110)\times \frac{\left[ 1-\frac{50}{110} \right]^2}{\left[ 1-\left( \frac{50}{110} \right)\left( \frac{120}{909} \right) \right]}=17.4 \frac{\text{s}}{\text{Bicycle}}
$$

##### Problem 2

Determine the level of service for a north-south exclusive bicycle path, carries a volume of 160 bicycles/hr during peak periods. 65% of the bicycles move in the peak direction Northbound during peak periods. The path is 2.4m wide, and can be assumed to have two eff. lanes. 

$V_{o}=\text{Flow rate in bicycles in opposing directions}$
$F_{p}=0.188 \frac{L}{s}$
$F_{m}=2V_{o}$
$F=0.5F_{m}+F_{p}$
$F_{p}=\text{Passing events}$
$F_{m}=\text{Opposing events}$
$F_{vs}=\text{total number of events on path}$
$V_{s}=\text{Flow rate of Bicycles in direction}$
$V_{b}=\text{Flow rate in opposite direction}$ 

For bikes going northward,
$$
\begin{align} \\

&V_{b}(NB)=160(0.65)=104\text{ bicycles per hour} \\ 
&V_{b}(SB)=160(0.35)=56\text{ bicycles per hour} \\
&F_{p}=0.188V_{b}=0.188\times 104=20\text{ events per hour} \\
&F_{m}=2V_{b}=2\times 56=112\text{ events per hour} \\
&F=20+112=132\text{ events per hour}
\end{align}
$$
##### Problem 3

One parking lot has 100 parking stalls, occupancy rate is 60% from 8am to 5om, the place has 240 vehicles, during the same time. Estimate the turnover rate for each stall
$$
\begin{align}
&V=SOT \\
&T=\frac{V}{SO}=\frac{240}{100}=4\text{ vehicles per stall on average}

\end{align}
$$
##### Problem 4

A store approves 1500 parking stalls using the ITE ADA design guides

1. Total parking for 60" and 76" aisles
2. For $100>=100$ use 2D plus 1 for each 100 over 1000 
$$
20+\frac{\left( 1500-\frac{1000}{100} \right)}{100}=20+5=25\text{ spaces}
$$
3. for 60" aisles, $\frac{7}{8}\times 25=22$
4. for 96" aisles, $\frac{1}{8}\times 25=3$
