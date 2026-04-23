
Slender Columns (long columns that can buckle). When a column is under compression, it may buckle. When it buckles, it will cause the column to deform and create a distance between the force and the material. 

![[Slender Column 1|100]]
![[Pasted image 20260421171408.png]]

![[Pasted image 20260421171429.png]]

Q is the stability index, if it is GREATER than 0.05, it will have **sway**. If the Q index is less than 0.05, there will be no sway. 

The sway or moment will be about the y-direction. (Y goes into the page)

$$
I_{e}=0.7\times I_{g}
$$
This is an example of what $I_{e}$ would be for columns. (look at column). 
for beams, the $I_e$ is half as effective. 

For RECTANGULAR shaped beam, $I_{e}=0.35I_{g}$
For T shaped beams, $I_{e}=2\times 0.35I_{g}$

![[Pasted image 20260421172209.png]]

For point A, two columns come to point A, so then then there could be two $\frac{EI}{l_{c}}$ for the numerator and denominator for $\psi$ 

When the column is at the ground at a fixed point, then $\psi=1$, and for hinged points $\psi=10$

For non-sway structures, K can be less than 1. For sway structures K is greater than 1. 

![[Pasted image 20260421173113.png]]
**note we are doing non-sway structures**
Steps to calculate are
1. Find $I_{e}$ for beam/column
2. Find K
3. $$\frac{kl_{u}}{r}\leq\text{min}$$
4. Min $[34+12\left( \frac{M_{1}}{M_{2}} \right)\text{ and }40]$
$r$ is the radius of gyration, which is $r=\sqrt{ \frac{I}{A} }=\sqrt{ \frac{a^2}{12} }$
A trick is that $r=0.3h$, $h$ being the column dimensions. 

For double curves (two moments are going the same way) BOTH moments are POSITIVE

For single curve (two moments are going against each other) The moment will be NEGATIVE. 

If the calculated $\frac{kl_{u}}{r}$ is greater than the minimum, it will be considered a slender column,
If the calculated $\frac{kl_{u}}{r}$ is less than the minimum (0.05) it will be considered a short column. Proceed to just go through the whole graph process that uses $R_{n}$ and $K_{n}$

![[Pasted image 20260421174220.png]]

We will have to magnify the moment we calculated, this is due to the buckling effect. (We need more moment resistance because of risk of buckling). 

The moment magnification factor must be at lease 1. Never less than 1. 

$P_{c}$ is the buckling load. The effective EI is calculated in the equation seen above. It uses $E_{c}$ and $I_g$.
For creep effect, it will be the dead load divided by the dead load and live loads. 

$P_{u}$ is the ultimate force on the column. (dead and live load)

$\beta_{dns}$ is for NON SWAY. 

![[Pasted image 20260421174714.png]]

$C_{m}$ is the moment magnification factor. It must be less than 1.4.

For single $C_{m}$
$$
1.4>C_{m}=0.6-0.4 \frac{M_{1}}{M_{2}}\geq 0.4
$$


---

Example 
![[Pasted image 20260421175256.png]]

First find $P_{u}$
$$
P_{u}=1.2\times P_{D}+1.6\times P_{L}=(1.2\cdot 230)+(1.6\cdot 173)=553\text{ kips}
$$

For the double curve, $M_{t}=2$ and $M_{b}=2$ in ft-kips

For the moment at the TOP
$$
M_{ut}=(1.2\cdot 2)+(1.6\cdot 108)=175 \text{ ft-kips} 
$$
For the moment at the BOTTOM

In this case, we considered clockwise to be positive,
and anti-clockwise to be negative. 

**NOTE** the direction matters, not the sign. (we basically just add up the directions for the top and bottom)
$$
M_{ub}=(1.2\cdot 2)+(1.6 \cdot 100)=157.6\text{ ft-kips}
$$

The top will be going clockwise moment, 
the bottom will be going anti-clockwise moment. 

This will cause us to have a single curve moment. (Looks like the Live-Load diagram)

$M_{2}$ will be max,
$M_{1}$ will be min. 
Remember, $M_{2}>M_{1}$, So our $M_{2}=175$ and $M_{1}=157.2$

![[Pasted image 20260421180257.png]]

Since this is for columns we use $I_e=0.7I_{g}=0.7\left( \frac{bh^3}{12} \right)$
$l_{c}$ is the distance between the centers of the junctions/joints which is 14 feet. 


For the beam, it is a T shaped beam, so $I_{e}=2\times 0.35I_{g}$
The base of the beam is 48", the height of the beam is 12" 

we now use the $\psi$ formula.

$$
\psi=\frac{(\sum \frac{EI}{l_{c}})_{\text{column}}}{(\sum \frac{EI}{L})_{\text{beam}}}
$$

notice that we will have the same $E$ across all terms, We then just need to use $\frac{I}{l_{c}}$ and $\frac{I}{l_{b}}$
NOTICE we already calculated it $\frac{I}{l_{c}/l_{b}}$, our $\phi_{a}=\phi_{b}$ because throughout the whole structure, it is all similar. 

From this, we see that our k value is $k=0.87$

$$
\frac{kl_{u}}{r}=\frac{0.87\times 13 \times 12 }{0.3 \times 18}=25.1
$$

Using the last equation in the above image, we see that it is 23.2,

Our $\frac{kl_{u}}{r}$ value is greater than our min, so that means the column will be considered **slender**. 
![[Pasted image 20260421182809.png]]

for $M_{2}min$ the h is the dimension of the column, 

![[Pasted image 20260421183053.png]]

Finally we can conclude that the magnification factor for the moments is 1.15. Using the calculated $C_{m}$ When finding the amount of steel needed for the column, we use the standard method we did before, using tables. 

Unfortunately our $\gamma$ is 0.72, meaning we might have to do some interpolation to find the exact $P_{g}$ value. 
 
We find that the required area of steel is 8.42 in$^2$ 


