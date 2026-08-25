Sedimentation is a phase in water treatment, water comes into a tank from the side. It goes into the inlet zone, settling zone, and then outlet zone which is the exit. As the water flows through this giant tank, sludge settles at the bottom. At the bottom, the sludge can be extracted. Scum may also start developing at the top. This is just oil, soap, and particles lighter than water. Scum can be easily skimmed 
![[Pasted image 20251208141233.png]]

Types of settling
* Type I: Discrete settling
	* Particles don't interact with each other and just sink
* Type II: Flocculent settling
	* Particles 'flocc' and interact with each other, sticking together, sinking faster.
* Type III: Hindered / Zone settling
	* Particles form a blanket of particles, settling velocity gets slowed.
* Type IV: Compression Settling 
	* Particles compress as settling happens
![[Pasted image 20251208141413.png]]

---
**Settling Velocity** - How fast particles settle
Settling velocity of a spherical particle:
$$
\begin{align}
\rho_{w}&=\text{density water} \\
\rho_{p}&=\text{density particle}\\
\upsilon_{s}&=\text{particle settling velocity} \\
d_{p}&=\text{particle diameter} \\
\mu&=\text{absolute viscosity of water}
\end{align}
$$
$$
R_{e}=\frac{\rho_{w}\upsilon_{s}d_{p}}{\mu}
$$
When a particle is suspended in water, there are three forces that act upon it. $F_{B}$ buoyancy force and $F_{D}$ drag force. Gravitational force, $F_{G}$ which goes down

The particle settling velocity is shown here 
$$
\upsilon_{s}=\frac{g(\rho_{p}-\rho_{w})d_{p}^2}{18\mu}
$$
$V_{o}$ is the critical settling velocity, a rule is that our settling velocity $V_{s}=\upsilon_{s}$ should be greater than or equal to our critical settling velocity **for it to be removed.** 
$$
V_{o}=\frac{h}{\theta}=\frac{Q}{A_{b}}
$$

If we want a ideal 100% particle removal, the area of the settling basin can be described as
$$
A_{b}=\frac{18Q\mu}{g(\rho_{p}-\rho_{w})d_{p}^2}
$$
if the % of particle removed is not 100%, we can just do 
$$
\frac{V_{s}}{V_{o}}\times 100=\%
$$

---
##### Example 1
A drinking water treatment plant uses a circular sedimentation basin to treat 3.0 MGD of river  water. (1.0 MGD = 0.0438 m 3/s). After storms occur upstream, the river often carries 0.010 mm  (=10 -5 m) silt particles with an average density of 2.2 g/cm 3, and the silt must be removed before the water can be used. The plant’s clarifier is 3.5 m deep and 21 m in diameter. The water is 15 ◦C.

Thus, water density (ρ) is 999.1 kg/m3 and dynamic viscosity (μ) is 0.00114 kg/m/s.

a. What is the hydraulic detention time of the clarifier 
$$
\text{Hydraulic detention time}=\frac{V}{Q}=\frac{\frac{\pi}{4}(21^2)(3.5)}{3\text{MGD}\times \frac{0.0438\text{ m}^3/s}{\text{MGD}}}=2.6 \text{ hrs}=9226\text{ sec}
$$
b. Will the Clarifier remove **all** of the silt particles?
$$
V_{s}=\frac{(9.81)(2200-999.1)(0.00001)^2}{18\times 0.00114}=5.7\times 10^{-5}
$$
$$
V_{o}=\frac{h}{\theta}=\frac{3.5}{9226}=38\times 10^{-5}
$$
Our condition for **all** silt particles to be or removed 
$$
V_{s} \geq V_{o} 
$$
The condition is not fulfilled, there will be leftover silt particles 

for exam: Oxygen demand, stream pollution, water treatment processes (coagulation flocculation sedimentation)