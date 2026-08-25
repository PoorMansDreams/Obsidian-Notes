**For deflections, do not use $\omega_{u}$** use unfactored loads. 
for a simply support beam, $\omega=\omega_{d}+\omega_{L}$
and the deflection is 
$$\Delta=\frac{5\omega L^4}{384EI}$$
The delta calculation for a reinforced beam is more complex, we cannot use the given deflection for a simply supported beam. When you have a frame, middle will have positive moment, and the ends will have a negative moment. 

remember, $E=E_{c}$ where $E_{c}$ is the concrete. 

We have to do **integral method** to find the deflection of a frame. Thankfully we will be given the equation for the beam. 

When a material is under sustained compression, there is "creep", this causes shrinking, and deflection can increase. 

Final Deflection = Immediate (Short term) Deflection + Time Dependent (Long Term) Deflection

---
## Immediate Deflection

![[Pasted image 20260303171602.png]]
Finding the moment of cracking for both negative and positive moment.
$F_{r}$ is the maximum tension concrete can take before it rips apart.
**Note** always use $\lambda=1$, 
$f'c$ is in psi for the $F_{r}$ equation

$$
M_{cr}=\frac{F_{r}I_{g}}{y_{t}}
$$
The $M_{cr}$ is the moment of cracking, the moment it will be at when the concrete cracks. 
$y_{t}$ is findable by using $\bar{y}$ or the Neutral axis. 

For the middle of the beam, positive moment,
for the supports, negative moment. 
NEGLET THE FLANGE THAT IS IN TENSION.

![[Pasted image 20260303171624.png]]

This is the equation for $\bar{y}$ it is
$$
\bar{y}=\frac{\frac{1}{2}bt_{f}^2+b_{w}(h-t_{f})\left( t_{f}+\frac{h-t_{f}}{2} \right)}{bt_{f}+b_{w}(h-t_{f})}
$$
$$
y_{t}=h-\bar{y}
$$
$$
I_{g}=\sum I_{o}+\sum Ad^2 
$$
for a I beam, the equation is exactly the [[Concrete Structure Lec 8]].
![[Pasted image 20260303173236.png]]
If the beams is different, we need to use different $t_{f}$

for a simply support beam, we will need to find all 3 different $M_{cr}$ . But they all use the same equation because the beam is the same

**NOTE** this is for an UNCRACKED beam.

---

### Quiz 21

Find $y_{t}$ and $I_{g}$ for a given beam if moment is positive
![[Drawing 2026-03-03 17.36.31.excalidraw]]

simply use the given equation we have, but make sure to ignore that BOTTOM FLANGE since it is in POSITVE MOMENT. 
h=5+11+4=20
$$
\bar{y}=\frac{\frac{1}{2}\cdot30(5^2)+10(20-5)\left( 5+\frac{20-5}{2} \right)}{30(5)+10(20-5)}=7.5\text{ in}
$$
$$
I_{g}^+= \frac{30(5^{3})}{12}+\frac{10(20-5)^{3}}{12}+30(5)\left(7.5-\frac{5}{2}\right)^{2}+10(20-5)\left(\frac{20-5}{2}+5-7.5\right)^{2}
$$
$$
I_{g}^+=10625\text{ in}^4
$$

### Quiz 22
for the same beam, find $I_{g}^-$ , (the moment must be negative)

we use the same equation, however we need to use a different b and $t_{f}$
$$
\bar{y}=\frac{\frac{1}{2}\cdot20(4^{2})+10(20-4)\left(4+\frac{20-4}{2}\right)}{20(4)+10(20-4)}=8.66\text{ in}
$$
$$
I_{g}^-=\frac{20(4^{3})}{12}+\frac{10(20-4)^{3}}{12}+20(4)\left(8.66-\frac{4}{2}\right)^{2}+10(20-4)\left(\frac{20-4}{2}+4-8.66\right)^2
$$
$$
I_{g}^-
=8853\text{ in} ^4$$

![[Pasted image 20260303180033.png]]

To find the neutral axis and moment of inertial for $I_{cr}$
for compress, $(n-1)A's$ these are conversions to turn 
for tensions, $nAs$ 
**Note** This is for a CRACKED beam. 

![[Pasted image 20260303180348.png]]
this is the equation to find calculate the CRACKED section. 
when we solve for $\bar{y}$ we will get two answers, one positive and one negative. **Positive** will be the correct answer. 

We will first assume that $\bar{y}$ is equal to $t_{f}$ if this is not true, 
move onto $\bar{y}>t_{f}$ 

In short, we first try to use the first equation assuming that $\bar{y}$ is less than or equal to $t_{f}$

If our solved $\bar{y}$ is more than $t_{f}$ , then we have to move onto the 2nd equation. 

$I_o$ for the rebar will be considered zero. 
![[Pasted image 20260303181047.png]]
This is the for the negative moment, exactly the same. 
![[Pasted image 20260303181151.png]]

$I_{e}$ is the effective moment of inertia, it could be $I_{g}^-$
$M_{a}$ is the moment that is acting upon the beam, or it could be $M_{1}$
$I_{g}$ is calculated previously, could be $I_{g}^-$
$M_{cr}$ is the moment where the beam cracks, which could be $M_{cr_{1}}$
$I_{cr}$ is the moment of inertia when it cracks, could be $I_{cr}^-$

note that the calculated value should be smaller than the $I_{g}$ 

Each $I_{e}$ equation is different depending on the case of the beam.

for 3 moments, (1 positive, 2 negative, use the equation in the image above)

for 2 moments
$$
I_{e}=0.75I_{e}^++0.25I_{e_{2}}^-
$$
for a simply supported beam, which is only 1 moment.
$$
I_{e}=I_{e}^+
$$
![[Pasted image 20260303183458.png]] ^c12c2d

---
## Long Term Deflection

we will be given
$$
\begin{align}
\Delta_{D+L}=\frac{70L^4}{EI_{e}}=2\text{ in}
\end{align}
$$
however, we will have to split it into two different deflections, one for live and one for dead load.

we simply use the equation
$$
\begin{align}
\Delta_{D}=\frac{\Delta_{D+L}\times \omega_{D}}{\omega_{D}+\omega_{L}} \\
\Delta_{L}=\frac{\Delta_{D+L}\times \omega_{L}}{\omega_{D}+\omega_{L}}
\end{align}
$$
Let's say we are given $\omega_{D}=2 \frac{\text{K}}{\text{ft}}$ and $\omega_{L}=3 \frac{\text{K}}{\text{ft}}$
$$
\begin{align}
\Delta_{D}=\frac{2\times 2}{2+3}=0.8 \\
\Delta_{L}= \frac{2\times 3}{2+3}=1.2
\end{align}
$$
For our Short term, 
$$
\Delta_{L}=1.2\times 0.3
$$
![[Pasted image 20260310170607.png]]
![[Pasted image 20260310170626.png]]
our full equation for $\Delta$ will be
$$
\Delta=\Delta_{D}\lambda_{D}+\Delta_{L_{ST}}\gamma_{L_{ST}}+\Delta_{L_{LT}}\gamma_{L_{LT}} | \text{in distance, like inches}
$$
Our Deltas will be calculated by using
$$
\begin{align}
\lambda_{\Delta}&=\frac{\xi}{1+50\rho'} & \rho'&=\frac{A's}{(b_{w}\times d)} | \text{ Midspan only}
\end{align}

$$
Where $\xi=$ time dependent factor for sustained load 

we will have to calculate the $\lambda_{\Delta}$ for both dead and live load. 

---

Example 
$\omega_{D}=1.65$
$\omega_{L}=3.3$
both are in kips per foot.

After extensive calculations, we conclude that 
$I_{e}^+=13340\text{ in}^4$
$I_{e_{1}}^-=11366\text{ in}^4$
$I_{e_{2}}^-=11366\text{ in}^4$
$$
I_{e}=0.5I_{e}^++0.25(I_{e_{1}}^-+I_{e_{2}}^-)
$$
$$
I_{e}=12395\text{ in}^4
$$
And now, for our short term deflection calculations
$$
\Delta_{D+L}=0.295\text{ in}
$$
$$
\begin{align}
\Delta_{D}=\frac{\Delta_{D+L}\times \omega_{D}}{\omega_{D}+\omega_{L}}=\frac{1.65}{4.95}\times 0.295\\
\Delta_{L}=\frac{\Delta_{D+L}\times \omega_{L}}{\omega_{D}+\omega_{L}}=\frac{3.3}{4.95}\times 0.295
\end{align}
$$
using this we can now calculate our final deflection after long term.

note that in the question, there is no compression bar so we have no $p'$ meaning that our $\xi$ values will be 3, 2, or 1

![[Pasted image 20260310175712.png]]

---

Quiz 23

$\omega_{D}=2$
$\omega_{L}=3$
$E_{C}=3600\text{ ksi}$
$I_{e}=12000\text{ in}^4$
$\Delta_{D+L}=\frac{9600000}{E_{C}I_{e}}=0.222$

$$
\begin{align}
\Delta_{D}=\frac{\Delta_{D+L}\times \omega_{D}}{\omega_{D}+\omega_{L}}=\frac{2}{5}\times 0.222=0.0888\text{ in}\\
\Delta_{L}=\frac{\Delta_{D+L}\times \omega_{L}}{\omega_{D}+\omega_{L}}=\frac{3}{5}\times 0.222=0.1332\text{ in}
\end{align}
$$
Quiz 24

if $A's$ at the mid span is 2#9, $A's= 2\text{ in}^2$ , find the $\Delta$ for Dead, live short term and live long term

Calculate $\rho'$

$$
\rho'=\frac{A's}{b_{w}\times d}=\frac{2}{10\cdot20}=0.01
$$

Now we can calculate the $\Delta$ for the rest

$$
\begin{align}
\lambda_{\Delta_{D}}=\frac{\xi}{1+50\rho'}=\frac{2}{1+50\left(0.01\right)}=1.333 \\
\lambda_{\Delta L_{LT}}=\frac{\xi}{1+50\rho'}=\frac{3}{1+50\left(0.01\right)}=2 \\
\lambda_{\Delta L_{ST}}=1
\end{align}
$$

Quiz 25

if long term live load is 30%, (short term will be 70%), calculate the total $\Delta$

$$
\Delta=\Delta_{D}\lambda_{D}+\Delta_{L_{ST}}\gamma_{L_{ST}}+\Delta_{L_{LT}}\gamma_{L_{LT}}
$$
$$
\Delta=0.0888\times 1.333 +70\%\times 0.1332 \times 1 + 30\%\times 0.1332 \times 2 = 0.2915\text{ in}
$$
Quiz 26

Calculate $\Delta$ if our short term live load is 100%

$$
\Delta=0.0888\times 1.333 +100\%\times 0.1332 \times 1 + 0\%\times 0.1332 \times 2 = 0.2515\text{ in}
$$
---
Special case methods;

if we have strange shaped cross section shape, we can force it into an I-shaped beam for easier calculation.

