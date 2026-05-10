![[Pasted image 20260317170658.png]]

The bond between concrete and steel is much stronger,

the $L_{d}$ is the depth of the rebar inside the beam. The $L_{d}$ required is based on several factors, including diameter of the rebar, the material it is inside, and the lateral force that is acting on the rebar.

$d_{b}=\text{diameter rebar}$

However, how deep does the rebar have to be inside the support? (beam is connected to support)
The rebar should have the same depth in BOTH the beam and the support. 

![[Pasted image 20260317171613.png]]

$$
\text{Max}=
\begin{cases}
\geq \left( \frac{f_{y}\psi_{r}}{50\lambda \sqrt{ f'c }} \right)d_{b}\\
\geq0.0003f_{y}d_{b}
\end{cases}
$$
The maximum MUST be greater than 8 inches.

![[Pasted image 20260317172322.png]]
This is the simplified method, which is much easier to use and very conservative. 

![[Pasted image 20260317172926.png]]

We also have to worry about where the rebar is located as well. If the concrete depth below the rebar is greater than 12", then it is considered a topbar. If the rebar is a top bar, the air from the drying concrete may get trapped UNDERNEATH the rebar. 

![[Pasted image 20260317174548.png]]

To calculate this, we first need to find the dimensions of the crossection. 

the spacing, or $S_{c}$ is 3.43", 
and the cover depth 1.875"

There is also more than 12 inches of fresh concrete below the rebar. 

note, $\psi_{t}\psi_{e}\leq 1.7$
the final would be
$$
87\text{ in} \times \frac{As_{re}}{As_{pro}}=87\times \frac{2.9}{3.12}=81\text{ in}
$$
---
Quiz 27

Find Sc, given two legs are #4, and there are 2 #8 top rebars on the left and right side. (4 total rebars on top), total width of 14"
**Note** remember to use DIAMETER, not cross sectional area
first find the variables
$$
\begin{align}
\text{cover}=1.5 \\
d_{s}=\text{number 4 rebar}=0.5 \\
b=14
\end{align}
$$
$n=\#\text{of rebars}$
$$
\begin{align}
Sc=\frac{b-2\times c-2d_{s}-nd_{b}}{n-1} \\
Sc=\frac{14-2(1.5)-2(0.5)-4(1)}{4-1}=2\text{ in}
\end{align}
$$

This is less than $d_{b}$ so we are ok.

---

A hooked bar gives us more variables to work with 
![[Pasted image 20260317181443.png]]

To be able to use 0.75, the distance between the top bar and the top of the beam must be smaller than 2.5" ($1.5+d_{s}\geq 2.5$)

The beam might be greater be greater than the beam size, so then $m+1.5+d_{s}\geq 2.5$
where $m=\frac{h-b}{2}$ , $h$ is the height of column, and $b$ is the height of the beam. 

The spacing between the ties should be less than three times the diameter of the rebar in the beam. 

![[Pasted image 20260317182927.png]]

the tail MUST be covered by at lease 2 inches of cover 


We also have new bolt-headed type rebars. 

![[Pasted image 20260317183421.png]]

![[Pasted image 20260317184205.png]]

