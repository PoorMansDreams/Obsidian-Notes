
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
V_{u}\times \phi=6263\text{ lb}>V_{n} \text{ OK}
$$




