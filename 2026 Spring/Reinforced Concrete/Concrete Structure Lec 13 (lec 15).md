
One way slabs are horizontal blocks that usually acts as a floor or ceiling. 

A one way slab can be identified if 

$$\frac{L_{A}}{L_{B}}>2$$

A two way slab can be identified if 
$$
\frac{L_{A}}{L_{B}}\leq2
$$
Where $L_{A}$ is the long length, and $L_B$ is the shorter length. It will also be a one-way slab if there are only two supports. 

Using reinforcements however, we are able to force a two-way slab to be a one-way slab. We put reinforcements parallel with $L_{B}$, this forces most of the load to be forced upon the supports along the length $L_{A}$. 

![[Pasted image 20260428174007.png]]

We are in grade 60 in this case. 

![[Pasted image 20260428174239.png]]

The thickness of the concrete should be considered by using the total length of the slab. 

the ratio $\rho$ is simply the percentage of rebar within the slab. 
$$
\frac{A_{s,one}}{Sd}
$$
---
Example, thickness of a slab is 5", $t=5$ 
We want to find $d$. $d$ is the distance between the top of the slab to the center of the rebar. 
lets say the rebar is a #4 rebar, meaning the diameter $d_{b}=0.5\text{"}$
so then $\frac{d_{b}}{2}+\frac{3}{4}=0.25+0.75=1$ 
$d=5-1=4\text{"}$


The clear cover MUST be at lease 3/4th an inch. 

If the rebar was a #8, then 
$\frac{d_{b}}{2}+\frac{3}{4}=\frac{1}{2}+\frac{3}{4}=1.25$
$d=5-1.25=3.75\text{"}$


$$
\frac{d_{b}}{2}+\text{clear cover}=\text{?}
$$

clear cover must be at lease 0.75

![[Pasted image 20260428180210.png]]

These are moment factors according to 

Simply supported (discontinuous end unrestrained) means the beam sits on the column (no moment cause it just sits there)

A spandrel is a beam that sits on the support

and "column" is a beam that sits on a column. 

To check for maximum shear, we will just use the 1.15 magnified version. If all the other beams pass, it will be fine. 


---
Example full

![[Pasted image 20260428181219.png]]

Start with the thickness of the of the slab, for spandrels, BOTH ends are continuous. so 
Times with 12 to turn it into inches.
$$
t=\frac{l}{28}=\frac{15\times 12}{28}=6.43\text{"} \approx 6.5''
$$
We use a standard weight of concrete of $150\text{ pcf}$ 
we multiply it by our thickness to get the weight per $\text{ft}^2$
$$
150\text{ pcf} \times \frac{6.5''}{12}=81\text{ psf}
$$

we then calculate the load per unit foot (in width)

$$
81\text{ psf}\times 1'=81\text{ lb/ft}
$$

This will be our dead load.

Our live load is given as $100\text{ psf}$

$$
100\text{ psf}\times 1' =100\text{ lb/ft}
$$
We then use these two to find the ultimate (factored) load

$$
w_{u}=81\times 1.2+100\times 1.6=257 \text{lb/ft}
$$
Using the table provided we can easily find the moments at each point of the beam

$$
M=\text{factor}\times w_{u}\times l_{n}^2
$$
$$
\begin{align*}
\text{At exterior support: } -M &= \frac{1}{24} \times 0.257 \times 15^2 = 2.41 \text{ ft-kips} \\
\text{At midspan: } +M &= \frac{1}{14} \times 0.257 \times 15^2 = 4.13 \text{ ft-kips} \\
\text{At interior support: } -M &= \frac{1}{9} \times 0.257 \times 15^2 = 6.43 \text{ ft-kips}
\end{align*}
$$
![[Pasted image 20260428182637.png]]

Based on these values, we can apply beam design. 
moment ult was multiplied by 12 and 1000 to convert to inch-pounds

NOTE, MUST be in lb-in
$$
As=\left[0.85f'c\cdot b\cdot d\left(1-\sqrt{1-\frac{\left|4Mu\right|}{1.7 \phi\ f'c\cdot b\cdot d^{2}}}\right)\right]\times \frac{1}{fy}
$$
$$
As=\frac{0.85(4000)(12)(5.5)\left( 1-\sqrt{ 1-\frac{4|2.41\times 12\times 1000|}{1.7(0.9)(4000)(12)(5.5^2)} } \right)}{60000}=0.099 \approx 0.1 \text{in}^2
$$

we continue this calculation for all the others, 
Our $As_{min}=0.0018bt=0.0018\times 12 \times 6.5=0.14\text{ in}^2$ 

Based on our calculated load, we can see that our $V_{u}$ is 

$$
V_{u}=1.15 \times\frac{ w_u \times L_{n}}{2}-d\times w_{u}=\frac{257\times 15}{2}-\frac{5.5}{12}\times 257=2100 \text{ lb}
$$

$V_{n}=V_{c}=2\lambda \sqrt{ f'c }\times bd=2\times 1 \times \sqrt{ 4000 } \times 12 \times 5.5=8350\text{ lb}$

our $\phi=0.75$ 

$$
V_{n}\times \phi=6263\text{ lb}>V_{u} \text{ OK}
$$

--- 

**Two Way Slabs**

For slabs,  $L_{B}$ is the longer side, and $L_A$ is the short side, 

when saying moment along the $L_{A}$ direction, imagine a beam parallel with $L_{A}$, the moment on that beam is what the moment is 

We have a chart that describes the different moments for different cases.

![[Pasted image 20260505172853.png]]

To use a chart like this, let's say $\frac{L_{a}}{L_{b}}=0.75$ and it is a Case 8. 

This means that 

$$
M_{u,a}^+=M_{uDL}^++M_{uLL}^+=(c_{a}\times w_{uD}\times L_{a}^2)+(c_{a}\times w_{uL}\times L_{a}^2)
$$
 This is similar for b as well
 
$$
M_{u,b}^+=M_{uDL}^++M_{uLL}^+=(c_{b}\times w_{uD}\times L_{b}^2)+(c_{b}\times w_{uL}\times L_{b}^2)
$$

![[Pasted image 20260505173345.png]]

![[Pasted image 20260505174711.png]]

For negative moments, the simply supported sides have zero moment, which is why some boxes are left empty 

![[Pasted image 20260505174826.png]]

This table is for shear, Lets say we have a 8x10 foot slab, $w_{D}=1\text{ kip/ft}^2$  and $w_{L}=2\text{ kip/ft}^2$

so, $w_{u}=1.2\times 1+1.6 \times 2 =4.4\text{ kip/ft}^2$
$$
\begin{align}
\frac{L_{a}}{L_{b}}=\frac{8}{10}=0.8 \\
\text{Case 3,} \\
w_{a}=0.33 \\
w_{b}=0.67
\end{align}
$$
This means that most of the load will go to the $L_{b}$ side, (the left and right side). In this case, this is because of the case 3, there is fixed points on the left and right. 

To calculate this,

$$
w_{u,a}=0.33\times 8 \times 10 \times 4.4 =116.16 \text{ kips}
$$

$$
w_{u,b}=0.67\times 8 \times 10 \times 4.4 = 235.84 \text{ kips}
$$

After finding the load, we have to divide it by two since there are two sides (116.16 kips is the TOTAL load on the slab

In this case (3), that means that there is $\frac{116.16}{2}\text{ kips}$ on the length $L_{b}$ . The shear per foot would be $\frac{116.16}{2}\text{ kip}/10\text{ ft}$ so, 5.808 kips per foot length on the $L_{b}$ side. (the shear comes from $w_{a}$)

That means that for the length $L_{a}$ we use the shear from $w_{b}$ so $\frac{235.84}{2}\text{ kips}/8\text{ ft}=14.74\text{ kip/ft}$ 


![[Pasted image 20260505180922.png]]

In this case, it is a spandrel beam or rigid, meaning it is supported ALL around, meaning it is a case 2. 

In the example, we will have to look at the negative and positive tables for both A and B sides. 

Doing the negative moment first, we simply find $w_{u}$ (Factored Load) and then multiplied it with $C_{a,neg}$ and $C_{b, neg}$

![[Pasted image 20260505181404.png]]

for shear, it is still a case 2, The $w_u=104$ so then

$w_{u,a}=0.71\times 104 \times 10 \times 12.5=9230\text{ lb}$ 
NOTE, This is the load for both sides, so we need to divide by 2 to make it for ONE side $\frac{9230}{2}=4615\text{ lb}$ 

Now, if we want to know the loading per unit length, it would be $\frac{4615\text{ lb}}{12.5\text{ ft}}=369.2\text{ lb/ft}$

---

