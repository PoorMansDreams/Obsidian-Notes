#reinforcedconcrete
Concrete is strong in compression, but weak in tension. A perpendicular force on a concrete beam will cause the beam to have tension on the bottom, and compression on the top. 

We add rebar in the bottom of the concrete so that it can take the tension. The rebar is usually made of steel. The rebar must be deformed and have indents so that the steel and concrete can have a strong grip on each other. 

Despite having rebar inside the concrete, there still may be flexure cracks that form in the concrete. The rebar is still taking the tension force however. 

![[Pasted image 20260120180047.png]]

On a section where moment is positive, the rebar should be on the bottom. 

Sulfates and Chloride can degrade and weaken concrete. To combat this, we use Type V concrete, which is resistant to sulfates. 

In a beam with negative moment, there is tension on the top, and compression on bottom
In a beam with positive moment, there is tension on the bottom, and compression on top

---
Definitions for concrete with steel reinforcement
![[Pasted image 20260127171452.png]]
b is the width of the concrete beam. 
dt is the distance between the concrete side and the furthest rebar row
when there is two or more sets of rebar, we have "d"
d is the distance between the concrete side and the **center** of the rebar rows

---
Strain and Stress & Neutral Axis 
Strain is the change in length compared to the total length of the material
Strain: $\epsilon=\frac{\Delta L}{L}$
Stress is the force exerted by the concrete which is just the strain times the **modulus of elasticitiy**
Stress: $\sigma=\epsilon \cdot E_{c}$

![[Pasted image 20260127172324.png]]

should memorize $\epsilon_{u}=0.003$
C is the compression
dt-c is tension. 
A balance failure means that the steel and concrete reach their maximum values. 
$$\epsilon_{y}=\frac{fy}{E_{s}}$$

fs = stress under fy
fy= the stress when the material starts to yield or deform. 
fu = ultimate stress, stress when the material fails 
for any steel, Es, or Modulus of Elasticity will be 29000 ksi, or kips per square inch. 

##### Practice Quiz 1
calc strain at yield point for grade 60 bar, 

Grade 60 means that the fy = 60 ksi, and we use Es is always 29000 ksi
$$
\epsilon_{y}=\frac{fy}{E_{s}}=\frac{60}{29000}=0.00206
$$

Percentage of tension bar, 
$$
\rho=\frac{As}{bd}=\frac{\text{Area of rebar}}{\text{width beam }\cdot \text{distance to rebar row}}=\frac{3}{10\cdot 17.5}
$$

![[Concrete 1 Ex|500]]


$$
\rho b=0.85\beta_{1}\cdot \frac{f'c}{fy}\cdot \frac{\epsilon _{u}}{(\epsilon_{u}+\epsilon_{y})}
$$

A structure has a capacity provided, we also have a required loading. One of the big requirements is that the Capacity provided by the material **must** be greater or equal to the required loading. We have to also put reduction values on the concrete we make because the designed concrete wont always be as strong as we think it will be, mostly due to production errors. 

Provided capacity = capacity provided
simply put, Mu is the ultimate loading, and Mn is the capacity the material can take
$\phi$ is a reduction factor that basically forces us to make a stronger capacity material to support the load. 
$$
M_{u}=\phi M_{n}
$$
$\phi$ has limits, defined
![[Pasted image 20260127175124.png]]

doesn't matter if we use per tension or per neutral, we will get the same. 

$$
\begin{align}
T&=C \\
Asfy&=0.85\cdot f'c\cdot ba \\
a&=\frac{Asfy}{0.85\cdot f'c\cdot b} \\
a&=\beta_{1}\cdot c
\end{align}
$$
a is the height of the compressed block,  C is the compression, $a$ is the height of the compressive force, and the 0.75f'c is the magnitude of the force. 

ds is the cover around the concrete, db is the diameter of the steel rebar, and the 1.5 is the cover around the whole concrete beam or bar 
$$
d_{t}=h-1.5-d_{s}-\frac{d_{b}}{2}
$$

---
#### Solved Example 1


Determine the Flexural strength of a rectangular beam according to the ACI code:

b = 12"
h = 12"
f'c = 4ksi 
fy = 60ksi

4x #9 rebars at the bottom, As = 4 inch squared
from the image, there is only 1 layer of rebar, so d=dt, from the top of the block to the middle of the row of rebar;
$$
d=d_{t}=20-2.5=17.5
$$

$$
a=\frac{4\cdot 60}{0.85 \cdot 4 \cdot 12}=5.88\text{ in}
$$
now time to find what $\beta_{1}$ is, at f'c is at 4000 psi, $\beta_{1}=0.85$
using this we can find what **c** is, 
$$
c=\frac{a}{\beta_{1}}=\frac{5.88}{0.85}=6.92\text{ in}
$$
now we can find what our $\phi$ is
$$
\phi=0.65+0.25\left[ \frac{dt}{c}-\frac{5}{3} \right]=0.65+0.25\left[ \frac{17.5}{6.92}-\frac{5}{3} \right]=0.87
$$
now we can calculate our minimums and maximums, 
when calcuing, we choose the pmin that is higher, (safer)
$$
\rho_{min}=\frac{3\sqrt{ f'c }}{fy}=\frac{3\sqrt{ 4000 }}{60000}=0.0032
$$
$$
\rho_{min}=\frac{200}{fy}=\frac{200}{60000}=0.0033
$$
$$
\rho_{min}=0.0033
$$
$$
\rho_{max}=\rho0.004=0.85\times \beta_{1}\cdot \frac{f'c}{fy}\cdot \frac{\epsilon _{u}}{\epsilon_{u}+0.004}
$$

 ![[Pasted image 20260127182019.png]]