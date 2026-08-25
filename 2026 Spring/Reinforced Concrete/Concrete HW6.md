![[Pasted image 20260322214157.png]]

--- 

In each of the examples, most variables are the same, except the rebar type. 
$d_{b}=1\text{ in (diameter)}$
$S_{c}=\frac{12-2(1.5)-2(0.375)-3(1)}{3-1}=3\text{ in}$
base - 2(cover) - 2(diameter leg) - number of rebar(diameter rebar) / number of rebar - 1


The maximum length of the rebar is 
Area of rebar is $3\#8 =3\cdot 0.79\text{ in}=2.37\text{ in}^2$
$\psi_{r}=\frac{2.12}{2.37}=0.8945$
$$
\text{Max}=
\begin{cases}
\geq \left( \frac{f_{y}\psi_{r}}{50\lambda \sqrt{ f'c }} \right)d_{b}=(\frac{60000\cdot0.8945}{50\cdot1\cdot\sqrt{4000}})\cdot 1\text{ in}=16.971\text{ in}\\
\geq0.0003f_{y}d_{b}=0.0003\cdot 60000 \cdot 1\text{ in}=18\text{ in}
\end{cases}
$$
use 16.971 inches as our max. 

There is more than 12 inches of fresh concrete below the casting position of the main rebar, $\psi_{t}=1.3$
There is no epoxy coating, so $\psi_{e}=1$
check $\psi_{t}\psi_{e}=1.3\cdot 1=1.3 \leq 1.7$ $\checkmark$
check Cover $> d_{b}$ , $1.5\text{ in}>1\text{ in } \checkmark$ 
check $S_{c}>d_{b}$ , $3\text{ in}>1\text{ in } \checkmark$

### Case 1: Straight Rebar

$$
\ell_d = \left( \frac{f_y \psi_t \psi_e}{20 \lambda \sqrt{f'_c}} \right) d_b=\left(\frac{60000\cdot1.3\cdot1}{20\cdot1\cdot\sqrt{4000}}\right)\cdot1=61.66 \text{ in}
$$
we now have to multiply by our $\ell_{d}$ modification, in this case, $\psi_{r}=\frac{2.12}{2.37}=0.8945$ 
$$
61.66 \text{ in} \times 0.8945 =\boxed{55.158\text{ in}}
$$
**NOT ACCEPTABLE**

### Case 2: Hooked Rebar

$$
\ell_{dh} = \left( \frac{f_y \psi_e \psi_c \psi_r}{50 \lambda \sqrt{f'_c}} \right) d_b
$$

for $\psi_{c}$, our rebar is indeed smaller than #11, and the cover on the hook tail is 2". Assuming the cover inside the column is greater than or equal to 2.5", 
for $\psi_{r}$ the spacing on the hook tail is 3". which is less or equal to  $3\cdot d_{b}=3\cdot 1\text{ in}$

following the table, $\begin{align} \psi_{e}=1 & &  \psi_{c}=0.7  &  & \psi_{r}=0.8 \end{align}$ 

$$
l_{dh}=\left(\frac{60000\cdot1\cdot0.7\cdot0.8}{50\cdot1\cdot\sqrt{4000}}\right)\cdot1=\boxed{10.62 \text{ in}}
$$
This is for a seismic design (we're in California, so we don't use a modification factor for $l_{dh}$)
check, $l_{dh}\geq 8d_{b}\text{ and 6 in?}$
$10.61\geq 8,6\text{ } \checkmark$
**Looks good!**
### Case 3: Headed Rebar

$$
\ell_{dt} = \left( \frac{0.016 f_y \psi_e}{\sqrt{f'_c}} \right) d_b
$$

There's no epoxy cover so $\psi_{e}=1$
checks, Bar is smaller than #11 $\checkmark$ 
$f_{y}$ is less than or equal to 60ksi $\checkmark$ 
There are clear covers that are 2" to the heads, they are not greater than than $2d_{b}$ $\times$
The clear spacing between bars is not greater than $4d_{b}=4\text{ in}$ or spacing between bars is $3\text{ in}$ $\times$

**We cannot use Headed Rebar.** 