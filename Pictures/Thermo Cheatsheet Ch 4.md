First, list assumptions; 
- Kinetic and potential energy is negligible
- Rigid tank, no boundary work needed 
To calculate heat transfer, need states 1 and 2
mass will be constant in both state 1 and 2, $m=2\text{ kg}$, and since total volume doesn't change, specific volume is constant as well.

State 1:
$T=80^\circ\text{C}=353.15\text{ K}$
$v=2.045\frac{\text {m}^3}{\text{kg}}$
State 2:
$T=94.15^\circ\text{C}=367.3\text{ K}$
$v=2.045\frac{\text {m}^3}{\text{kg}}$

we are given the saturated vapor's specific volume, so we can use that to calculate the temperature as well, using interpolation. (Using table A-4)
$$
\begin{align}
y - y_1 &= \frac{y_2 - y_1}{x_2 - x_1} (x - x_1) \\
y-95&=\frac{90-95}{2.3593-1.9808}\left(2.045-1.9808\right) \\
y&=94.15^\circ\text{C}
\end{align}
$$

using Table A-4, we can also interpolate internal energy $u$, follow the temperature, volume, and the corresponding internal energy in the same row

$$
\begin{align}
T&=95 & v_{1}&=1.9808 & u_{g_{1}}&=2500.1 \\
T&=94.15 & v&=2.045 & u_{g}&=? \\
T&=90 & v_{2}&=2.3593 & u_{g_{2}}&=2494.0 \\ \\
&y-2500.1=\frac{2494.0-2500.1}{90-95}\left(94.15-95\right) \\
&y=2499.063 \\
&u_{g}=2499.063 \frac{\text{kJ}}{\text{kg}}
\end{align}
$$
now, we have to find the internal energy in State 1, Since this is a rigid box, $v_{1}=v_{2}$, we can find $x$, note that the $v_{f}$ and $v_{fg}$ are from Table A-4, at $T=80^\circ\text{C}$
$$
\begin{align}
x_{1}&=\frac{v_{1}-v_{f}}{v_{fg}} \\
x_{1}&=\frac{2.045-0.001029}{3.4053-0.001029} \\
x_{1}&=0.6
\end{align}
$$
now that we know what the x is, we can calculate the $u_{g}$ of state 1, Table A-4 at $T=80^\circ\text{C}$
$$
\begin{align}
u_{g}&=u_{f}+xu_{fg} \\
u_{g}&=334.97+0.6(2146.6) \\
u_{g}&=1622.93 \frac{\text{kJ}}{\text{kg}}
\end{align}
$$
now we can use the evil equation, note this is a rigid tank, there's no energy going out
$$
\begin{align}
Q_{in}-W_{out}&=\Delta U \\
Q_{in}&=m(u_{2}-u_{1}) \\
Q_{in}&=2\text{ kg}(2499.063 \frac{\text{kJ}}{\text{kg}}-1622.93 \frac{\text{kJ}}{\text{kg}})=\boxed{1752.266\text{ kJ}}
\end{align}
$$


