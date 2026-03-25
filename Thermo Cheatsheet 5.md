interpolation formula
$$
y - y_1 = \frac{y_2 - y_1}{x_2 - x_1} (x - x_1)
$$

3-36 Steam enters a nozzle at 400C and 800 kPa with a velocity of 10 m/s, and leaves at 375C and 400 kPa while losing heat at a rate of 25 kW. For an inlet area of 800 cm^2 ()
determine the velocity and the volume flow rate of the steam at the nozzle exit.

Steady-flow process, potential energy change is negligible, no work interactions.
$\dot{E}_{in}-\dot{E}_{out}=\Delta \dot{E}_{\text{system}}$

for flows, $\dot{E}=\dot{m}\left( h_{1}+\frac{V_{1}^2}{2} \right)$
There is a $\dot{Q}$ flowing OUT of the system as the steam enters (heat is exiting) which is 25 kW

$$
\begin{align}
\dot{m}\left( h_{1}+\frac{V_{1}^2}{2} \right)=\dot{m}\left( h_{2}+\frac{V_{2}^2}{2} \right)+\dot{Q}_{out} \\
\text{or} \\
h_{1}+\frac{V_{1}^2}{2}=h_{2}+\frac{V_{2}^2}{2}+\frac{\dot{Q}_{out}}{\dot{m}}
\end{align}

$$
flow in = flow out + heat (going out)

Using table A-6,
in $\frac{\text{m}^3}{\text{kg}}$ and $\frac{\text{kJ}}{\text{kg}}$ respectively 
$\text{v}_{1}=0.38429$ , $h_{1}=3267.7$ 
$\text{v}_{2}=0.74334$ , $h_{1}=3221.8$ 

Flow rate formulas
$Q=\text{area}\times\text{velocity}$ 
$\dot{m}=Q\times\text{density}$ 
remember, $\text{density}=\frac{\text{mass}}{\text{volume}}$, so then $\text{density}=\frac{1}{\text{v}}=$ 1 over specific volume
$\dot{m}=Q\times \frac{1}{\text{v}}$ 
so then we have our equation, make sure it is in meter/seconds
$$
\dot{m}=Q\times \frac{1}{0.38429}=\text{area}\times\text{velocity}_{1}\times \frac{1}{0.38429}=0.08\text{ m}^2\times 10 \frac{\text{ m}}{\text{s}}\times \frac{1}{0.38429 \frac{\text{m}^3}{\text{kg}}}=2.082 \frac{\text{kg}}{\text{s}}
$$
now we can substitute to find what $V_2$ is
We need to convert the velocity into energy, which is the conversion 

$$
\frac{1\text{ kJ/kg}}{1000 \text{ m}^2/\text{s}^2}
$$
$$
3267.7+\frac{10^2}{2}\cdot\left( \frac{1}{1000} \right)=3221.8+\frac{V_{2}^2}{2}\cdot \left( \frac{1}{1000} \right)+\frac{25}{2.082}
$$

solving for $V_{2}$ we get $V_{2}=260 \frac{\text{m}}{\text{s}}$
now we can calculate the volumetric flow rate (Q) of the exiting steam

$\dot{m}=Q\times \frac{1}{\text{v}}$
$\dot{m}\times\text{v}=Q$ 
$$
2.082\times0.74334=1.547 \frac{\text{m}^3}{\text{s}}
$$

2x(9.81)x(15)= 294.30000000

sqrt(294.3)=