#structural
In the diagram, detect zero force members and determine the forces in members **CD, JE, and JK**
![[Structural HW4]]

#### 1. Find Reaction forces

$$
\sum M_{A}=-60\cdot 4-60\cdot 8-75\cdot 12+Ey\cdot 16 -75\cdot 20-75\cdot 24=0
$$
$$
Ey=307.5\text{ kN}
$$
$$
\sum Fy=Ay+Ey-60-60-75-75-75=0
$$
$$
Ay=37.50
$$
#### 2. Remove Zero-Force members and Cut the beam (CD)


![[Structural HW4-2]]

after cutting,
![[Structural HW4-3]]
Using moment about point J, we can find $F_{CD}$
$$
\sum M_{J}=60\cdot 4+60\cdot 8-37.5\cdot 12+F_{CD}\cdot 6=0
$$
$$
\boxed{F_{CD}=-45 \text{kN (under compression)}}
$$
Keep in mind, knowing what $F_{CD}$ is, we can calculate what $F_{ED}$ is as well,

![[Structural HW4-4]]
$$
\sum F_{Dx}=-F_{CD}+F_{DE}=0
$$
$$
F_{DE}=45\text{kN (compression)}
$$

#### 3. Find JE 
![[Structural HW4-5]]
![[Structural HW4 5.1]]
$$
\tan(\theta)=\frac{5}{4}
$$
$$
\theta=\tan^{-1}\left( \frac{5}{4} \right)=51.34^\circ
$$
$$
F_{JEx}=F_{JE}\cos(51.34^\circ)
$$
$$
\sum M_{K}=-75\cdot 4-75\cdot 8+45\cdot 5-F_{JEx}\cdot  5=0
$$
$$
F_{JE}\cos(51.34^\circ)=135
$$
$$
\boxed{F_{JE}=216.104\text{ kN}}
$$
