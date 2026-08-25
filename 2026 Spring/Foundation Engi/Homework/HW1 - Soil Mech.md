---

---
Andy Nguyen

--- 
1. A saturated clay has a water content of 23% and specific gravity of 2.62. Calculate the total
unit weight, dry unit weight, and void ratio 

$\omega =0.23$
G.S.$=2.62$ 
$\gamma=2.62\times 62.4 \frac{\text{lb}}{\text{ft}^3}=163.49\frac{\text{lb}}{\text{ft}^3}$
$S=100\%=1$
$\gamma_{\text{t}}=?$
$\gamma_{\text{d}}=?$
$e=?$
![[HW1-Soil Mech|700]]
Assume the Weight of the solids is 1, $W_{s}=1$ 
Since the weight of solids is just "1", we can say that for $\omega=\frac{W_{w}}{W_{w}}$
$\boxed{\omega =\frac{W_w}{1}=0.23=W_{w}}$
note that 
$$
\begin{align}
\gamma&=\frac{\text{weight}}{\text{volume}}\\
\gamma_{s}&=\frac{W_{s}}{V_{s}} \\
V_{s}&=\frac{W_{s}}{\gamma_{s}} \\
V_{s}&=\frac{1}{\text{G.S.}\times 62.4}
\end{align}
$$
For the volume of water,
$$
\frac{W_{w}}{\gamma_{w}}=V_{w}
$$
For the volume of void, $S=\frac{V_{w}}{V_{v}}$
$$
V_{v}=\frac{V_{w}}{S}=\frac{W_{w}}{\gamma_{w}\times S}=\frac{W_{w}}{62.4\times S}
$$

For the total volume, we just add the Volume of Voids with the Volume of solids, so
$$
V_{t}=V_{s}+V_{v}=\frac{1}{\text{G.S.}\times 62.4} + \frac{W_{w}}{62.4\times S}=\frac{1}{2.62\times 62.4}+\frac{0.23}{62.4\times 1}=0.0098\text{ ft}^3
$$
Calculate Void Ratio
$$
e=\frac{V_{v}}{V_{s}}=\frac{\frac{W_{w}}{62.4\times S}}{\frac{1}{\text{G.S.}\times 62.4}}=\frac{W_{w}\times\text{G.S.}}{S}=\frac{0.23\times2.62}{1}=\boxed{0.6026}
$$


Calculate $\gamma_{d}$
$$
\gamma_{d}=\frac{W_{s}}{V_{t}}=\frac{1\text{ lb}}{0.0098\text{ ft}^3}=\boxed{102.014 \frac{\text{lb}}{\text{ft}^3}}
$$
Calculate $\gamma_{t}$ or $\gamma_{b}$
$$
\gamma_{t}=\frac{W_{t}}{V_{t}}=\frac{W_{w}+W_{s}}{0.0098\text{ ft}^3}=\frac{0.23+1\text{ lb}}{0.0098\text{ ft}^3}=\boxed{125.51 \frac{\text{lb}}{\text{ft}^3}}
$$
---
2. Classify the following soils using the Unified Soil Classification System (USCS).

| Parameter                      | Soil A | Soil B | Soil C | Soil D | Soil E | Soil F |
|--------------------------------|--------|--------|--------|--------|--------|--------|
| % Passing #4 (4.75 mm)         | 27     | 82     | 70     | 100    | 100    | 100    |
| % Passing #200 (0.075 mm)      | 4      | 55     | 32     | 0      | 57     | 100    |
| Size at 10% Passing, D10​ (mm) | 1.1    | 0.005  | 0.001  | 0.16   | 0.006  | NA     |
| Size at 30% Passing, D30​ (mm) | 6.5    | 0.04   | 0.055  | 0.24   | 0.017  | NA     |
| Size at 60% Passing, D60​ (mm) | 29     | 0.085  | 1.5    | 0.3    | 0.106  | 0.003  |
| Liquid Limit, LL (%)           | 15     | 37     | 37     | -      | 42     | 63     |
| Plastic Limit, PL (%)          | 10     | 31     | 20     | NP     | 29     | 31     |
$$
\begin{align}  
 PI=LL-PL
\\
 \\

C_{u}&=\frac{D_{60}}{D_{10}} \\ \\

C_{c}&=\frac{{D^2}_{30}}{D_{60}\times D_{10}}
\end{align}


$$
For Soil A, P200 < 50%, Coarse grained 
(100-27) > (27-4), Gravel 
P200 < 5%, either GW or GP 
$C_{u}=\frac{29}{1.1}=26.36$
$C_{c}=\frac{6.5^2}{29 \times 1.1}=1.32$
==Soil A is GW==

For Soil B, P200>50%, Fine grained
LL-PL=6, LL=37
==Soil B is ML==

For Soil C, P200 < 50%, Coarse grained 
(100-70)<(70-32), Sand
P200 >12%, 
LL-PL=17, LL = 37
==Soil C is SC==

For Soil D, P200 < 50%, Coarse grained
(100-100)<(100-0), Sand
P200 < 5%, SW or SP
$C_{u}=\frac{0.3}{0.16}=1.875<6$
$C_{c}=\frac{0.24^2}{0.3\times 0.16}=1.2$
==Soil D is SP==

For Soil E, P200 > 50%, Coarse grained
(100-100)<100-57), Sand
P200>12%, SM or SC
LL-PL=PI=13, LL = 42
==Soil is SM==

For Soil F, P200 > 50%, Fine grained 
LL-PL=PI=32, LL=63
==Soil is CH==

---
3. Plot the total vertical stress, effective vertical stress, and pore water pressure versus depth for
the following soil profile. Ignore pore water pressures in the unsaturated zone.

![[HW1-Soil Mech 1.3|700]]

Solve Specific weight for the Clay, we're given $\omega$ so assume weight of soil is 1, $W_{s}=1$
$$
\gamma_{t}=\frac{W_{t}}{V_{t}}=\frac{W_{w}+W_{s}}{\frac{1}{\text{G.S.}\times 62.4} + \frac{W_{w}}{62.4\times S}}=\frac{0.25+1}{\frac{1}{2.7\times 62.4}+\frac{0.25}{62.4\times 0.65}}=103.31 \frac{\text{lb}}{\text{ft}^3}
$$
For the 10' of sand with S=70%, we can set $V_{s}=1\text{ ft}^3$
$$
\gamma_{s}=\gamma_{w}\times \text{G.S.}=\frac{W_{s}}{V_{s}}
$$
![[HW1-Soil Mech 1.3 1|700]]
$$
\gamma_{t}=\frac{W_{t}}{V_{t}}=\frac{V_{w}\gamma_{w}+\text{G.S.}\times V_{s}\gamma_{w}}{V_{s}\times e+1}=\frac{0.7\cdot 1\cdot 0.45\cdot 62.4+2.65\times 1\cdot 62.4}{1\cdot 0.45+1}=127.59\frac{\text{lb}}{\text{ft}^3}
$$
Similarly, for the 30' portion of sand, 
$$
\gamma_{t}=\frac{W_{t}}{V_{t}}=\frac{V_{w}\gamma_{w}+\text{G.S.}\times V_{s}\gamma_{w}}{V_{s}\times e+1}=\frac{1\cdot 1\cdot 0.45\cdot 62.4+2.65\times 1\cdot 62.4}{1\cdot 0.45+1}=133.41\frac{\text{lb}}{\text{ft}^3}
$$

$$
\sigma=103.31\cdot 15+127.59\cdot 10+133.41\cdot 30=6827.5 \text{ psf}
$$
$$
u=62.4\cdot 30=1872\text{ psf}
$$
$$
\sigma'=103.31\cdot 15+127.59\cdot 10+(133.41-62.4)\cdot 30=4955.85\text{ psf}
$$
