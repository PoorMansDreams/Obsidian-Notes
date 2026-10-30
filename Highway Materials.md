- Two types of pavement 
	- Flexible Pavement
		- Made of bitumen material (from oil processing)
		- Strong surface layer, impermeable so water does not seep in. 
		- Softer, to drive on used widely
	- Rigid Pavement 
		- Concrete slabs with steel reinforcement
		- More expensive than flexible pavement
		- Used in airports and highways

- Types of Rigid pavement
	- Jointed Plain Concrete Pavement (JPCP)
		- Joint spacing of 15-20 feet, has longitudinal bars/dowels to connect the segments of slabs together 
	- Jointed Reinforce Concrete Pavement (JRCP)
		- JRCP includes steel reinforcement mesh within the slabs, allowing for larger slab sizes (joint spacing of 30-100 feet)
	- Continuously Reinforced Concrete Pavement 
		- No dowels needed, no transverse joints. Steel goes all the way through the whole slab. 

##### AASHTO Flexible Design method
- Design Parameters
	- Design Traffic
	- Reliability
	- OVerall Standard Deviation
	- Effective $M_{r}$ of Subgrade Soil
	- Design Serviceability Loss $\Delta$PSI 

$M_{r}$ is the Resilient Modulus, we want to find the effective $M_r$ 
We will estimate the relative damage, $u_{f}$ we use the equation

$$
u_{f}=1.18\times 10^8 \times M_{r}^{-2.32}
$$
The relative damage will determine how high the resilient modulus will need to be. (In PSI)

we find the relative damage $u_{f}$ for each month and average them. In the problem, we get a $u_{f}$ of **1.73**. Now we plug it into the equation.

$$
\begin{align}
1.73&=1.18\times 10^8 \times M_{r}^{-2.32} \\
M_{r}&=\left(  \frac{1.73}{1.18\times 10^8} \right)^{\frac{1}{-2.32}}
\end{align}
$$

To find traffic after a set amount of year, then we can use the compounded traffic growths
$$
C=P(1+r)^n
$$
We will be given a table that gives us TSI/$p_{t}$

Calculate the total daily ESAL of the traffic-loading data for flexible pavement with structural number SN=5.0. The Design terminal serviceability index for both pavements is 2.5. 

we will be given the axle load in kips, and number of axles per day. 
Looking at the table, we use the SN number (5) and the axle load in kips, it will then give us the ESAL factor. We multiply the ESAL factor with the number of axles per day, the product will be the ESAL. We then do this for the rest of the axle loads and sum it all up. 


| Axle Load | No. Axles per Day | ESAL factor (Table) | ESAL (No. Axle times ESAL Fac.) |
| --------- | ----------------- | ------------------- | ------------------------------- |
| 2 kip     | 1438              | 0.0002              | 0.2876                          |
| 4 kip     | 3391              | 0.002               | 6.782                           |
| 6 kip     | 3432              | 0.01                | 34.32                           |
| 8 kip     | 6649              | 0.034               | 226.066                         |
|           |                   |                     | **Total=267.5**                 |

---
The daily ESAL computed in example 10 (412.2) is based on the intitial traffic estimate. The annual growth of traffic 3%. The expressway is to be constructed of flexible pavement. The predicted ESAL (X10^6) for a service life of 30 years is most nearly...? 

First, make sure that ESAL is in **years** so we multiply 412.2 by 365 days to convert to years, so ESAL (yearly) is 150453.


$$
\begin{align}
\text{ESAL in } t \text{ years}=\text{Initial ESAL} \times\text{Total Growth Factor} \\
150453\times \frac{(1+0.03)^{30}-1}{0.03}=7.156\times 10^6
\end{align}
$$

