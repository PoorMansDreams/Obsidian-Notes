- Average End Area Method

![[Pasted image 20261001204400.png]]

Note, that the divide by 27 is to convert the units into cubic yards. This method wants us to multiply the average of the two ends with the length to find the Volume. Usually, the more sections or cuts we have, the more accurate. 

![[Pasted image 20261001204644.png]]

the first calculation, Vcut, is the length (100') times the average of the area of the first end (0) and the area of the second end (1620) for cut. Then divide by 2, and an additional 27 to convert to cubic yards.
$$
V_{cut}=100' \times \frac{(0 +1620\text{ ft}^2)}{2\times 27}=3000\text{ yd}^3
$$
---

- Earth Volume Adjustment
	- When earth is excavated, it may change the volume when it is used, 
		- Generally, freshly excavated materials decreases in volume after compaction during the construction process. The difference in volume is defined as "shrinkage"
	- When Rock is excavated, it will generally have "Swell" because it actually ends up larger.
		- When rock is broken up, air voids are introduced.
	- Example: 1 cubic yard earth is compacted to 0.8 cubic yards, $\frac{0.8}{1}=0.8$ shrinkage factor

![[Pasted image 20261001205343.png|506]]

Fill won't change from Earth Volume adjustments, but Cuts will be effected. The adjusted cut volume will be how much we would have after cutting. We do this because we usually use the extra cut material as filling material. 

![[Pasted image 20261001205537.png|512]]

In this table, the Adj. Cut-Fill tells us how much cut we have compared to how much we need to fill. Between station 0+00 and 1+00, we excavate 3000 cubic yards, but due to shrinkage, it actually turns into 2400 cubic yards worth of fill. We still need 600 cubic yards to fill the 3000  cubic yard fill volume. (hence why we have -600). 

Between station 1+00 and 2+00, we have 3600 cubic yards to use, and 2500 cubic yards to fill, so we have 1100 cubic yards extra. 

The Mass ordinate tells us how much fill we have/are missing as we go down the stations. So at first we have -600 fills because we didn't have enough. But it gets balanced by the 1100 extra, leaving us with an extra 500 cubic yards of fill from cuttings. 

---

![[Pasted image 20261001210454.png]]

CY is cubic yard. 

Example:

If the free-haul distance is 1000 ft, the earth excavation cost e is $0.14 per $\text{yd}^3$ and the overhaul cost $o$ is \$0.02 per yd$^3$ per station. Every station is 1+00 ft

The length of economic hauling distance, LEH or EHD  is 
$$
\begin{align}
\text{LEH}=\frac{e}{o}+\text{ free-haul distance} \\
\text{LEH}=\frac{0.14}{0.02}\text{ stations}+1000 \text{ ft} \\
\text{LEH}= 7\text{ stations}\times \frac{100\text{ ft}}{\text{station}}+1000\text{ ft}=1700\text{ ft}
\end{align}
$$

any distance greater than 1700 ft will be borrowed material (from outside the jobsite). Any material less than than the length of economic haul, is considered waste.

![[Pasted image 20261001211400.png]]

---
#### Earthworks Part 2

![[Pasted image 20261008191107.png]]

The part where the fills turn into cuts (the balance point) on the profile diagram is where the crest (or sag) is at the mass diagram. On a mass diagram, a positive slope means we have extra material, a negative slope means that the ground needs to be cut. 

Cost of overhaul is 
$$
\begin{align}
\text{Cost of Overhaul}=h\times o && h=\text{overhaul distance} && o=\text{overhaul cost per unit length}
\end{align}
$$
---

$e$ is the cost of excavation, when $h\times o <e$ , or when the cost of overhaul is less than the cost of excavation, overhauling is worthwhile. 

The economic hauling distance is an equation seen below
$$
\text{Economic Hauling Distance}=\frac{e}{o}+\text{free hauling distance}
$$
anything beyond the economic hauling distance will be considered waste/borrow. 

![[Pasted image 20261008192853.png]]

On this diagram we can calculate how much overhaul we will have graphically. The y-axis is the cubic yards, and the x-axis is the stations 
$$
\text{OH}=(\text{870c.y. - 210c.y.})\times(26.99-8.02-10)=5920\text{c.y.} \times \text{stations}
$$
The reason why we subtract 10 from the second term is because we get 10 stations (1000ft) of free haul distance

---

![[Pasted image 20261008194248.png]]

The steps to solve the OH cost here is to subtract CM2 from CM1 then subtract by the free overhaul distance. In the example, they convert the stations to feet.
$$
1692'-1032'-500'= 160'
$$
Then, they find the amount of cubic yards (point S) at station 11+20 by interpolation. Which is 691cy

They finally calculate the cost
$$
\frac{$11}{\text{Cubic yard-Stations}}\times 691\text{cy}\times (1+60\text{ stations}) =$12162
$$
note that when calculating using station, the station will have a numerical value of 1.60.

