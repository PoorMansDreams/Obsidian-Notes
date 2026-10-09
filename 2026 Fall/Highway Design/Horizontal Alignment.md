- Horizontal Alignments 
	- Simple Curves (just one arc with same radius throughout)
	- Compound Curves (similar, but has two arcs with two different radii, curves in the same direction)
for more information, refer to [[Topic 4 - Horizontal Curves]]

![[Pasted image 20260930172808.png]]

![[Pasted image 20260930173313.png]]

notice how the angle I/2 also shows up as the angle between the chord and tangent in PC. 

---
### Example Problems

![[Pasted image 20260930173417.png]]

I) Chord length can be calculated in the equation, HOWEVER we want to find the chord length between stakes (50 ft)

$$
\begin{align}
C_{1}&=2R \sin\left( \frac{\delta_{1}}{2} \right)\\
\frac{\delta_{1}}{I}&=\frac{l_{1}}{L} \\ 
L&=R\times I\times \frac{\pi}{180}=314.159 \\
\frac{\delta_{1}}{60}&=\frac{50}{314.159} \\
\delta_{1}&=9.549 \\

C_{1}&=300\times 2 \sin\left( \frac{9.549^\circ}{2} \right) \\
C_{1}&=49.94\text{ ft}
\end{align}
$$

II) Last central angle in degrees near the PT?

We know the central angle (I) is 60$^\circ$, and each "50 ft" stake creates a 9.549$^\circ$ 
we simply divide and subtract to find remainder
$$
\begin{align}
\frac{60}{9.549}=6.28 \\
60^\circ-(6\times 9.549^\circ)=2.706 ^\circ
\end{align}
$$

III) The length of the partial curve is findable, since we know what $\delta_{2}$ is, $\delta_{2}=2.706$
$$
\begin{align}
C_{2}=2R\sin\left( \frac{\delta_{2}}{2} \right) \\
C_{2}=2\times 300\sin\left( \frac{2.706^\circ}{2} \right) \\
C_{2}=14.167\text{ ft} \\
\end{align}
$$

### Problem 2
![[Pasted image 20260930175611.png]]

I) Determine the radius of the horizontal curve
we know that the chord length between A and B is 565.50 ft

To find the $I$ or deflection angle, we just find the 3rd angle formed from A, B and PI.
$T$ is the tangent length. 

$$
I =30^\circ 21'+27^\circ 43' = 58.07^\circ
$$
We will need to find the tangent length, which we use the law of sins using the interior triangle.
$$
\begin{align}
\frac{a}{\sin(27^\circ 21')}=\frac{565.50}{\sin(58.07 ^\circ)} \\
a=306.133
\end{align}
$$
a is the remaining length we have to add to 78+49 to get the total tangent length
$$
T=7849 + 306.133-7519=636.133\text{ ft}
$$
$$
\begin{align}
T&=R \tan \frac{I}{2} \\
636.133\text{ ft}&= R \left( \tan \frac{58.07^\circ}{2} \right) \\
R&=1145.96\text{ ft}
\end{align}
$$

II) Finding L, or length of the horizontal curve is
$$
\begin{align}
L=R\times I \times \frac{\pi}{180} \\
L=1145.96 \times 58.07\times \frac{\pi}{180} \\
L=1161.44\text{ ft}
\end{align}
$$

III) Finding the PT station, which means we simply need to add the length of the curve with PT
$$
1161.44+PC=PT
$$
$$
PT=1161.44+7519=8680.445
=86+80.445
$$

![[Pasted image 20260930182110.png]]

we know that the $I$ deflection angle is 68.4167$^\circ$

But we need to find the radius required, to find this, we know that the arc goes through point M.
this must mean that PT needs to have an a certain $T$ tangent distance. The x distance between M and PT can be denoted as $x$
$$
\begin{align}
T=x+278.75 \\
4430-T=PC \\
T=R\tan\left( \frac{I}{2} \right) \\
x+278.75=R\tan \frac{I}{2} \\
x+278.75=R\tan \left( \frac{68.4167}{2} \right) \\
 \\
x=R\tan(34.208)-278.75 \\
x=R\times 0.6798 - 278.75 \\
\end{align}
$$
if we imagine that there is a radius line that connects from the center of the arc, it will create a triangle

![[Pasted image 20260930182916.png|355]]

The triangle is **Green**, we know one of the distances to be x, use Pythagorean
$$
\begin{align}
x^2+(R-97.45)^2=R^2 \\
x=\sqrt{R^2 -(R-97.45)^2}
\end{align}
$$
now we can solve
$$
R\times 0.6798-278.75=\sqrt{R^2 -(R-97.45)^2}
$$
$$
R=1064.4\text{ ft}
$$

Now that we have R, we can solve for the Length of the Horizontal curve and PT station.
$$
L =R\times I\times \frac{\pi}{180}=1270.996'
$$
to find the PT station, we just subtract the tangent length from PI and then add L
$$
T=723.592
$$
$$
PT=PI-T+L=4977.4=49+77.4
$$

---
#### Sight Distance for Horizontal Curves

![[Pasted image 20261007172258.png]]

![[Pasted image 20261007172321.png]]

So in this case, we will calculate the adjusted Radius, and the distance between the centerline and the house is not the HSO. 
$$
R_{A}=425'-\frac{12}{2}'=419'
$$
$$
HSO=30'-6'=24'
$$

$$
\begin{align}
S=\frac{R_{A}}{28.65}(\cos^{-1}\left( 1-\frac{HSO_{A}}{R} \right)) \\
S=284.98
\end{align}

$$
---
#### Superelevation

![[Pasted image 20261007173127.png]]

![[Pasted image 20261007173201.png]]

We simply need to find $e$ which is the superelevation slope in ft/ft
$$
e=\frac{V^2}{15R}=\frac{65^2}{15\times 1482}-0.11=0.08 \frac{\text{ft}}{\text{ft}}
$$