
---
## <p align="left"><center>Memorandum</center></p>


To: Dr. Amr M. Morsy

From: Andy Nguyen

Date: 5/4/2026

Subject: HW7 Cut Walls

---

Below contains calculations for a cantilever wall and soil nail reinforcement, both have Slide2 global stability checks. 
![[Signature.excalidraw]]


![[Pasted image 20260504154222.png]]

Find $K_{a}$ and $K_{p}$ 
$$
K_{a}=\frac{1-\sin 30}{1+\sin30}=\frac{1}{3}
$$
$$
K_{p}\times K_{a}=1
$$
$$
K_{p}=3
$$
Start by finding lateral earth pressure for 3 main points
units are in $\frac{\text{lb}}{\text{ft}^2}$
$$
\begin{align}
e_{1}=0 \\
e_{2}=(103\times 15')\times \frac{1}{3}=515 \\
e_{3}=-[515+103(u+x)(K_{a}-K_{p})]
\end{align}
$$

we are unable to calculate what u or x is, so we can't find what $e_{3}$ is, but we can instead find a point where the lateral earth pressure is 0, at $e_4$ the lateral earth pressure is net 0. (it is where the left and right side lateral earth pressure forces cancel eachother out)

$$
\begin{align}
e_{4}=515+\gamma u(K_{a}-K_{p}) \\
0=515+103\times u\left( \frac{1}{3} -3\right) \\
u=1.875'
\end{align}
$$

We can further simplify our $e_{3}$ equation knowing that the forces at $e_{4}$ is net zero.

$$
e_{3}=\gamma(K_{p}-K_{a})\times x
$$
$$
e_{3}=274.67x
$$

Now, we find all the forces from the 3 triangles, 

$$
\begin{align}
E_{1}=\frac{1}{2}e_{2}H=3862.5 \\
E_{2}=\frac{1}{2}e_{2}u=482.8125 \\
E_{e}=\frac{1}{2}e_{3}x=137.335x^2
\end{align}
$$

We can now calculate what the sum moment is, since this is a static structure we will set $\sum M=0$
The moment will be at around point "o" which is the bottom of the wall.
$$
0=E_{1}\left( \frac{15}{3} +u+x\right)+E_{2}\left( \frac{2}{3}u+x \right)+E_{3}\left( \frac{1}{3}x \right)
$$

Plug in our values, and we will see that $x=12'$

Knowing x, we can finally find how deep the wall will be (under the excavation line). We do 25% longer than the calculated $u+x$ value so, 

$$
D=1.25(x+u)=1.25(12+1.875)=17.34'
$$

But now we will need to find the maximum moment on the wall. Luckily, we know that the maximum moment will be a distance $l$ under the excavation line. This point $l$ will **always** be deeper than the $u$. 

To find $l$ we find the point where the shear is 0.

$$
\begin{align}
\sum F_{n}=E_{1}+E_{2}-E'_{3}=0 \\
E'_{3}=4345.3125 \frac{\text{lb}}{\text{ft}}
\end{align}
$$

**NOTE** $E'_3$ is just the force formed from the distance $l$

The equation for $E'_{3}$ is

$$
\begin{align}
E'_{3}=\frac{1}{2}e'_{3}\times l=\frac{1}{2}[\gamma(K_{p}-K_{a})\times l]\times l \\
E'_{3}=137.33l^2
\end{align}
$$
$$
4345.3125 \frac{\text{lb}}{\text{ft}}=137.33l^2
$$

$$
l=5.625'
$$

We then plug it into the MAX moment, which is at $M_l$

**NOTE** the $E'_{3}$ is negative because it goes clockwise (around point $l$)
$$
M_{max}=E_{1}\left( \frac{H}{3} +u+l\right)+E_{2}\left( \frac{2}{3}u+l \right)-E_{3}'\left( \frac{l}{3} \right)=43453.125\text{ ft-lb}
$$

![[Pasted image 20260423144532.png]]
![[Pasted image 20260504154404.png]]


---

![[Pasted image 20260504154246.png]]

![[Pasted image 20260504155545.png]]
![[Pasted image 20260504155503.png]]