As shown in the figure, water is contained in a piston-cylinder assembly at $0.15 \text{ MPa}$ and a quality of $20\%$, is heated until the piston hits the stops. At that point, the water is saturated vapor and the pressure is $0.4 \text{ MPa}$. Ignore the weight of the piston. Evaluate the changes in internal energy between State 2 and State 1, and State 3 to 2, in $\text{kJ/kg}$. (circle your answers) (20 points)

note that x is the ratio of vapor mass to total mass, 
x=0 is saturated liquid
x=1 is saturated vapor
![[ExamProb3|300]]
We need to calculate what $x_2$ is, (its not 1)

based on the graph, the volume at point 3, and point 2 are the **same**, using this knowledge,

$v_{2}=v_{3}$ , we also know x=1 for point 3.
$$
\begin{align}
v_{3}&=v_{f}+x_{3}(v_{fg}) \\
v_{2}&=v_{f}+x_{2}(v_{fg})
\end{align}

$$
point 3 has a pressure of 0.4 MPa, Use table A-5
$$
v_{3}=0.001084+1(0.46242-0.001084)=0.46242 \frac{\text{m}^3}{\text{kg}}
$$
assuming there's only 1 kg of water in the piston, $v_{3}=0.46242\text{ m}^3$

we know that $v_{2}=v_{3}$ , **NOTE** that for $v_{2}$ we are using pressure of 0.15 MPa
 $$
x_{2}=\frac{v_{2}-v_{f}}{v_{fg}}
$$
$$
x_{2}=\frac{0.46242-0.001053}{1.1594-0.001053}=0.3982 \approx 0.4
$$

State 1 (initially)
$p_{1}= 0.15\text{ MPa}$
$x_{1}=0.20$ (this means 20% is vapor by mass)

State 2 (piston hits the stops)
$p_{2}=0.15\text{ MPa}$
$x_{2}=0.4$

State 3 (piston already hits stops but is heated more)
$p_{3}=0.4\text{ MPa}$
$x_{3}=1$
since the water is saturated vapor now.

---

First, find the internal energy of state 1,
$$
y=y_{f}+xy_{fg}
$$
Using Table A-5, we can find the internal energy at the first since we are given the pressure and x.
$$
u_{1}=466.97+(0.2)(2052.3)= 877.43 \frac{\text{kJ}}{\text{kg}}
$$
Now we can calculate the internal energy at the 2nd state, which is when the piston stops. The pressure is constant. The energy going into the system is added to expand the fluid, the fluid is being turned into **STEAM**, only 40% of it has turned into steam at this point. 
$$
u_{2}=466.97+0.4(2052.3)=1287.89 \frac{\text{kJ}}{\text{kg}}
$$

The change in internal energy is 
$$
u_{2}-u_{1}=1287.89 \frac{\text{kJ}}{\text{kg}}-877.43 \frac{\text{kJ}}{\text{kg}}=410.46 \frac{\text{kJ}}{\text{kg}}
$$
Steam has more "energy" than normal water 

---

From state 3 to 2, we first find the internal energy at state 3

The volume doesn't change, but the pressure does. So we simply look at $u_{g}$ at saturated vapor at 400 kpa.
$$
u_{3}=u_{g@400\text{ kpa}}=2553.1 \frac{\text{kJ}}{\text{kg}}
$$
the difference is simply
$$
u_{3}-u_{2}=2553.1 \frac{\text{kJ}}{\text{kg}}-1287.89  \frac{\text{kJ}}{\text{kg}}= 1265.21 \frac{\text{kJ}}{\text{kg}}
$$
---
Determine volume of 1 kg of water pressurized to 60Mpa at 600 $^\circ$C 
What are the properties?
$m=1\text{ kg}$
$p=60\text{ MPa}=60000\text{ KPa}$
$T=600^\circ\text{C}=873.15\text{ K}$
The water is superheated.

a) using the steam table (superheated water)
$$
\begin{align}
\upsilon_{@\text{600}^\circ}=0.004833 \frac{\text{m}^3}{\text{kg}} \\
v=0.004833 \frac{\text{m}^3}{\text{kg}}\times 1\text{ kg}=0.004833\text{ m}^3
\end{align}

$$
b) Using the Ideal gas model
From Table A-1, gas constant for water is $R=0.4615 \frac{\text{kJ}}{\text{kg}\cdot\text{K}}$
$$
\begin{align}
Pv&=RT \\
v&=\frac{RT}{P} =\frac{0.4615\frac{\text{kJ}}{\text{kg}\cdot\text{K}}\times 873.15\text{ K}}{60000\text{ KPa}} =0.00671598\text{ m}^3\\
\end{align}
$$
Calculate error using ideal gas equation
$$
\%\text{error}=\frac{|v_{table}-v_{ideal}|}{v_{table}}=\frac{0.004833-0.00671598}{0.004833}=38.96 \%
$$

c) using the Real Gas model we need to use Z. the compressibility Factor.
$$
\begin{align}
Z=&\frac{v_{\text{actual}}}{v_{\text{IG}}}=\frac{0.004833\text{ m}^3}{0.00671598\text{ m}^3}=0.72 \\
v=&Z\times v_{\text{IG}}=0.72\times 0.00671598=0.00483551\text{ m}^3
\end{align}
$$
d) need to use the reduced pressure
$P_{R}=\frac{P}{P_{cr}}=\frac{60\text{ MPa}}{22.06\text{ MPa}}= 2.7198$
then calculate for the reduced Temp as well
$T_{R}=\frac{T}{T_{cr}}=\frac{873.15\text{ K}}{647.1\text{ K}}=1.34$
from table, Z=0.72, similar results to calculating **USE THE TABLE**
the steam occupies only about 72% of the volume that an ideal gas would occupy at the same temperature and pressure
so now, 
$$
\begin{align}
Pv&=ZRT \\
v_{RG}&=Z\left( \frac{RT}{P} \right)=0.72(\frac{0.4615\frac{\text{kJ}}{\text{kg}\cdot\text{K}}\times 873.15\text{ K}}{60000\text{ KPa}})=0.72(0.00671598\text{ m}^3)= 0.00483551\text{ m}^3
\end{align}
$$
$$
\%\text{error}=\frac{|v_{table}-v_{real}|}{v_{table}}=\frac{0.004833-0.00483551}{0.004833}= 0.0519 \%
$$
