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

We sometimes have to add seeded diluted water into the wastewater because there might be too much pollutants in it. Full of Water and some seed

$$
\text{BOD}_{\text{w}}=\frac{(\text{DO}_{i}-\text{DO}_{f})-(\text{B}_{i}-\text{B}_{f})(1-\text{P})}{\text{P}}
$$
where
$\text{B}_{i}=\text{Initial DO of the Blank}$
$\text{B}_{f}=\text{Final DO of the Blank}$
$\text{P}=\frac{V_{w}}{V_{m}}$ = Volume Waste Water/Volume of the Mixture



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
L_{t}=L_{o}e^{-kt}
$$
$$
\text{BOD}_{t}=L_{o}(1-e^{-kt})
$$
$$
\text{BOD}_{t}+L_{t}=L_{o}
$$


where

BODt is the ultimate CBOD
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
Some domestic wastewater has 30 mg/L of nitrogen in the form of either organic nitrogen or ammonia. Assuming that very few new cells of bacteria are formed during the nitrification of the waste (that is, the oxygen demand can be found from a simple stoichiometry analysis of the nitrification reactions), find  

a. The ultimate nitrogenous oxygen demand 
simply convert 30 mg/L of nitrogen to mg/L of oxygen using stoich
$$
NBOD=30 \times \frac{17}{14}\times \frac{64}{17} = 137 \frac{\text{mg }\text{O}_{2}}{L}
$$
b. The ratio of the ultimate NBOD to the concentration of nitrogen in the waste.
$$
\frac{\text{ultimate NBOD}}{\text{concentration of N}}=\frac{137}{30}=4.57 \frac{\text{mg}\text{ O}_{2}}{\text{mg N}}
$$

Ultimate NBOD = $4.57\times \text{TKN}$ (Total Kjeldahl Nitrogen)
TKN = total concentration of (organic nitrogen + ammonia nitrogen) in wastewater
so if we have something like 15-50 mg/L of TKN 
then Ultimate NBOD would be 68.55-228.5

##### Other Oxygen Demand Measurements

- Theoretical Oxygen Demand (ThOD)  
	- The amount of oxygen required for the complete oxidation of organic waste (theoretical calculation)  
- Chemical Oxygen Demand (COD)  
	- Measures oxygen required for compounds which are not biologically degradable, e.g., industrial chemicals (phenols, benzene, pesticide..)  
	-  Strong oxidizing chemicals are used to oxidize the organics

$$
\text{C}_6\text{H}_{12}\text{O}_6 + 6\text{O}_2 \longrightarrow 6\text{CO}_2 + 6\text{H}_2\text{O}
$$
in this case, the 6 oxygen is the theoretical need.

ThOD > BOD,
Ultimate BOD > BOD$_{5}$
ThOD > COD > BOD
$$
\text{C}_6\text{H}_{12}\text{O}_6 + 6\text{O}_2 \xrightarrow{\text{microorganisms}} 6\text{CO}_2 + 6\text{H}_2\text{O} + \text{cells}

$$
##### Example 6

Wastewater from a fruit-canning factory contains 150mg/L of fructose, what is the ThOD of this wastewater mg/L?

$$
C_{6}H_{12}O_{6}+6O_{2}\to_{6}CO_{2}+6H_{2}O
$$
$$
150 \frac{mg\text{ fructose}}{L}\times \frac{192g \text{ O}_{2}}{180g \text{ fructose}}=160mg\text{ O}_{2} 
$$
---

If a $1.67\times 10^{-3}$ M glucose solution that is completely oxidized to CO2 and H2O, find amount of oxygen mg/L required to complete the reaction
$$
C_{6}H_{12}O_{6}+6O_{2}\to_{6}CO_{2}+6H_{2}O
$$
$$
1.67\times 10^{-3} \frac{mol}{L}\times \frac{180g}{mol}\times 10^3
\frac{mg}{g}=\frac{301mg}{L}\text{ glucose}$$
$$
301 \frac{mg}{L}\text{ glucose}\times \frac{192g\text{ O}_{2}}{180g \text{ glucose}}=321g\text{ O2}
$$
##### Example 7 (1)

A sewage is containing 150 mg/L of CH2(NH2)COOH and 40 mg/L of NH3.  
Find the amount of oxygen (mg/L) required for oxidation of both carbon and nitrogen compounds.

$$
\begin{align*}
\text{CH}_2(\text{NH}_2)\text{COOH} + 1.5\text{O}_2 &\longrightarrow 2\text{CO}_2 + \text{H}_2\text{O} + \text{NH}_3 \\
\text{NH}_3 + 2\text{O}_2 &\longrightarrow \text{NO}_3^- + \text{H}_2\text{O} + \text{H}^+
\end{align*}
$$
Molar mass of the sewage is 75g/mol = 75mg/mmol
$$
\frac{150\frac{mg}{L}}{75 \frac{mg}{mmol}}=2 \frac{mmol}{L} \text{ sewage}
$$
for every 1 mmol/L of the CH2(NH2)COOH, there is 1.5 mmol/L of O2, so
$$
2 \frac{mmol}{L}\times 1.5=3 \frac{mmol}{L} \text{ O}_{2}
$$
---
MW of NH$_3$ is 17g/mol = 17mg/mmol
$$
\frac{40\frac{mg}{L}}{17 \frac{mg}{mmol}}=2.35 \frac{mmol}{L}\text{NH}_{3}
$$
from our first equation, 2 mmol/L of NH$_3$ is produced from the 150mg/L of sewage (CH2(NH2)COOH)
so total moles of NH$_3$ is 2.35+2= 4.35 mmol/L

There is 2 oxygen needed per 1 NH$_3$ so
$$
4.35 \frac{mmol}{L}\times 2\text{ O}_{2}=8.7 \frac{mmol}{L} \text {O}_{2}
$$
We cant forget about the O2 from the sewage, 
$$
3 \frac{mmol}{L}+8.7 \frac{mmol}{L} =11.7 \frac{mmol}{L} \text{ O}_{2}
$$
