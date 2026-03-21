
![[Pasted image 20260317141328.png]]

We will be using Rankine's method to solve for all the lateral earth pressures in the walls.

--- 

#### Wall A

$\gamma_{bulk}=100 \frac{\text{lb}}{\text{ft}^3}$ and $\gamma_{sat}=119 \frac{\text{lb}}{\text{ft}^3}$
i). Neglecting wall roughness basically means we use Rankine's method.

Solving for section **at the top of the soil** 
$q$ is the surcharge on top of the soil
from solution, $e=\sigma'_{h,a}$
$$
\begin{align}
K_a = \frac{1 - \sin \phi'}{1 + \sin \phi'} = \tan^2 \left( 45 - \frac{\phi'}{2} \right) =\tan^2\left( 45-\frac{33}{2} \right)=0.291\\
\sigma'_{h,a} = K_a \sigma'_v - 2c' \sqrt{K_a} \\
o'_{h,a}=(q+\gamma z)K_{a}-2c\sqrt{ K_{a} }
\end{align}
$$
this section is at the top, so $z=0$ and we don't have a cohesion, so $c=0$
$$
\sigma'_{h,a,1}=(420+0)\times 0.291-0=122.22 \frac{\text{lb}}{\text{ft}^3}
$$

now we have to solve for the section **at the ground water table**, we use the same $K_{a}$
$$
\sigma'_{h,a,2}=(420+100\cdot 6.6)\times 0.291-0=314.28 \frac{\text{lb}}{\text{ft}^3}
$$
now we have to solve for the section **below the groundwater table**, same $K_{a}$
$$
\sigma'_{h,a,3}=(420+(100\cdot 6.6)+(119-62.4)\cdot 19.8)\times 0.291-0=640.397 \frac{\text{lb}}{\text{ft}^3}
$$
now we have to lateral earth pressure of the water itself 
$$
u=\gamma_{w}\times 19.8=62.4\times 19.8 =1235.52\frac{\text{lb}}{\text{ft}^3}
$$

ii.) given our $\delta=\frac{2}{3}$ we need to use Coulombs method
$$
K_a = \frac{\sin^2(\beta + \phi')}{\sin^2 \beta \sin(\beta - \delta) \left[ 1 + \sqrt{\frac{\sin(\phi' + \delta) \sin(\phi' - \alpha)}{\sin(\beta - \delta) \sin(\beta + \alpha)}} \right]^2} =0.26
$$
in this case, $\beta=90^\circ$ $\phi=33^\circ$ $\delta=\frac{2}{3}\times 33^\circ=22^\circ$ $\alpha=0^\circ$

we can use the same equations as we did last time, but just with a different $K_{a}$
$$
\begin{align}
\sigma'_{h,a,1}=(420+0)\times 0.26-0=109.2 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,2}=(420+100\cdot 6.6)\times 0.26-0=280.8 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,3}=(420+(100\cdot 6.6)+(119-62.4)\cdot 19.8)\times 0.26-0=572.1768 \frac{\text{lb}}{\text{ft}^3} \\
u=\gamma_{w}\times 19.8=62.4\times 19.8 =1235.52\frac{\text{lb}}{\text{ft}^3}
\end{align}
$$
---

#### Wall B

i). Using rankine
This soil on this wall doesn't rest perfectly straight, it's at an angle. So we have to make a imaginary vertical line. Everything else is the same, but we have no surcharge. $K_{a}=0.291$ since our $\phi$ is the same

$$
\sigma'_{h,a,1}=(0+0)\times 0.291-0=0 \frac{\text{lb}}{\text{ft}^3}
$$

$$
\sigma'_{h,a,2}=(0+100\cdot 6.6)\times 0.291-0=192.06 \frac{\text{lb}}{\text{ft}^3}
$$
$$
\sigma'_{h,a,3}=(0+(100\cdot 6.6)+(119-62.4)\cdot 19.8)\times 0.291-0=518.17788 \frac{\text{lb}}{\text{ft}^3}
$$
$$
u=\gamma_{w}\times 19.8=62.4\times 19.8 =1235.52\frac{\text{lb}}{\text{ft}^3}
$$

ii). Using Coulomb, $K_{a}$ will be different from our first because of the new angles
in this case, $\beta=76^\circ$ $\phi=33^\circ$ $\delta=\frac{2}{3}\times 33^\circ=22^\circ$ $\alpha=0^\circ$ 
$$
K_{a}=0.38
$$
using the same equations again, 
$$
\begin{align}
\sigma'_{h,a,1}=(0+0)\times 0.38-0=0 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,2}=(0+100\cdot 6.6)\times 0.38-0=250.8 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,3}=(0+(100\cdot 6.6)+(119-62.4)\cdot 19.8)\times 0.38-0=676.65 \frac{\text{lb}}{\text{ft}^3} \\
u=\gamma_{w}\times 19.8=62.4\times 19.8 =1235.52\frac{\text{lb}}{\text{ft}^3}
\end{align}
$$
---

#### Wall C

i.) Same wall, but the backslope is raised where $\alpha=10^\circ$
$$
K_a = \cos \alpha \frac{\cos \alpha - \sqrt{\cos^2 \alpha - \cos^2 \phi'}}{\cos \alpha + \sqrt{\cos^2 \alpha - \cos^2 \phi'}}=0.31
$$
we use the same equations again as well
$$
\begin{align}
\sigma'_{h,a,1}=(0+0)\times 0.31-0=0 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,2}=(0+100\cdot 6.6)\times 0.31-0=204.6 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,3}=(0+(100\cdot 6.6)+(119-62.4)\cdot 19.8)\times 0.31-0=552.01 \frac{\text{lb}}{\text{ft}^3} \\
u=\gamma_{w}\times 19.8=62.4\times 19.8 =1235.52\frac{\text{lb}}{\text{ft}^3}
\end{align}
$$
The lateral earth pressure direction will be at an angle, **this angle is the same as the ground surface inclination** so the angle the lateral earth pressure is at is $10^\circ$ 

ii.) Using Coulomb, 
$\beta=90^\circ$ $\phi=33^\circ$ $\delta=\frac{2}{3}\times 33^\circ=22^\circ$ $\alpha=10^\circ$ $K_{a}=0.30$
$$
\begin{align}
\sigma'_{h,a,1}=(0+0)\times 0.30-0=0 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,2}=(0+100\cdot 6.6)\times 0.30-0= 198\frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,3}=(0+(100\cdot 6.6)+(119-62.4)\cdot 19.8)\times 0.30-0= 534.204\frac{\text{lb}}{\text{ft}^3} \\
u=\gamma_{w}\times 19.8=62.4\times 19.8 =1235.52\frac{\text{lb}}{\text{ft}^3}
\end{align}
$$
---

#### Wall D

This wall has both a inclined wall and a inclined ground surface (backslope)

i). We have to use the imaginary wall again for Rankine, but this imaginary wall will be SLIGHTLY taller.
use $K_{a}$ that includes $\alpha$ $K_{a}=0.31$


$$
\sigma'_{h,a,1}=(0+0)\times 0.31-0=0 \frac{\text{lb}}{\text{ft}^3}
$$

$$
\sigma'_{h,a,2}=(0+100\cdot (6.6+6.6\tan 10))\times 0.31-0=240.653 \frac{\text{lb}}{\text{ft}^3}
$$
$$
\sigma'_{h,a,3}=(0+(100\cdot (6.6+6.6\tan 10))+(119-62.4)\cdot 19.8)\times 0.31-0=588.0638 \frac{\text{lb}}{\text{ft}^3}
$$
$$
u=\gamma_{w}\times 19.8=62.4\times 19.8 =1235.52\frac{\text{lb}}{\text{ft}^3}
$$
ii.) Solving for Coulomb, 
$\beta=76^\circ$ $\phi=33^\circ$ $\delta=\frac{2}{3}\times 33^\circ=22^\circ$ $\alpha=10^\circ$ $K_{a}=0.44$

$$
\begin{align}
\sigma'_{h,a,1}=(0+0)\times 0.44-0=0 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,2}=(0+100\cdot 6.6)\times 0.44-0=290.4 \frac{\text{lb}}{\text{ft}^3} \\
\sigma'_{h,a,3}=(0+(100\cdot 6.6)+(119-62.4)\cdot 19.8)\times 0.44-0=783.49 \frac{\text{lb}}{\text{ft}^3} \\
u=\gamma_{w}\times 19.8=62.4\times 19.8 =1235.52\frac{\text{lb}}{\text{ft}^3}
\end{align}
$$
remember, the $\delta+\text{perpendicular of wall}$ is the angle of the force from the soil.

---

![[Pasted image 20260319141348.png]]

For this questions we will be using Rankine's method, which means we will have an invisible wall.

we use the equation 

$$
\begin{align}
K_{a_{1}} = \frac{1 - \sin \phi'}{1 + \sin \phi'} = \tan^2 \left( 45 - \frac{\phi'}{2} \right) =\tan^2\left( 45-\frac{20}{2} \right)=0.49 \\ \\
K_{a_{2}}=\tan^{2}\left(45-\frac{30}{2}\right)=0.3333 \\
K_{a_{3}}=\tan^{2}\left(45-\frac{40}{2}\right)=0.217 \\
\sigma'_{h,a} = K_a \sigma'_v - 2c' \sqrt{K_a} \\
o'_{h,a}=(q+\gamma z)K_{a}-2c\sqrt{ K_{a} }
\end{align}
$$
only difference now is that we have to worry about the cohesions of the soils. When there are multiple different cohesions, we have to worry about the interfacing of the soils.

starting off, for the point at the soil surface 

$$
\sigma'_{h_{1}}=(1000+0)K_{a_{1}}-(2\cdot 400 \cdot \sqrt{ K_{a_{1}} })
$$
for the bottom of the soil layer 1, right before it reaches layer 2
$$
\sigma'_{h_{2}}=(1000+118\cdot 3.3)K_{a_{1}}-(2\cdot 400\cdot \sqrt{ K_{a_{1}} })
$$
this is for the top of the soil layer 2, 
$$
\sigma'_{h'_{2}}=(1000+118\cdot 3.3)K_{a_{2}}-(2\cdot 0\cdot \sqrt{ K_{a_{2}} })
$$
for when the ground water able starts, 
$$
\sigma'_{h_{3}}=(1000+118\cdot 3.3+116\cdot 3.3)K_{a_{2}}-0
$$
at the bottom of the 2nd soil layer
$$
\sigma'_{h_{4}}=[1000+118\cdot 3.3+116\cdot 3.3+(116-62.4)\cdot 3.3]K_{a_{2}}-0
$$

at the top of the 3rd soil layer

$$
\sigma'_{h'_{4}}=[1000+118\cdot 3.3+116\cdot 3.3+(116-62.4)\cdot 3.3]K_{a_{3}}-0
$$
now, finally, at the bottom of the 3rd soil layer

$$
\sigma'_{h'_{4}}=[1000+118\cdot 3.3+116\cdot 3.3+(116-62.4)\cdot 3.3+(120-62.4)\cdot 6.6]K_{a_{3}}-0
$$

We will also have to account for the lateral pressure due to the water as well. 
$$
u=(3.3+6.6)(62.4)=617.76\frac{\text{lb}}{\text{ft}^3}
$$

