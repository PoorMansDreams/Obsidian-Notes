
| Quantity   | SI Unit (Metric) | Symbol | Base Units (kg, m, s) | US Customary / Imperial |
| :--------- | :--------------- | :----- | :-------------------- | :---------------------- |
| **Force**  | Newton           | N      | kg⋅m/s²               | pound-force (lbf)       |
| **Work**   | Joule            | J      | N⋅m = kg⋅m²/s²        | foot-pound (ft-lb)      |
| **Energy** | Joule            | J      | N⋅m = kg⋅m²/s²        | BTU / Calorie           |
| **Power**  | Watt             | W      | J/s=kg⋅m²/s³          | Horsepower (hp)         |
$$
1\text{ hp}=745.7 \text{ W}
$$

1. A small electrical motor produces 5 W
$$
5\text{ W}=5 \frac{\text{ Nm}}{s}=5 \frac{\text{ kg m}^2}{\text{s}^3}
$$
---

1. A damaged 1200-kg car is being towed by a truck. Neglecting the friction, air drag, and rolling resistance, determine the extra power required (a) for constant velocity on a level road, (b) for constant velocity of 50 km/h on a 30$^\circ$ (from horizontal) uphill road, and (c) to accelerate on a level road from stop to 90 km/h in 12s
	1. At a constant velocity, there is no "extra power" required, **0**
	2. At a constant velocity of 50 km/h at slope of  30$^\circ$ from horizontal
	$$
50 \frac{\text{km}}{\text{h}}\cdot \frac{1\text{ h}}{3600\text{ s}}\cdot \frac{1000\text{ m}}{1\text{ km}}=13.889 \frac{\text{m}}{s}
$$
	Equation for Force going up (fighting against Weight at an angle)
$$
F=m\cdot g\cdot \sin \theta=1200\text{ kg}\cdot 9.81 \frac{\text{m}}{s^2}\cdot \sin(30^\circ) = 5886 \text{ N}
$$
	Power equation
$$
P=F\cdot v=5886\text{ N}\cdot 13.889 \frac{\text{m}}{s}= 81750.6 \text{ W extra power}
$$
	3. Accelerate on a level road from 0 to 90km/h in 12s
$$
v_{f}=90\frac{\text{ km}}{\text{h}}=25 \frac{\text{m}}{s}
$$
Use $\Delta KE$ equation (energy)
$$
\begin{align}
\Delta KE=\frac{1}{2}mv^2_{f}-\frac{1}{2}mv_{i}^2 \\
\Delta KE=\frac{1}{2}\cdot 1200\text{ kg}\cdot \left (25 \frac{\text{m}}{s} \right )^2 -0 =375000 \text{ J} \\
\end{align}
$$
Power equation can also be 

$$P=\frac{\Delta KE}{\Delta T}=\frac{375000 \text{J}}{12\text{ s}-0\text{ s}}=31250\text{ W}$$

---


3. Water is pumped from a lower reservoir to a higher reservoir by a pump that provides 20 kW of shaft power. The free surface of the upper reservoir is 45 m higher than that of the lower reservoir. If the flow rate of water is measured to be $0.03 \frac{\text{m}^3}{s}$ determine mechanical power that is converted to thermal energy during this process due to frictional effects

Convert the flowrate to mass flow rate
$$
\dot{m}=\rho \cdot \dot{V}=1000 \frac{\text{kg}}{\text{m}^3}\cdot 0.03 \frac{\text{m}^3}{\text{s}}=30 \frac{\text{ kg}}{\text{s}}
$$
Find the power of the water if it flowed down the channel (this is another form of Power Eq, for water)
$$
\dot{W}_{u}=\dot{m} \cdot g \cdot \Delta z
$$
$$
\dot{W}_{u}=30 \frac{\text{ kg}}{s} \cdot 9.81 \frac{\text{ m}}{\text{s}^2}\cdot 45 \text{ m}= 13243.5\text{ W}
$$
now compare this with how much power the shaft has to use

$$
\frac{\dot{W}_{u}}{\dot{W}_{\text{pump}}}= \frac{13243.5\text{ W}}{20000 \text{ W}}=0.662 \text{ efficiency}
$$
in short, the difference in useful energy and how much the shaft powers
$$
20000\text{ W}-13243.5\text{ W}=6756.5 \text{ W loss} 
$$
---

4. A 75-hp (shaft output) motor that has an efficiency of 91.0 percent is worn out and is replaced by a high-efficiency 75-hp motor that has an efficiency of 95.4 percent. Determine the reduction in the heat gain of the room due to higher efficiency under full-load conditions. 

note that we don't have $\dot{W}_{in}$ so we cannot simply plug in 75 hp to it, we have to use


$$
\begin{align} 
\dot{Q}_{loss}&=\dot{W}_{in}-\dot{W}_{out}\\ \\

\eta&=\frac{\dot{W}_{out}}{\dot{W}_{in}} = \text{efficiency}\\ \\

\dot{W}_{in}&=\frac{\dot{W}_{out}}{\eta} \\
 \\
\dot{Q}_{loss}&=\frac{\dot{W}_{out}}{\eta}-\dot{W}_{out} \\
\dot{Q}_{loss}&=\dot{W}_{out}\left( \frac{1}{\eta}-1 \right)
\end{align}
$$


knowing this, we can finally calculate 
$$
\begin{align}
75\text{ hp}\cdot\left( \frac{1}{0.91} -1\right)=7.418 \text{ hp} \\
75\text{ hp}\cdot\left( \frac{1}{0.954} -1\right)=3.616 \text{ hp} \\
7.418\text{ hp} - 3.616 \text{ hp}= 3.8016 \text{ hp}
\end{align}

$$
$$
3.8016\text{ hp} \cdot \frac{745.7 \text{ W}}{1 \text{ hp}}=2842.49\text{ W}
$$

