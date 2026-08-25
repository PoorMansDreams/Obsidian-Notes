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
![[Pasted image 20260217170827.png|400]]
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
![[Pasted image 20260217171038.png]]

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

---

Design Required sheer reinforcements Example-1
![[Pasted image 20260217172624.png]]

Note that our required shear that was calculated was $V_{u}=94-9.4\text{ kip/ft}\times 1.83\text{ ft}=76.8\text{ kips}$
First, calculate $V_{c}$ , $\lambda$ is given to us already

$$
V_{c}=2\lambda \sqrt{ f'c } \cdot b_{w}\cdot d=2\cdot 1 \cdot \sqrt{ 4000 }\cdot 16 \cdot \frac{22}{1000}=44.525\text{ kips}
$$
note, dividing by 1000 to convert it back from lb to kips
$$
\phi V_{C}=0.75\cdot 44.525=33.4\text{ kips}
$$
our calculated $V_{u}$ is less than the $V_{u}$

calculate how much $V_{sr}$ is needed
$$
V_{u}=\phi V_{c} + \phi V_{sr}
$$
$$
\phi V_{sr}=V_{u}-\phi V_{c}
$$
$$
\phi V_{sr}=76.8-33.4=43.3 \text{ Kips}
$$
make sure to check $\phi V_{sr}<4\phi \sqrt{ f'c }\cdot b_{w}\cdot d=66.8\text{ kips}$
all is well

![[Pasted image 20260217173953.png]]

Now we can calculate what we need to obtain $\phi V_{sr}=43.4\text{ kips}$ 
$$
\phi V_{sr}=\frac{\phi A_{v}\cdot fyt \cdot d}{S}
$$
$$
S=\frac{\phi A_{v}\cdot fyt \cdot d}{\phi V_{sr}}=\frac{0.75\cdot 0.22\cdot 60000 \cdot 22}{43.4\cdot 1000}=5\text{ in}
$$

$A_{v}=0.22\text{ in}^2$ (2 legs, #3 rebar)
$$
A_{v}min=max =
\begin{cases}
\frac{0.75\sqrt{ f'c }\cdot b_{w} \cdot S}{fyt}&=0.14\text{ in}^2 \\
\frac{50\cdot b_{w}\cdot S}{fyt}&= 0.15\text{ in}^2
\end{cases}

$$
Our current $A_{v}$ is above the minimum so we're OK
$$
S_{max}=Min=
\begin{cases}
\frac{d}{2} &=\frac{22}{2}=11 \\
\frac{A_{v}\cdot fyt}{0.75 \cdot \sqrt{ f'c }\cdot b_{w}} &=17.4\\
24\text{ in}
\end{cases}
$$
our $S_{max}=11\text{"}$ this is OK

so now
$$
\phi V_{sr}=\frac{0.75\cdot 0.22 \cdot 60000 \cdot 22}{11}=19.8 \text{ kips}
$$

---
Q 17
$$
\begin{align}
R_{U}=94 \text{ kip}\\
w_{u}=9.4 \text{ kip} \\
\text{find distance such that } V_{u }=60 \text{ kips}
\end{align}
$$
$$
\begin{align}
R_{U}-w_{u}x-V_{u}=0\\
94-9.4x-60=0 \\
x=3.617\text{ ft}
\end{align}
$$
Q 18
Find all u (Face of support) to $S_{max}=11\text{"}$ (#3 @ 11")
remember, our $\phi=0.75$ and $\lambda=1$
$$
\begin{align}
V_{u}=\phi V_{n}=\phi V_{c}+\phi V_{sr} \\ \\
V_{c}=\frac{2\lambda \sqrt{ 4000 } \cdot 16 \cdot 22}{1000} =44.5 \text{ kips}\\ \\
V_{sr}=\frac{0.22\cdot 60\text{ kips} \cdot 22}{11}=26.4 \text{ kips}\\
V_{u}=0.75\cdot (44.5+26.4)= 53.17 \text{ kips}
\end{align}

$$

Q 19

find x if we use #3 at 9" 
Our $V_c$ will be the same 
Our $V_{sr}$ will not be the same
$$
V_{sr}=\frac{0.22\cdot 60\text{ kips} \cdot 22}{9}= \text{ 32.267 kips}
$$
$$
V_{u}=\phi(V_{sr}+V_{c})=0.75(32.267+44.5)=57.57 \text{ kips}
$$

$$
\begin{align}
R_{U}-w_{u}x-V_{u}=0 \\
94-9.4(x)-57.57=0 \\
x=3.87
\end{align}


$$
---
