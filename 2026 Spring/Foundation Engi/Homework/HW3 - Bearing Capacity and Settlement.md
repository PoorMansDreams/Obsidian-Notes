

---
### <p align="left"><center>Memorandum</center></p>



To: Dr. Amr M. Morsy

From: Andy Nguyen

Date: 3-25-2026

Subject: HW3 Bearing Capacity and Settlement

---

Below are calculations for the Bearing Capacity and Settlement of several different scenarios. To calculate for B for some of the equations, excel was used to make the iteration process easier. All examples are solved with work shown. 
![[Signature.excalidraw|200]]
<div style="page-break-after: always;"></div>






1. 
A footing of area 6 ft x 6 ft is constructed at a depth 6 ft from the ground surface in a silty clay
soil with c' = 820 psf, $\phi$' = 20º, and $\gamma$ = 118.5 pcf. Calculate the ultimate bearing capacity (gross
and net) of the foundation in the following cases:

i) Groundwater table is at the ground surface
ii) Groundwater table is at 3 ft from ground surface
iii) Groundwater table is at the foundation level
iv) Groundwater table is at 9 ft from ground surface
v) Groundwater table is at 15 ft from ground surface

Use equation
$$\begin{aligned}
q_{ult,gross} &= c'N_c s_c d_c + \sigma'_D N_q s_q d_q + \frac{1}{2} \gamma_b B N_\gamma s_\gamma d_\gamma \\
q_{ult,net} &= q_{ult,gross} - \sigma'_D
\end{aligned}$$
$$

\begin{align} 
\textbf{Bearing Capacity Factor}
 \\
N_c = \begin{cases} 
\frac{N_q - 1}{\tan \phi'} & \text{for } \phi' > 0 \\ 
5.14 & \text{for } \phi' = 0 
\end{cases}
 \\

% N_q Factor
N_q = e^{\pi \tan \phi'} \tan^2 \left( 45 + \frac{\phi'}{2} \right)
 \\

% N_gamma Factor
N_\gamma = 2(N_q + 1) \tan \phi'
\end{align}

$$
$$
\begin{align} \\
\textbf{Shape Factor} \\

% Shape factor for Cohesion
s_c = 1 + \left( \frac{B}{L} \right) \left( \frac{N_q}{N_c} \right)
 \\

% Shape factor for Surcharge
s_q = 1 + \left( \frac{B}{L} \right) \tan \phi'
 \\

% Shape factor for Unit Weight
s_\gamma = 1 - 0.4 \left( \frac{B}{L} \right)
\end{align}
$$
$$
\begin{align} 
\textbf{Depth Factors} \\

% Depth factor for Cohesion
d_c = 1 + 0.4k
 \\

% Depth factor for Surcharge
d_q = 1 + 2k \tan \phi' (1 - \sin \phi')^2
 \\

% Depth factor for Unit Weight
d_\gamma = 1
 \\

% The k-factor definition
k = \begin{cases} 
\frac{D}{B} & \text{for } \frac{D}{B} \leq 1 \\ 
\tan^{-1} \left( \frac{D}{B} \right) & \text{for } \frac{D}{B} > 1 
\end{cases}
\end{align}

$$
knowing our variables $B=6' \hspace{10pt}L=6' \hspace{10pt}D=6' \hspace{10pt}K=\frac{D}{B}=1$
and for our stress $\sigma'_{D}=6\cdot(118.5-62.4)=336.6 \frac{\text{lb}}{\text{ft}^2}$
for the effective unit weight $\gamma_{b}=118.5-62.4=56.1 \frac{\text{lb}}{\text{ft}^3}$
our cohesion is $c'=820 \frac{\text{lb}}{\text{ft}^2}$
(this is for when the GWT is at the ground surface)

after calculating;
$$
\begin{align}
N_{c}=14.8   &  & s_{c}=1.43 &  & d_{c}=1.4\\
N_{q}=6.4  &  & s_{q}=1.36 &  & d_{q}=1.315\\
N_{\gamma}=5.38 &  & s_{\gamma}=0.6 &  & d_{\gamma}=1
\end{align}
$$

i) GWT at ground surface

Plug into our equation for $q_{ult,gross}$
$$
q_{ult,gross}= 820(14.8)(1.43)(1.4)+336.6(6.4)(1.36)(1.315)+\frac{1}{2}(56.1)(6)(5.38)(0.6)(1)=28700 \frac{\text{lb}}{\text{ft}^2}
$$
$$
q_{ult,net} = 28700 \frac{\text{lb}}{\text{ft}^2} - 336.6 \frac{\text{lb}}{\text{ft}^2}=28363\frac{\text{lb}}{\text{ft}^2}
$$

ii) GWT 3 feet below ground level

only difference here is that our $\sigma'_{D}=3(118.5)+3(118.5-62.4)=523.8\frac{\text{lb}}{\text{ft}^2}$

$$
q_{ult,gross}= 820(14.8)(1.43)(1.4)+523.8(6.4)(1.36)(1.315)+\frac{1}{2}(56.1)(6)(5.38)(0.6)(1)=30834.8 \frac{\text{lb}}{\text{ft}^2}
$$

$$
q_{ult,net} = 30834.8 \frac{\text{lb}}{\text{ft}^2} - 523.8 \frac{\text{lb}}{\text{ft}^2}=30311.03\frac{\text{lb}}{\text{ft}^2}
$$

iii) GWT is 6 feet from the ground, which means the water level is right at the bottom of the footing

our overburden pressure is now $\sigma'_{D}=6(118.5)=711 \frac{\text{lb}}{\text{ft}}$

$$
q_{ult,gross}= 820(14.8)(1.43)(1.4)+711(6.4)(1.36)(1.315)+\frac{1}{2}(56.1)(6)(5.38)(0.6)(1)=32977.5 \frac{\text{lb}}{\text{ft}^2}
$$
$$
q_{ult,net} = 32977.5 \frac{\text{lb}}{\text{ft}^2} - 711 \frac{\text{lb}}{\text{ft}^2}=32266.4\frac{\text{lb}}{\text{ft}^2}
$$
iv) GWT is 9ft below the ground surface
$\sigma'_{D}=711 \frac{\text{lb}}{\text{ft}}$
Our water depth, $D_{w}=9'$
we have to use a different $\gamma_{b}$
$$
\gamma_b = \gamma - \gamma_w \left( 1 - \frac{D_w - D}{B} \right)
$$
$$
\gamma_{b}=118.5-62.4\left( 1-\frac{9-6}{6} \right)=87.3
$$

$$
q_{ult,gross}= 820(14.8)(1.43)(1.4)+711(6.4)(1.36)(1.315)+\frac{1}{2}(87.3)(6)(5.38)(0.6)(1)=33279.62 \frac{\text{lb}}{\text{ft}^2}
$$

$$
q_{ult,net} = 33279.62 \frac{\text{lb}}{\text{ft}^2} - 711 \frac{\text{lb}}{\text{ft}^2}=32568.62\frac{\text{lb}}{\text{ft}^2}
$$
$$

$$

v) GWT is 15ft below the ground surface, 
at this point, the $D_{w}>D+B \hspace{10pt}15>6+6$ 
which means $\gamma_{b}=\gamma=118.5$

$$
q_{ult,gross}= 820(14.8)(1.43)(1.4)+711(6.4)(1.36)(1.315)+\frac{1}{2}(118.5)(6)(5.38)(0.6)(1)=33581.76 \frac{\text{lb}}{\text{ft}^2}
$$
$$
q_{ult,net} = 33581.76 \frac{\text{lb}}{\text{ft}^2} - 711 \frac{\text{lb}}{\text{ft}^2}=32870.76\frac{\text{lb}}{\text{ft}^2}
$$
---

2. 
A column carries 330 kips is supported by a square footing resting on dry sand with $\phi$' = 35º
and $\gamma$ = 112 pcf. Apply a factor of safety of 2.5 to the net ultimate bearing capacity. Find the
size of the footing in the following cases:

i) If the footing rests at the ground surface.

$D=0 \hspace{10pt}c'=0$ 
so we really only need to calculate the $\gamma$ portion of our variables
$\gamma_{b}=\gamma=112\text{ lb/ft}^3$
use equation

$$
F.S.=\frac{\text{Provided}}{\text{Applied}}=\frac{\text{Provided}}{\frac{330000\text{ lb}}{\text{B}^2}}
$$
the applied pressure is the footing on the ground in $\frac{\text{lb}}{\text{ft}^2}$
we are given the factor of safety, so we can rearrange

$$
\frac{330000\text{ lb}}{B^2}=\frac{\text{Provided}}{F.S}
$$

our provided can be found by calculating $q_{gross}$, since our $\sigma'_{D}$ (overburden stress) is zero, $q_{gross}=q_{net}$

$$
\begin{align}
N_{c}=   &  & s_{c}= &  & d_{c}=\\
N_{q}=33.3  &  & s_{q}= &  & d_{q}=\\
N_{\gamma}=48.028 &  & s_{\gamma}=0.6 &  & d_{\gamma}=1
\end{align}
$$
$$
q_{ult,gross} = \cancel{ c'N_c s_c d_c + \sigma'_D N_q s_q d_q} + \frac{1}{2} \gamma_b B N_\gamma s_\gamma d_\gamma
$$

$$
q_{ult,gross}=q_{net}=\frac{1}{2}(112)(B)(48.028)(0.6)(1)=1613.74B \frac{\text{lb}}{\text{ft}}=\text{Provided}
$$

$$
\frac{330000\text{ lb}}{B^2}=\frac{1613.74B \frac{\text{lb}}{\text{ft}}}{2.5}
$$
after calculating, $B=L=8\text{ feet}$

ii) If the footing rests at a depth of 5 ft from the ground surface.

Since the footing now rests 5 feet below the ground surface we have to account for overburden pressure. 

$$
q_{ult,gross} = \cancel{ c'N_c s_c d_c} + \sigma'_D N_q s_q d_q + \frac{1}{2} \gamma_b B N_\gamma s_\gamma d_\gamma
$$

$\sigma'_{D}=5(112)=560\text{ lb/ft}^2$
now we have to calculate our new factors, 

$$
\begin{align}
N_{c}=   &  & s_{c}= &  & d_{c}=\\
N_{q}=33.3  &  & s_{q}=1.7 &  & d_{q}=1+\frac{1.273}{B}\\
N_{\gamma}=48.028 &  & s_{\gamma}=0.6 &  & d_{\gamma}=1
\end{align}
$$

$$
q_{ult,gross}=560(33.3)(1.7)\left( 1+\frac{1.273}{B} \right)+\frac{1}{2}(112)(B)(48.028)(0.6)(1)=\text{Provided}
$$
however, we need to remember that this is INSIDE the soil now, so we need to use $q_{ult,net}$

$$
q_{ult,net}=560(33.3)(1.7)\left( 1+\frac{1.273}{B} \right)+\frac{1}{2}(112)(B)(48.028)(0.6)(1)-560
$$
put it into this awful equation
$$
\frac{330000\text{ lb}}{B^2}=\frac{560(33.3)(1.7)\left( 1+\frac{1.273}{B} \right)+\frac{1}{2}(112)(B)(48.028)(0.6)(1)-560}{2.5}
$$

$$
2.5\cdot 330000\text{ lb}=B^2(560(33.3)(1.7)\left( 1+\frac{1.273}{B} \right)+\frac{1}{2}(112)(B)(48.028)(0.6)(1)-560)
$$

After several iterations in excel... (guessing B)

$B=4.165'$  


---

3.  ![[Pasted image 20260325195335.png]]
use equations 
$$
S=\delta=m_{v}\cdot \Delta \sigma \cdot H
$$
There are two layers, so we have to separate it into $S_{1}$ and $S_{2}$

Using 2:1 method, we can calculate the $\Delta \sigma$
adapting from the original equation, of 

$$
\Delta \sigma=q_{applied, net}\cdot \frac{B\times L}{(B+z)(L+z)}
$$

![[Pasted image 20260325220736.png]]

---
4. A raft 45 ft x 45 ft is designed to support a residential building with a basement. The foundation
level is 15 ft below the ground surface. The supporting soil is deep clay of $\gamma$ = 110 pcf, su = 0.9
ksf. The groundwater table is 1.0 ft below the ground surface. Estimate the allowable bearing
capacity. Apply a factor of safety of 2.0 to the net ultimate bearing capacity

![[Pasted image 20260325224526.png]]

---

5. 
![[Pasted image 20260325225006.png]] 

geostatic effective vertical stresses?

$$
\sigma'=10(100)+12(106-62.4)+3(112-62.4)=1672 \frac{\text{lb}}{\text{ft}^2}
$$

---

Induced effective stress at points a and b from the building?

solve for eff. vertical stress at a.

$q_{net}=q-q_{removed}$
$q_{net}=2000-5\times 100=1500 \frac{\text{lb}}{\text{ft}^2}$


at the center, $m_{1}=m_{2}=m_{3}=m_{4}$ and $n_{1}=n_{2}=n_{3}=n_{4}$

$$
m=\frac{B_{1}}{z}=\frac{50}{20}=2.5 \hspace{10pt} n=\frac{L_{1}}{z}=\frac{60}{20}=3
$$

using the influence value table, $I_{z}=0.245$
knowing this, 

$$
\Delta \sigma_{a}=q\cdot \sum I_{z}=q\times(I_{z_{1}}+I_{z_{2}}+I_{z_{3}}+I_{z_{4}})
$$

all the $I_{z}$ are the same since this is at the center, so

$$
\Delta \sigma_{a}=1500\cdot 4\cdot 0.245=1470 \frac{\text{lb}}{\text{ft}^2}
$$

---

solving for eff. vertical stress at b?

$$
m=\frac{100}{20}=5 \hspace{10pt} n=\frac{120}{20}=6
$$

using table, $I_{z}=0.247$

$$
\Delta \sigma_{b}=0.247\cdot 1500 = 373\frac{\text{lb}}{\text{ft}^2}
$$

---

Using 2:1 method

$$
\Delta \sigma_{z}=q\times \frac{BL}{(B+z)(L+z)}=\frac{100\cdot 120}{(100+20)(120+20)}=1071.43 \frac{\text{lb}}{\text{ft}^2}
$$

according to 2:1 method, it assumes that any area under the projected is $\Delta_{\sigma_{z}}$
$$
\Delta \sigma_{a}=\Delta \sigma_{b}=1071.43 \frac{\text{lb}}{\text{ft}^2}
$$






