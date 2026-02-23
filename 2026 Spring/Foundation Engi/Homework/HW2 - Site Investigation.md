
---
### <p align="left"><center>Memorandum</center></p>



To: Dr. Amr M. Morsy

From: Andy Nguyen

Date: 2-22-2026

Subject: HW2 Site Investigation

---

The contents of this document contain questions and answers  regarding 'An Introduction to Drilling and Sampling in Geotechnical Practice'. There are are also N-value calculations as seen on question 7, there are tables and graphs ask directed by the question. There are sample calculations for $\phi'$ as well.
![[Signature.excalidraw|200]]
<div style="page-break-after: always;"></div>



1. What are the four main types of drilling according to the video?
	Highway 
	Offroad - access to a site is difficult 
	Over Water - for drills over big bodies of water
	Portable - access by a offroad is impossible, or helicopter cannot be used

2. What is drilling ‘mud’ and what are the three primary functions it serves?
	 Drilling mud is made of water and bentonite, has a density higher than water. 
	 
	 The density helps with the removal of cuttings 
	 Drilling mud disturbs and erodes the soil. 
	 The drilling mud helps support the bore hole walls, so the uncased holes can remain stable in sands under the water table. 

3. What are the four main soil sampling methods according to the video?
	Solid stem continuous flight auger 
	hollow stem Continuous flight auger 
	Mud Rotary
	Coring 

4. Complete the following sentence: The Standard Penetration Test (SPT) blow count (N-value) is
obtained by driving a **Split Spoon** sampler a  total of **18** inches into the soil using a **140** pound hammer dropped from a height of **30** inches. The N-value is representative of the **standard penetration resistance** of the soil, and is obtained by summing up the number of blows over the last **12** inches of driving.

5. Will you most likely obtain conservative or unconservative estimates of consolidation settlement
from disturbed clay samples? Briefly explain your answer. 
	We would obtain unconservative estimates. This is because the disturbed clay samples will usually give higher consolidation settlement estimates than the actual. The disturbance in the clay often causes the consolidation to increase.

6. Will you most likely obtain conservative or unconservative estimates of undrained shear strength
from disturbed clay samples? Briefly explain your answer.
	We will most likely obtain conservative estimates of undrained shear strength from disturbed clay samples because the undrained shear strength estimates will often be much lower than what it is actually. The estimate will be lower because of disturbances to the soil. 

7. Consider a hypothetical soil profile with N values measured during SPT testing tabulated below.
The automatic hammer had a hammer energy correction factor (CE) of 1.3. A standard size
borehole (4.5-in. diameter) was used and the split-spoon sampler did not have space for a liner.
The rod stickup was generally around 5 ft. N values were measured every 2.5 ft over the top 10 ft
of the subsurface, after which N values were measured every 5 ft. down to a depth of 100 ft. The
ground water level (GWL) at the site is very near the surface and the soil has a saturated unit
weight of 130 pcf. Determine the N60 and (N1)60 values for the site. Note that N60 and (N1)60 values
should always be rounded to the nearest whole number. Make these rounding adjustments for N60
values prior to calculating (N1)60 values (ensure that you are actually rounding the N60 and (N1)60
values, not just displaying them with zero decimal places). After your calculations are complete, do
the following:

For $C_{R},$ $L_{R}=5'+\text{testing depth}$ 
For $C_{B}$ , our boring diameter is 4.5 inches, $C_{B}=1$
our $\sigma'=\sigma-u$ or stress from soil subtracted by stress by water.
$$
\gamma'=\gamma_{sat}-\gamma_{w}=130 \frac{\text{lb}}{\text{ft}^3}-62.4\frac{\text{lb}}{\text{ft}^3}=67.6\frac{\text{lb}}{\text{ft}^3}
$$
$$
\sigma'=\gamma'\times z
$$

a)Plot the measured/raw N values, the N60 values and the (N1)60 values as a function of depth on
the same figure. Explain what you observe from this plot.

![[Pasted image 20260222163630.png]]
The N60 values are greater than the regular N values, this is most likely due to the Cs values being consistently 1.3, as well as the Ce values. 

The N1(60) values start off with a large difference compared to the N(60) values, but slowly dip below N60 values, and then goes along the original N values. This is probably because the CN values start off larger than 1, but then gradually decreases below 1 as it increases in depth. 

b) Create a table that looks exactly like the one below and highlight the raw N values, N60 values
and (N1)60 values at depths 2.5 ft, 15 ft, 60 ft, and 100 ft.

sample calculations for N(60)
$$
N_{60}=\text{N}\cdot C_{E}\cdot C_{R} \cdot C_{B}\cdot C_{s}=17\cdot 1.3 \cdot 0.95 \cdot 1 \cdot 1.3 = 27 \text{ (after rounding)}
$$
$$
(N_{1})_{60}=N_{60}\cdot C_{N}=27\cdot 1.6=43
$$
![[Pasted image 20260222164426.png]]

c) Estimate the angle of internal resistance of the soil using the correlations by Hatanaka and
Uchida (1996) and Schmertmann (1975)
sample calculations and table 
$$
\phi'96=\sqrt{15.4\cdot43}+20=45.733^\circ
$$
$$
\begin{align}
\phi'75=\tan^{-1}\left(\frac{27}{12.2+20.3\left(\frac{169}{2116}\right)}\right)^{0.34}=1.032\text{ rad}=59.14^\circ
\end{align}
$$
![[Pasted image 20260222170316.png]]