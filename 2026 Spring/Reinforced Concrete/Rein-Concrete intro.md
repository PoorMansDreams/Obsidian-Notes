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
\rho_{max}=\rho0.004=0.85\times \beta_{1}\cdot \frac{f'c}{fy}\cdot \frac{\epsilon _{u}}{\epsilon_{u}+0.004}, \epsilon_{u}=0.003, \beta_{1}=0.85
$$
$$
\rho_{max}=0.021
$$


 ![[Pasted image 20260127182019.png]]
##### HW problem 1
![[Pasted image 20260129150638.png]]

4x #8 bars, As = 0.79 x 4 = 3.16 in^2

$$
a=\frac{3.16\times 60}{0.85\times 4 \times 12}=4.647\text{ in}
$$
Calculate for $\beta_{1}$
$$
\beta_{1}=0.85-0.05(\frac{4000\text{psi}-4000\text{psi}}{1000\text{psi}})=0.85
$$
Calculate for c, using $\beta_{1}$ and $a$
$$
c=\frac{a}{\beta_{1}}=\frac{4.647\text{ in}}{0.85}=5.467 \text{ in}
$$
There is only one layer of rebar in this problem, so $d=dt=20-2.5=17.5\text{ in}$
we can now use these values to find what $\phi$ is
$$
\begin{align}
\phi&=0.65+0.25\left( \frac{dt}{c}-\frac{5}{3} \right) \\
\phi&=0.65+0.25\left( \frac{17.5}{5.467}-\frac{5}{3} \right)=1.033
\end{align}

$$
note that our $\phi>0.9$ the beam is not up to code
pmin and pmax?
$$
\begin{align}
p_{min}=\frac{3\sqrt{ 4000 }}{60000}=0.0032\\
p_{min_{2}}=\frac{200}{60000}=\boxed{0.0033} \\ \\
P_{max}=0.85(0.85)\left( \frac{4}{60} \right)\left( \frac{0.003}{(0.003+0.004)} \right)=\boxed{0.021}
\end{align}
$$
$$
\rho=\frac{4}{12\cdot 17.5}=0.019
$$
note that $p_{min_{2}}<\rho<p_{max}$ so it's all good.
Now we can calculate for the Mu, the ultimate loading
$$
M_{u}=\phi M_{n}=1.033 \times 3.16\times 60\left( 17.5-\frac{4.647}{2} \right)=2972.42\text{ in-kips}
$$

---
A second case that could happen is a beam design problem
We are given everything EXCEPT $a$, so in this case we just adjust the equation we use to solve for Mu, since we are given Mu
$$
\begin{align}
M_{n}=A_{s}f_{y}\left( d-\frac{a}{2} \right) \\
M_{n}=\frac{M_{u}}{\phi} \\
M_{u}=\frac{A_{s}f_{y}\left( d-\frac{a}{2} \right)}{\phi}
\end{align}
$$
long ahh derivation
$$
a=d\left[ 1-\sqrt{ 1-\frac{4M_{u}}{1.7\phi f'c\times b\times d^2} } \right]
$$
we need a for $\phi$ but we don't have a, so we just assume a number for $\phi$ instead.
remember, $\phi$ must be within 0.65 < $\phi$ < 0.9
once we assume a good $\phi$, we can use it to find $A_{s}$
$$
A_{s}=\frac{0.85f'c\times b\times a}{f_{y}}
$$

---
##### Example 2
b=10"
h=20"
As=?
f'c=4ksi
fy=60ksi
Mu=1300 in-kip
from the diagram, d is 20-2.5=17.5

$$
\begin{align}
a=d\left[ 1-\sqrt{ 1-\frac{4M_{u}}{1.7\phi f'c\times b\times d^2} } \right] \\
a=17.5\left[ 1-1\sqrt{1-\frac{4(1300)}{1.7\phi(4)(10)(17.5^2)} } \right]
\end{align}
$$
after assuming that $\phi=0.9$
$$
a=2.62\text{ in}
$$
$$
A_{s}=\frac{0.85(4)(10)(2.62)}{60}=1.49\text{ in}^2
$$
we can then finally calculate for c and $\beta_{1}$
$$
\beta_{1}=0.85-\frac{(4000)-4000}{1000}\times 0.05=0.85
$$and to calculate for c
$$
c=\frac{a}{\beta_{1}}=\frac{2.62}{0.85}=3.09\text{ in}
$$
now we can calculate the $\epsilon_{t}$
$$
\epsilon_{t}=e_{u}\left( \frac{d-c}{c} \right)=0.003\left( \frac{17.5-3.09}{3.09} \right)=0.014
$$
our calculated $\phi$ is greater than our assumed $\phi$ so we just used the assumed, which is 0.9
our As=1.49 square inches, to achieve this, we need to get a combination of rebar cross sections that can add up to a number greater than 1.49 but not too much. 

for example, 2 #7 and 1 #6 rebar, which will be 
$$
2 \times 0.44+1\times 0.6= 1.48 
$$
