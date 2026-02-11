we have two equations
$$
\begin{align}
fc_{max}=\frac{My_{c}}{I} \\
ft_{max}=\frac{My_{t}}{I}
\end{align}

$$
for both, we will need the moment of inertia $I$
$$
I=\frac{bh^3}{12}
$$
If we have two beams that are glued, nailed, or just stuck together, the moment of inertia is about 4 times as greater than if the two beams were just put on top of each other
$$
\begin{align}
I_{\text{stacked}}&=\frac{bh^3}{12}\times 2 \\
I_{\text{glued}}&=\frac{b(2h)^3}{12}=\frac{bh^3}{12}\times 8
\end{align}
$$
 ---
 
 If we have tension, the direction of the tensions should be the same direction as the rebar. (it also causes concrete to crack perpendicular to the tensions direciton)

![[Concrete structure]]

The blue line indicates the steel rebar, while the red line indicates the possible tension direction. 

---

#### Concrete Shear Strength

![[Pasted image 20260210173738.png]]

Our nominal, or calculated shear that the concrete can handle is $V_{n}$ . Our ultimate shear is $V_{u}$
$$
\begin{align}
V_{n}&=V_{c}+V_{sr} \\
V_{uc}&= \phi V_{c}\\
V_{u}&=\phi V_{n} \\
\end{align}
$$

for $V_{c}$ we can use a simplified version, which is just
Note that for $\lambda$ ==we are ALWAYS using 1.== Lambda is the type of concrete we use. 
$$
V_{c}=2\lambda \sqrt{ f'c } \times b_{w}\times d
$$
note that $b_{w}\times d$ is the area, and $2\lambda \sqrt{ f'c }$ is force. Force times area is pressure/stress. Units should be **psi** 

for the stirrup shear strength, we will have to use another equation
$$
V_{sr}=\frac{A_{v}\times fyt\times d}{S}
$$
S is the spacing between the stirrups of the steel. 
$fyt$ is the shear reinforcement yield strength (psi)
$A_{v}$ is the total cross sectional area of the [^1]legs 

[^1]: A legs are the vertical portion of the steel rebar, the thing that looks like a 0 shape

We also have to know the $S_{\text{max}}=S_{\text{min}}$ as well which are given with these equations note that the MAXIMUM spacing is 24 inches, it is spaced too far. 
$$
\begin{align}
&=\frac{A_{v}\times fy}{0.75\sqrt{ f'c }\times bw} \\ \\

&=\frac{A_{v}\times fyt}{50bw} \\ \\

&=24\text{ in}
\end{align}
$$
We also have a $A_{v}$ minimum and maximum
$$
\begin{align}
&=\frac{0.75\sqrt{ f'c }\times b_{w}\times S}{fyt} \\
 \\
&=\frac{50b_{w}\times S}{fyt}
\end{align}
$$
---
##### Quiz 7
determine $V_{uc}$ if 
$f'c=4\text{ ksi}$
$fyt=60\text{ ksi}$
![[Concrete Quiz 7]]
first find d, which is 
$$
d=h-3-\frac{2}{2}=30-4=26
$$
our $b_{w}$, or width of the rectangular section will be 12 inches. 

$$
V_{c}=2\lambda \sqrt{ f'c } \times b_{w}\times d
$$
$$
V_{c}=2\times 1 \sqrt{ 4000 }\times 12\times 26
=39465 \frac{\text{lb }}{\text{in}^2}$$
$$
V_{uc}=\phi V_{c}=0.75 \times 39465=29599\frac{\text{lb }}{\text{in}^2}
$$

to calculate $V_{sr}$ 
we start by calculating $A_{v}$ which is the area of the legs of our steel rebar
$$
A_{v}= 3\times 0.11=0.33 \text{ in}^2
$$
we then have to calculate what our $S$ is, which is simply $S=6$, we are given this for this case 
then we use the equation to calculate $V_{sr}$
$$
V_{sr}=\frac{A_{v}\times fyt\times d}{S}
$$
$$
V_{sr}=\frac{0.33\times 60000\times 26}{6}=85800\frac{\text{lb}}{\text{ in}^2}
$$
$$
V_{usr}=0.75 \times 85800=64350 \frac{\text{lb }}{\text{in}^2}
$$
given all this we can finally calculate our $V_{u}$
$$
V_{n}=V_{c}+V_{sr} = 125265 \frac{\text{lb}}{\text{ in}^2}
$$
$$
V_{u}=\phi V_{n}=0.75\times 125265 = 93947.75 \frac{\text{lb }}{ \text{in}^2}
$$

now we have to check for our other $S$
$$
\begin{align} 
S_{max}=\frac{0.33\times 60000}{0.75\sqrt{ 4000 }\times 12}=34.78\text{"} \\
S_{max}=\frac{0.33\times 60000}{50\times 12}=33\text{"} \\
S_{max}=\frac{d}{2}=\frac{26}{2}=13\text{"}
\end{align}
$$
we used 6" for our $S$ so we are fine.

now we have to check for our $A_{v_{min}}$ 
$$
A_{v_{min}}=\frac{0.75\sqrt{ 4000 }\times 12 \times 6}{60000}=0.056 \text{ in}^2
$$
$$
A_{v_{min}}=\frac{50\times 12\times 6}{60000}=0.06\text{ in}^2
$$

for our minimum we choose the maximum, which is 0.06 square inches
In this case, our $A_{v}$ is larger than the minimum we're fine

for our maximum, we choose the minimum, which is 13 inches. 

Now we have to check, if the [^2]stirrup spacing needing to not more than $\frac{S_{max}}{2}$ is applicable or not 

$$
4\phi \sqrt{ f'c }\times b_{w}\times d < \phi V_{sr} < 8 \phi \sqrt{ f'c }\times b_{w}\times d
$$
$$
59197<64350<118395
$$
we are within the limits, so yes, the stirrup spacing must not be more than $\frac{S_{max}}{2}=\frac{13}{2}=6.5\text{ in}$
but we used 6 inches anyways so we're fine. 

[^2]: If our $\phi V_{sr}$ isn't within the bounds, we will have to redo the entire beam

---
Q13
in a simply supported beam of length $L$, if we have a uniform load $w_{v}$ across the beam, the supports will have a reaction force of $\frac{w_{v}L}{2}$
Q14
for a simply supported beam with a length L, and there is a moment $M_{v}$ (positive) on the right side. The left support will have a upward reaction of $\frac{M_{v}}{L}$ and the right support will have a downward reaction of $\frac{M_{v}}{L}$
Q15
If the beam has a positive moment on the left side, then right support will have a downward reaction of $\frac{M_{v}}{L}$ and the left side of the support will be upward reaction $\frac{M_{v}}{L}$
Q16
if we have a positive reaction on both sides, we just add the $M_{v}$ of bothn 
