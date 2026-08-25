![[Pasted image 20260223195801.png]]
1. Shear Diagram
 ![[Concrete HW4 Diagram]]
 The max shear in the problem will be at support B. 

2. Maximum shear at d from face of support
From face of the support $x=d$ and $d=25\text{ in}$. The equation for the shear is
converting units, $6 \frac{\text{ kip}}{\text{ft}}=0.5 \frac{\text{kip}}{\text{in}}$

![[Concrete HW4 Diagram 1-2|200]]

$$
\begin{align} \\
V_{u}+R_{u}-w_{u}\cdot x =0\\
-V_{u}=R_{u}-w_{u}\cdot x \\
V_{u}=64.5-0.5\cdot 25 = (-)52\text{ kip}
\end{align}

$$
this is the **required** shear, or the maximum shear

3. With stirrups #3, the total area of the rebar will be $0.11 \text{ in}^2\cdot 2=0.22\text{ in}^2$ , $A_{v}=0.22\text{ in}^2$
in short, find what $S$ would be.

Find what the provided shear ($V_{c}$)
$$
\begin{align}
V_{c}&=2\lambda \sqrt{ f'c }\cdot b_{w}\cdot d \\
V_{c}&=2\cdot 1 \sqrt{ 4000 \frac{\text{lb}}{\text{in}}} \cdot 10\text{ in}\cdot 25\text{ in} \cdot \frac{1\text{ kip}}{1000\text{ lb}}  = 31.62 \text{ kips}
\end{align}

$$
The provided shear by the concrete is only 31.62 kips, much lower than the required 52 kips, stirrups are indeed needed. The shear that needs to be provided by the stirrups is provide by rearranging
$$
\begin{align}
V_{u} &=\phi V_{c}+\phi V_{sr} \\
\phi{V_{sr}}&=V_{u}-\phi V_{c} \\
\phi V_{sr}&=52\text{ kip}-0.75\cdot 31.62\text{ kip} \\
\phi V_{sr}&=28.285 \text{ kip}
\end{align}


$$
in this case, always use $\phi=0.75$
Time to check our $\phi V_{sr}$
![[Pasted image 20260217171038.png]]
$$
4\phi \sqrt{ f'c }\cdot b_{w}\cdot d=4\cdot 0.75\sqrt{ 4000 \frac{\text{lb}}{\text{in}}} \cdot 10\text{ in}\cdot 25\text{ in} \cdot \frac{1\text{ kip}}{1000\text{ lb}}=47.43\text{ kips}
$$
Our $\phi V_{sr}<4\phi \sqrt{ f'c }\cdot b_{w}\cdot d$ 
so our stirrup spacings cannot be more than Smax, use Smax.

to find our required S, we use equation
$$
\begin{align}
\phi V_{sr}&=\frac{\phi Av \cdot fyt \cdot d}{S} \\
S&=\frac{\phi Av \cdot fyt \cdot d}{\phi V_{sr}} \\
S&=\frac{0.75\cdot 0.22\text{ in}^2 \cdot 60000 \frac{\text{lb}}{\text{in}^2} \cdot 25\text{ in}}{28285 \text{ lb} }=8.75\text{ in}
\end{align}
$$
**Our S spacing at maximum shear is 8.75 inches**

check our maximum $S$ 
![[Pasted image 20260217170827.png|400]]
$$
\begin{align} 
S_{max}&=\frac{0.22\times 60000}{0.75\sqrt{ 4000 }\times 10}=27.82\text{ in} \\
S_{max}&=\frac{0.22\times 60000}{50\times 10}=26.4\text{ in} \\
S_{max}&=\frac{d}{2}=\frac{25}{2}=12.5\text{ in}
\end{align}
$$
our $\frac{d}{2}$ is the lowest, so we use that one. Our calculated $S$ is 8.75 inches, lower than Smax, OK

Now to check our $A_{vmin}$

![[Pasted image 20260223211612.png]]

$$
\begin{align}
A_{vmin}&=\frac{0.75\cdot \sqrt{ 4000 } \cdot 10 \cdot 12.5}{60000}=0.0988\text{ in}^2 \\
A_{vmin}&=\frac{50 \cdot 10 \cdot 12.5}{60000}= 0.104\text{ in}^2
\end{align}
$$
our $A_{v}=0.22\text{ in}^2$ so we're OK

going back to our original equation,

$$
\begin{align}
\phi V_{sr}&=\frac{\phi Av \cdot fyt \cdot d}{S} \\
\phi V_{sr}&=\frac{0.75\cdot0.22\cdot60000\cdot 25}{12.5}= 19800\text{ lb}=19.8 \text{ kip}\\
\end{align}
$$
Using spacing of 12.5 inches.
$$
\begin{align}
V_{u}=\phi V_{c}+\phi V_{sr} \\
V_{u}=0.75\cdot31.62+19.8=43.515\text{ kip}
\end{align}

$$
4. at what distance from face of support at maximum shear side, shear would be at 15 kips.

to find x, we use equation
$$
\begin{align}
V_{u}+R_{u}-w_{u}\cdot x =0\\
15\text{ kip}+64.5\text{ kip}-6 \frac{\text{ kip}}{\text{ft}}\cdot x =0\\
x=13.25 \text{ ft}
\end{align}

$$
