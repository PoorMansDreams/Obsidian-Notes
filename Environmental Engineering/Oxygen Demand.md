#environmental 
BOD, COD, ThOD,
##### BOD Introduction
Dissolved Oxygen, Oxygen concentration in water is contributed from
1. Photosynthesis of plants
2. Oxygen in the air dissolved in the water
DO (Dissolved Oxygen) concentration in water is effected by
* Pressure
* Temperature (higher=worse)
* The size of the body of water (Bigger = more Oxygen dissolved)

Why do we need to know DO?
1. Indicating quality of water
2. Used as an operating indicator in biological wastewater treatment system  
3. Used to analyze biochemical oxygen demand (BOD)  
4. Controlling corrosion of iron pipes
	SAG curve
![[Pasted image 20251020142538.png]]

- **BOD** is the measure of the amount of oxygen required by aerobic microorganisms to oxidize organic wastes $\left(\frac{mg-O_{2}}{L} \right)$ 
$$
\text{Organic Matter}+O_{2}\to^\text{Aerobic}_{\text{microorganisms}}\to CO_{2}+H_{2}O+\text{New Cells}+\text{By-products}
$$
some of the by-products are $NO^-_{3},PO_{4}^{-2},SO_{4}^{-2}$
Methane, $CH_{4}$ : swamp gas, greenhouse gas. 


---

Five Day Standardized BOD test

The way it works is that we measure the total amount of oxygen consumed in the first 5 days.
![[Pasted image 20251020143804.png]]

We sometimes have to add seeded diluted water into the wastewater because there might be too much pollutants in it. 

$$
\text{BOD}_{\text{w}}=\frac{(\text{DO}_{i}-\text{DO}_{f})-(\text{B}_{i}-\text{B}_{f})(1-\text{P})}{\text{P}}
$$
where
$\text{B}_{i}=\text{Initial DO of the Blank}$
$\text{B}_{f}=\text{Final DO of the Blank}$
$\text{P}=\frac{V_{w}}{V_{m}}$

##### Example 1
A 10 mL sample of sewage mixed with enough water to fill a 300 mL bottle has an initial DO of 9.0 mg/L. It is desirable to have at lease 2.0 mg/L drop in DO during the five-day run, and the final DO should be at least a 2.0 mg/L. For what range of BOD$_{5}$ would this dilution produce the desired results?
$$
\text{BOD}_{\text{w}}=\frac{(\text{DO}_{i}-\text{DO}_{f})-(\text{B}_{i}-\text{B}_{f})(1-\text{P})}{\text{P}}
$$Since there is no "Blank" sample we can just remove the B portion.
$$
\text{BOD}_{\text{w}}=\frac{(\text{DO}_{i}-\text{DO}_{f})}{\text{P}}
$$
To get at least 2.0 mg/L drop in DO, the minimum BOD would need to be 
$$
\text{BOD}_{5}\geq \frac{2\frac{\text{ mg}}{L}}{\frac{10}{300}}=60 \frac{\text{ mg}}{L}
$$
To assure at least 2.0 mg/L of DO remains after 5 days, it requires that
$$
\text{BOD}_{5}\leq \frac{(9-2)\frac{\text{ mg}}{L}}{\frac{10}{300}}=210 \frac{\text{ mg}}{L}
$$
So then we'd need 60-210 mg/L of BOD to get a 2.0 mg/L drop in DO

##### Example 2
A test bottle containing just seeded dilution water has its DO level drop by 1.0 mg/L in a five-day test. A 300 mL BOD bottle filled with 15 mL of wastewater and the rest seeded dilution water experiences a drop of 7.2 mg/L in the same time period. What would be the five-day BOD of the waste?
$$
\text{BOD}_{\text{w}}=\frac{(\text{DO}_{i}-\text{DO}_{f})-(\text{B}_{i}-\text{B}_{f})(1-\text{P})}{\text{P}}
$$
we can plug in numbers
$$
\text{BOD}_{\text{w}}=\frac{7.2-1\left(1- \frac{15}{300} \right)}{\frac{15}{300}}=125 \frac{\text{ mg}}{L}
$$

---
##### BOD

This is the rates of decomposition of BOD and the proportion rate of how much organic matter is left remaining. They bolt reach a certain Ultimate BOD
![[Pasted image 20251020145632.png]]

Oxygen demand can be shown as 
$$
L_{t}=L_{o}e^{-klt}
$$
where
$k=$ BOD reaction rate constant
$L_{o}=$ Total amount of BOD or the ultimate CBOD
$L_{t}=$ amount of BOD left after time, t

##### Example 3
The dilution factor, P for an unseeded mixture of waste and water is 0.03. The DO of the mixture is initially 9.0 mg/L, and after five days, it has dropped to 3.0 mg/L. The reaction rate constant k has been found to be 0.22 day$^{-1}$.  

a. What is the five-day BOD of the waste?  
$$
BOD_{5}=\frac{9-3}{0.03}=200 \frac{\text{mg}}{\text{L}}
$$

b. What would be the ultimate carbonaceous BOD ($L_{o})$ ?  
$$
BOD_{t}=L_{o}(1-e^{-kt})
$$
$$
L_{o}=\frac{BOD_{5}}{(1-e^{-kt})}=\frac{200}{(1-e^{-0.22\times 5})}=300 \frac{\text{mg}}{\text{L}}
$$
c. What would be the remaining oxygen demand after five days?
After 5 days, the 200 mg/L of oxygen demand out of the 300 mg/L would have already been used. So the remaining oxygen demand would be 300-200 = **100 mg/L**

##### BOD Cont.
The BOD rate constant $(k)$ depends upon the 
* nature of the waste
* type of microorganisms present
* temperature
The temperature relation can be shown as 
$$
k_{T}=k_{20}\theta^{(T-20)}
$$
Where $k_{T}$ is the rate constant at $T^\circ C$ 
and $k_{20}$ is the rate constant at 20$^\circ$C
and $\theta$ = 1.047

##### Example 4
In example 3, the waste had an ultimate BOD equal to 300 mg/L. At 20 ◦C, the five-day BOD was 200 mg/L, and the reaction rate constant was 0.22 day-1. What would be the five-day BOD of this waste be at 25◦C?  
$$
k_{25}=0.22\times(1.047)^{(25-20)}=0.277\text{ days}^{-1}
$$
if we plug this back into example 3, 
$$
L_{o}=\frac{BOD_{5}}{(1-e^{-kt})}=\frac{200}{(1-e^{-0.277\times 5})}=266 \frac{\text{mg}}{\text{L}}
$$
##### NBOD (Nitrification)
$$
\text{NH}_{3}+2\text{O}_{2} \longrightarrow \text{NO}_{3}^- +\text{H}^++\text{H}_{2}\text{O}
$$
![[Pasted image 20251020152139.png]]

##### Example 5
