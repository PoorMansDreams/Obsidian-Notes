For structures of a column and beams, with a rebar going through them, the provided moment should always be greater than the applied moment. Moment capacity Required. 

Our calculated $M_{u_{1}}$ must be less than our provided $M_u$, generally thicker rebar will give a greater moment capacity. 

Basically, based on the moment graph, which is a U shape. We can adjust the size of rebar, since at certain parts at the beam, the moment is 0. We can save money by adjusting the amount of rebar needed.

The amount of rebar we "cut off" is simply called **Cut Off Point**, we will be calculating the cut off point. 

![[Pasted image 20260324171758.png]]

Based on theory we can find the cutoff point, but based on code, we have to extend the cutoff point from around $12d_{b}$ or $d$. The theoretical cutoff point is $x$. 

In short, find x, find $l_{d}$, find 
The true cutoff point (based on code) is 
$$
\text{max cutoff point}
\begin{cases}
x+\text{max}\begin{cases}
12 d_{b} \\
d
\end{cases} \\
l_{d}
\end{cases}
$$
whichever is further (larger) is the one we choose. 

in steps,
1. Find x, we will need to find $M_{u}$ to solve for x (using Moment calculation of a beam)
	1. $M_{u}^-$ for remaining ba's
	2. Find $As$ (compression bar)
	3. Find $a=\frac{Asf_{y}}{0.85f'c \cdot b}$
	4. Find $M_{b}=Asf_{y}\left( d-\frac{a}{2} \right)$, also find $\beta_{1}$
	5. Find $C=\frac{a}{\beta}\to \frac{c}{d_{t}}\to \phi$
2. Find the maximum cutoff point by using the equation above. 

![[Pasted image 20260324173114.png]]

There are some limits to having cutoff points, We need to have some conditions to meet if we want to apply this cutoff.

![[Pasted image 20260324173626.png]]


Example 4; Bar cutoff

![[Pasted image 20260324173723.png]]

The problem wants us to find the cutoff point for four #5 rebar
After the cutoff, there will be 3 #5 rebars remaining.

We will start off with the first steps, finding $M_{u}$ (provided moment) by the **REMAINING REBAR**  to find x.
$$
\begin{align}
As=3\times 0.31=0.93\text{ in}^2 \\
a=\frac{0.93\times 60}{0.85\times 4 \times 10}=1.64\text{ in} \\
\beta_{1}=0.85 \\
c=\frac{a}{\beta_{1}}=\frac{1.64}{0.85}=1.93 \text{ in} \\
d=17.5\text{ in} \\
\phi= 2.5 > 0.9, \phi =0.9 \\
M_{u}=\phi M_{n}=0.9\times \frac{0.93\times60\left( 17.5-\frac{1.64}{2} \right)}{12}=69.8\text{ ft-kip}
\end{align}
$$
Now we can calculate the **theoretical cutoff point**
using the beam, 

Resultant force on left side:  $R_{u_{1}}=$ 37.5 ft-kip
Uniform load: $\omega_{u}=5\text{ ft-kip}$
Moment applied: $M_{u_{1}}=93.45\text{ ft-kip}$

knowing this, we take moment at point $M_{b}$, this point is "x" distance

$$
\Sigma M_{b}= M_{u_{1}}-R_{u_{1}}\times x+\omega_{u}x\times \frac{x}{2}-M_{u}=0
$$
after calculating, we will get
$x_{1}=14.34'$ and $x_{2}=0.66'$
we will use $x_{2}$ because it is shorter. 
After calculating the $l_{d}$ and $MAX$ we find that $l_{d}=30.83$ while the $x+\text{max}$ will give us $25.42\text{ in}$ we use the safer option, (larger) so then our cutoff point will be
$$
\text{Cut Off}=31\text{ in}
$$

---

Quiz #28

$$
\begin{align}
\omega_{D}=1\text{ k/ft}  &  & b=11\text{ in}\\
\omega_{L}=2\text{ k/ft}  &  & dt=2.6\text{ in}\\
f'c =5\text{ ksi}  &  &  H=22\text{ in}\\
fy= 60\text{ ksi} &  & \text{Legs are \#4}
\end{align}
$$

there are 3 #9 rebar on the top of the beam, evenly spaced. 
Given that the $M_{u_{1}}=260\text{ ft-kip}$ and $R_{u_{1}}=57.2\text{ kip}$
adjust our loads, $1.2\omega_{d}+1.6\omega_{L}=4.4$

first, find x.
$$
\begin{align}
As=2\times 1=2\text{ in}^2 \\
a=\frac{2\times 60}{0.85\times 5 \times 11}=2.567\text{ in} \\
\beta_{1}=0.80 \\
c=\frac{a}{\beta_{1}}=\frac{2.567}{0.80}=3.208 \text{ in} \\
d=22-1.5(\text{cover})-\frac{1.128}{2}(\text{half rebar diam})-0.5(\text{stirrup diam})=19.436\text{ in} \\
\phi= 0.65+0.25\left( \frac{19.436}{3.208}-\frac{5}{3} \right)=1.747 > 0.9, \phi =0.9 \\
M_{u}=\phi M_{n}=0.9\times \frac{2\times60\left( 19.436-\frac{2.567}{2} \right)}{12}=163.37\text{ ft-kip}
\end{align}
$$
Calculate x using $M_{b}$

$$
\Sigma M_{b}= M_{u_{1}}-R_{u_{1}}\times x+\omega_{u}x\times \frac{x}{2}-M_{u}=0
$$
$$
\Sigma M_{b}= 260-57.2\times x+4.4x\times \frac{x}{2}-163.37=0
$$
$x=24.1, 1.81$
we choose 1.81 feet, which is 21.72 inches

our real cutoff will then be compared 
$$
\text{max cutoff point}
\begin{cases}
x+\text{max}\begin{cases}
12 d_{b} =12\times 1.128 =13.536\\
d= 19.36
\end{cases} \\
l_{d} = 
\end{cases}
$$




