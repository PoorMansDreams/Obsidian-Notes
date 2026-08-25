
Axial compression is basically the compressive force going down on the concrete column.

The way it is designed is with the following equation.
NOTE $D_{c}$ is the diameter of the concrete
S is the PITCH, of distance between the spirals inside the column. (There is a spiral inside the column)

$A_{sp}$ is the cross sectional area of the spiral wire, so $A_{sp}=\frac{\pi d_{c}^2}{4}$

Spiral rebar concrete is good, but NOT GOOD IN EARTH QUAKE AREAS. DONT USE SPIRAL DESIGN IN A COLUMN IN A EARTHQUAKE AREA

![[Pasted image 20260414171101.png]]

This is to ensure buckling does not happen from compression. 
When calculating MAXIMUM tie spacing, we use the smaller $d_b$ (diameter rebar)

Between the three, find the minimum, (this will be the max), conservative
![[Pasted image 20260414171051.png]]


For a **beam column**

![[Pasted image 20260414172534.png]]

The **minor** side/moment means that there a bending moment on the weaker side (thinner side) 

we can calculate moment by also apply eccentricity, $e$

$$
\begin{align}
M_{u}=e\cdot P_{u} && e=\frac{M_{u}}{P_{u}}
\end{align}
$$

Quiz #29 if we have $P_{u}=400\text{ k}$ and $M_{u}=600\text{ ft-kip}=1.5\text{ ft}=18\text{ in}$
$$
e=\frac{600\text{ ft-kip}}{400\text{ kip}}
$$
In short, this is basically the equation for Moment, $M=F \times d$, force times distance


The Moment capacity is given as $M_{n}$ while $Pn$ is the axial loading capacity. 
![[Pasted image 20260414175521.png]]

For massive structures, couplers are often used because of the required length of the rebar. 

Rebar placement is very important, it is integral to have rebar only on the sides where it is utilized fully for moment. 

---

Example 1

![[Pasted image 20260414182140.png]]

in this case, our h is 25, which is parallel with e, (always is)

![[Pasted image 20260414182244.png]]

For our first load case, 
We first find our design/ultimate force $P_{u}$

$$
P_{u}=1.2(P_{D})+1.6(P_{L})
$$
Then we find Ultimate moment

$$
M_{u}=1.2(M_{D})+1.6(M_{L})
$$

use the equation $K_{n}$

Note, $A_{g}$ is the cross sectional area $A_{g}=20\times 25=500$
$$
K_{n}=\frac{P_{u}}{\phi f'c A_{g}}
$$

$$
R_{n}=\frac{M_{u}}{\phi f'c A_{g}h}=\frac{P_{u}\times e}{\phi f'c A_{g}h}
$$

After calculating, we use graph A-7 to find what $p_g$ is, in this case, it is 

$p_g=0.024=2.4\%$

knowing this, we apply it to our $As$ formula

$$
\begin{align}
p=\frac{As}{bh} \\
As=pbh=0.024\times 20 \times 25 = 12 \text{ in}^2
\end{align}
$$

So in short, we'd need at lease 12 in$^2$ worth of steel. Translates to Twelve #9 rebars. 

![[Pasted image 20260414182920.png]]


---
Example 2

![[Pasted image 20260414183807.png]]

We need to calculate B and H, (dimensions). 
In this case, we assume there are rebar on the left and right side. 

![[Pasted image 20260414183846.png]]

In this case, we do it the other way around when it comes for the graph. We assume what $p_{g}$ is, which is 0.03. (less than 4%). Then we use that to find what $K_{n}$ is. We can then find out what our $B$ is.

We will have to assume what $h$ is initially. So in this case we guessed 25 inches. 
note, $A_{g}=b\times h$
$$
\begin{align}
K_{n}=\frac{P_{u}}{\phi f'c A_{g}} \\
A_{g}=\frac{P_{u}}{\phi f'c K_{n}} \\
b=\frac{P_{u}}{\phi f'c K_{n} h}
\end{align}
$$