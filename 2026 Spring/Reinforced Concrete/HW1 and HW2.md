##### HW1 problem 1
![[Pasted image 20260129150638.png]]

4x #8 bars, As = 0.79 x 4 = 3.16 in^2

$$
a=\frac{3.16\times 60}{0.85\times 4 \times 12}=4.647\text{ in}
$$
Calculate for $\beta_{1}$
$$
\beta_{1}=0.85-0.05(\frac{4000\text{psi}-4000\text{psi}}{1000\text{psi}})=0.85
$$
Calculate for c, using $\beta_{1}$ and $a$
$$
c=\frac{a}{\beta_{1}}=\frac{4.647\text{ in}}{0.85}=5.467 \text{ in}
$$
There is only one layer of rebar in this problem, so $d=dt=20-2.5=17.5\text{ in}$
we can now use these values to find what $\phi$ is
$$
\begin{align}
\phi&=0.65+0.25\left( \frac{dt}{c}-\frac{5}{3} \right) \\
\phi&=0.65+0.25\left( \frac{17.5}{5.467}-\frac{5}{3} \right)=1.033
\end{align}

$$
$\phi$ must not be greater than 0.9, so we use 0.9 instead.
pmin and pmax?
$$
\begin{align}
p_{min}=\frac{3\sqrt{ 4000 }}{60000}=0.0032\\
p_{min_{2}}=\frac{200}{60000}=\boxed{0.0033} \\ \\
P_{max}=0.85(0.85)\left( \frac{4}{60} \right)\left( \frac{0.003}{(0.003+0.004)} \right)=\boxed{0.021}
\end{align}
$$
$$
\rho=\frac{4}{12\cdot 17.5}=0.019
$$
note that $p_{min_{2}}<\rho<p_{max}$ so it's all good.
Now we can calculate for the Mu, the ultimate loading
$$
M_{u}=\phi M_{n}=0.9 \times 3.16\times 60\left( 17.5-\frac{4.647}{2} \right)=2589.72\text{ in-kips}
$$
---
#### HW1 problem 2
![[Pasted image 20260209173755.png]]
$d=dt=20-2.5=17.5$"
given the parameters
$w_{D}=1.4 \frac{\text{kip}}{\text{ft}}$ and $w_{L}=2.2 \frac{\text{kip}}{\text{ft}}$
We use the load combination $1.2w_{D}+1.6w_{L}$
$$
1.2\times 1.4 + 1.6 \times 2.2= 5.2 \frac{\text{kip}}{\text{ft}}
$$
 $$w=5.2 \frac{\text{kip}}{\text{ft}}\times\frac{1000\text{ lb}}{1\text{ kip}}=5200 \frac{\text{lb}}{\text{ft}}$$
Beam is symmetrical, load is uniformly distributed through the entire beam

Reactions at the ends of the beam $\frac{wL}{2}$
shear at the center of the beam is 0
moment at the center of the beam $\frac{wL^2}{8}=\frac{5200\times15}{8}=146250 \text{ lb-ft}$
our $M_{u}=146250 \text{ lb-ft}=1755000\text{ lb-in}$

$$
a=d\left[ 1-\sqrt{ 1-\frac{4M_{u}}{1.7\phi f'c\times b\times d^2} } \right]
$$
Assume that $\phi=0.9$
$$
a=17.5\left[ 1-\sqrt{ 1-\frac{4(1755000)}{1.7(0.9) (4000)\times 10\times 17.5^2} } \right] = 3.66\text{ in}
$$

$$
A_{s}=0.85ab \frac{f'c}{fy}=0.85(3.66)(10) \frac{4}{60}=2.074\text{ in}^2
$$
$$
\beta_{1}=0.85-\frac{f'c-4000}{1000}\times 0.05 = 0.85
$$
$$
c=\frac{a}{\beta_{1}}=\frac{3.66}{0.85}=4.306 \text{ in}
$$
we can now calculate for $\epsilon_{t}$
$$
\epsilon_{t}=\epsilon_{s}=\epsilon_{u} \frac{d-c}{c}=0.003 \frac{17.5-4.306}{4.306}=0.00919
$$
calculate what $\phi$ would've been
$$
\phi=0.65+\frac{250(\epsilon _{t}-0.002)}{3}=0.65+\frac{250(0.00919-0.002)}{3}=1.24
$$
our calculated $\phi$ is greater than 0.9, no need to recalculate

we need a 2 #7 rebar, and 2 #6
$0.60\times 2+0.44\times 2=2.08\text{ in}^2$

$p_{\text{min}}=\frac{\sqrt{ f'c }}{fy}$ and $\frac{200}{fy}= \left[ 3\times\frac{\sqrt{ 4000 }}{60000} , \frac{200}{60000} \right ]$ =$[0.0032,\boxed{0.0033}]$
$p_{max}=\rho 0.004=0.85\times \beta_{1} \frac{f'c}{fy}\times \frac{\epsilon_{u}}{(\epsilon_{u}+0.004)} =0.85\times 0.85\times \frac{4}{60}\times \frac{0.003}{0.003+0.004}=0.0206$

$\rho=\frac{2.074}{10\times 17.5}=0.011$
$p_{\text{min}}<\rho<p_{\text{max}}$ **OK** 

---

#### HW2 problem 1
![[Pasted image 20260209233105.png]]

$d_{t}=h-2.5=23.5\text{"}$
$d_{t}=22\text{"}$
$A_{s}=3\times 1.27+3\times 1=6.81\text{ in}^2$
$A'_{s}=2\times1=2\text{ in}^2$

solve for $\beta_{1}$ 
$$
\begin{align}
\beta_{1}&=0.85-\frac{f'c-4000}{1000}\times 0.05 \\
\beta_{1}&=0.85-\frac{5000-4000}{1000}\times 0.05  \\
\beta_{1}&=0.8
\end{align}
$$
$p_{\text{max}}=0.85\times \beta_{1} \frac{f'c}{fy}\times \frac{\epsilon_{u}}{\epsilon_{u}+0.004}=0.85\times 0.8\times \frac{5}{60}\times \frac{0.003}{0.003+0.004}= 0.0243$
$\rho=\frac{A_{s}}{bd}=\frac{8.81}{12\times 22}=0.0334$
$\rho>p_{\text{max}}$ we need a compression bar

| Es    | Ey    | As   | A's |
| ----- | ----- | ---- | --- |
| 29000 | 0.002 | 6.81 | 2   |

| iteration | C (in) | Es       | E's      | fs  | f's      | Ts    | C's      | Cc       | P        |
| --------- | ------ | -------- | -------- | --- | -------- | ----- | -------- | -------- | -------- |
| 1         | 7      | 0.007071 | 0.001929 | 60  | 55.92857 | 408.6 | 103.3571 | 285.6    | -19.6429 |
| 2         | 8      | 0.005813 | 0.002063 | 60  | 59.8125  | 408.6 | 111.125  | 326.4    | 28.925   |
| 3         | 7.5    | 0.0064   | 0.002    | 60  | 60       | 408.6 | 107.5    | 306      | 4.9      |
| 4         | 7.3    | 0.006658 | 0.001973 | 60  | 57.20548 | 408.6 | 105.911  | 297.84   | -4.84904 |
| 5         | 7.4    | 0.006527 | 0.001986 | 60  | 57.60811 | 408.6 | 106.7162 | 301.92   | 0.036216 |
| 6         | 7.39   | 0.00654  | 0.001985 | 60  | 57.56834 | 408.6 | 106.6367 | 301.512  | -0.45133 |
| 7         | 7.399  | 0.006528 | 0.001986 | 60  | 57.60414 | 408.6 | 106.7083 | 301.8792 | -0.01253 |
Sample calculations
$$
Es=0.003\times \frac{23.5-7}{7}=0.007071
$$
$$
E's=0.003\times\frac{7-2.5}{7}=0.001929
$$
for $fs$ our $\epsilon_{s}>\epsilon_{y}$ so we just use $fs=fy$
for $f's$ $\epsilon_{s}<\epsilon_{y}$ so 
$$
f's=\epsilon'_{s}Es=0.001929\times29000=55.92
$$
$$
Ts=A_{s}\times fs=6.81\times 60=408.6
$$
$$
C's=A's(f's-0.85f'c)=2(55.92-0.85(5))=103.34
$$
$$
Cc=0.85f'c\times b \times \beta_{1}\times c=0.85\times 5\times 12\times 0.8\times 7=285.6
$$
$$
P=Cc+C's-T=285.6+103.34-408.6=-19.6
$$

P is negative, we must increase our C. 

after 7 iterations, the closest I could get to 0 was when 
$$
\boxed{C=7.399\text{ in}}
$$
after solving for pmax, our $\rho$ is less than our pmax so its ok

test our p again
$p_{max}=0.0298$
$$
p=\frac{A's}{bd}=\frac{2}{12\cdot 22}=0.00757 < p_{max} 
$$
our new $\phi$
$$
\phi= 0.65+0.25\left[ \left( \frac{1}{\frac{7.399}{23.5}} \right)-\frac{5}{3} \right]
=1.027$$
calculated phi is greater than 0.9, so we just use 0.9

$$
M_{n}=Cc\left( d-\beta_{1}\left( \frac{c}{2} \right) \right)+C's(d-d')
$$
$$
M_{n}=301.8792\left( 22-0.8\left( \frac{7.399}{2} \right) \right)+106.7083(22-2.5)=7828 \text{ kip-in}
$$
$$
M_{u}=M_{n}\theta=7828\cdot 0.9=7045 \text{ kips-in}
$$

