 #hydraulics

#### Problem 1

For the following system, continue the solution provided below for one new guess of HJ. (What is your updated guess for HJ given the calculated. Explain your reasons

![[Hydraulics HW4-1]]

##### First Iteration

Sample Calc for first iteration, guess $H_J=5170.1 \text{ ft}$ 

Head Losses:

| Resevoir | Head Loss (R1-HJ) | Flow Direction |
| -------- | ----------------- | -------------- |
| R1       | 5200-5170.1= 29.9 | Entering       |
| R2       | 5170.1-5170= 0.1  | Exiting        |
| R3       | 5170.1-5100= 70.1 | Exiting        |

| Pipe # | Resevoir Water Height | Pipe Diameter | Pipe Length | Pipe Roughess (e) |
| ------ | --------------------- | ------------- | ----------- | ----------------- |
| 1      | 5200 ft               | 3 ft          | 4000 ft     | 0.0004 ft         |
| 2      | 5170 ft               | 5 ft          | 2000 ft     | 0.0004 ft         |
| 3      | 5100 ft               | 4 ft          | 3000 ft     | 0.0004 ft         |
$v=0.0000108$ 
$T(^\circ F)=68$

for pipe 1
$$
\frac{e}{D}=\frac{0.0004}{3}=0.00013
$$
from moody, $f=0.0127$
$$
h_{L}=f \frac{L}{D} \frac{V^2}{2g}=0.0127 \frac{4000}{3} \frac{V^2}{2\times 32.2}=0.2629V^2
$$
$$
h_{L}=29.9=0.2629V^2
$$
$$
V=10.68
$$
$$
R_{N}=\frac{VD}{v}=\frac{10.68\times3}{0.0000108}=2.96\times10^6
$$
from moody, $f=0.0132$


$Q_{1}=A_{1}V_{1}=\frac{\pi}{4}\cdot3^2\times 10.68=75.49 \frac{\text{ ft}^3}{\text{s}}$
$Q_{2}=A_{2}V_{2}=\frac{\pi}{4}\cdot 5^2 \times 1.18=23.17 \frac{\text{ ft}^3}{\text{s}}$
$Q_{3}=A_{3}V_{3}=\frac{\pi}{4}\cdot4^2\times 22.42=281.74 \frac{\text{ ft}^3}{\text{s}}$

| Pipe # | e/D     | Turb. f | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​   | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------- | ---- | -------- | ----------------- | -------- | ---------- | ----------- |
| 1      | 0.00013 | 0.0127  | 1333 | 29.9     | 10.68             | 2.97E+06 | 0.0132     | 75.49       |
| 2      | 0.00008 | 0.0115  | 400  | 0.1      | 1.18              | 5.48E+05 | 0.0141     | 23.17       |
| 3      | 0.0001  | 0.012   | 750  | 70.1     | 22.42             | 8.30E+06 | 0.0123     | 281.74      |

Using Revised $f$

| Pipe # | e/D     | f*     | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​   | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------ | ---- | -------- | ----------------- | -------- | ---------- | ----------- |
| 1      | 0.00013 | 0.0132 | 1333 | 29.9     | 10.46             | 2.97E+06 | 0.0132     | 75.49       |
| 2      | 0.00008 | 0.0141 | 400  | 0.1      | 1.07              | 5.48E+05 | 0.0141     | 23.17       |
| 3      | 0.0001  | 0.0123 | 750  | 70.1     | 22.16             | 8.30E+06 | 0.0123     | 281.74      |
Check flow rate sum.
$$
\sum Q=Q_{1}-Q_{2}-Q_{3}=75.49-23.17-281.74=-229.42\frac{\text{ ft}^3}{\text{s}}
$$

Too much fluid exiting from the junction $(-Q)$, our new $H_{J}$ should be lower to increase head loss in pipe 1, decrease head loss in pipe 3 as well. 
Increasing head loss in pipe 1 will increase velocity in pipe 1, increasing flow rate. 
Decreasing head loss in pipe 3 will decreased velocity, decreasing flow rate. 

##### Second Iteration

New Guess: $H_J=5150 \text{ ft}$ 

| Resevoir | Head Loss (R1-HJ) | Flow Direction |
| -------- | ----------------- | -------------- |
| R1       | 5200-5150= 50     | Entering       |
| R2       | 5170-5150= 20     | Entering       |
| R3       | 5150-5100= 50     | Exiting        |
$$
h_{L}=f \frac{L}{D} \frac{V^2}{2g}=0.0127 \frac{4000}{3} \frac{V^2}{2\times 32.2}=0.2629V^2
$$
$$
h_{L}=50=0.2629V^2
$$
$$
V=13.79
$$
$$
R_{N}=\frac{VD}{v}=\frac{13.79\times3}{0.0000108}=3.83\times10^6
$$


| Pipe # | e/D     | Turb. f | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​  | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------- | ---- | -------- | ----------------- | ------- | ---------- | ----------- |
| 1      | 0.00013 | 0.0127  | 1333 | 50       | 13.79             | 3.83+06 | 0.0129     |             |
| 2      | 0.00008 | 0.0115  | 400  | 20       | 16.73             | 7.75+06 | 0.0118     |             |
| 3      | 0.0001  | 0.012   | 750  | 50       | 18.92             | 7.01+06 | 0.0122     |             |
revised $f$
$Q_{1}=A_{1}V_{1}=\frac{\pi}{4}\cdot3^2\times 13.68=96.73 \frac{\text{ ft}^3}{\text{s}}$
$Q_{2}=A_{2}V_{2}=\frac{\pi}{4}\cdot 5^2 \times 16.51=324.35 \frac{\text{ ft}^3}{\text{s}}$
$Q_{3}=A_{3}V_{3}=\frac{\pi}{4}\cdot4^2\times 18.75=235.74 \frac{\text{ ft}^3}{\text{s}}$

| Pipe # | e/D     | f*     | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​  | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------ | ---- | -------- | ----------------- | ------- | ---------- | ----------- |
| 1      | 0.00013 | 0.0129 | 1333 | 50       | 13.68             | 3.80+06 | 0.0129     | 96.73       |
| 2      | 0.00008 | 0.0118 | 400  | 20       | 16.52             | 7.64+06 | 0.0118     | 324.35      |
| 3      | 0.0001  | 0.0122 | 750  | 50       | 18.76             | 6.95+06 | 0.0122     | 235.74      |

Check flow rate sum.
$$
\sum Q=Q_{1}+Q_{2}-Q_{3}=96.73+324.35-235.74=185.34\frac{\text{ ft}^3}{\text{s}}
$$
positive flow rate sum indicates too much inflow, need more fluid to exit. Next $H_{J}$ should be higher, 

##### Third Iteration
$H_J=5160$

| Resevoir | Head Loss (R1-HJ) | Flow Direction |
| -------- | ----------------- | -------------- |
| R1       | 5200-5160= 40     | Entering       |
| R2       | 5170-5160= 10     | Entering       |
| R3       | 5160-5100= 60     | Exiting        |

| Pipe # | e/D     | Turb. f | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​  | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------- | ---- | -------- | ----------------- | ------- | ---------- | ----------- |
| 1      | 0.00013 | 0.0127  | 1333 | 40       | 12.33             | 3.8+06  | 0.013      |             |
| 2      | 0.00008 | 0.0115  | 400  | 10       | 11.83             | 7.64+06 | 0.0119     |             |
| 3      | 0.0001  | 0.012   | 750  | 60       | 20.72             | 6.95+06 | 0.0122     |             |
Revised $f$
$Q_{1}=A_{1}V_{1}=\frac{\pi}{4}\cdot3^2\times 12.19=86.18 \frac{\text{ ft}^3}{\text{s}}$
$Q_{2}=A_{2}V_{2}=\frac{\pi}{4}\cdot 5^2 \times 11.63=228.38 \frac{\text{ ft}^3}{\text{s}}$
$Q_{3}=A_{3}V_{3}=\frac{\pi}{4}\cdot4^2\times 20.54=258.23 \frac{\text{ ft}^3}{\text{s}}$

| Pipe # | e/D     | f*     | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​  | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------ | ---- | -------- | ----------------- | ------- | ---------- | ----------- |
| 1      | 0.00013 | 0.013  | 1333 | 40       | 12.19             | 3.38+06 | 0.013      | 86.18       |
| 2      | 0.00008 | 0.0119 | 400  | 10       | 11.63             | 7.75+06 | 0.0119     | 228.38      |
| 3      | 0.0001  | 0.0122 | 750  | 60       | 20.54             | 7.01+06 | 0.0122     | 258.23      |
Check flow rate sum.
$$
\sum Q=Q_{1}+Q_{2}-Q_{3}=86.18+228.38-258.23=56.33\frac{\text{ ft}^3}{\text{s}}
$$
positive flow rate sum indicates too much inflow, need more fluid to exit. Next $H_{J}$ should be a bit higher, we are approaching 0, so this value is much closer.
##### Last Iteration

![[Pasted image 20251012030839.png]]

from the graph, we can hopefully obtain a Q sum of zero at a height of $H_J=5163.54$

| Resevoir | Head Loss (R1-HJ) | Flow Direction |
| -------- | ----------------- | -------------- |
| R1       | 5200-5162.5=36.46 | Entering       |
| R2       | 5170-5162.5=6.46  | Entering       |
| R3       | 5162.5-5100=63.54 | Exiting        |

| Pipe # | e/D     | Turb. f | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​  | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------- | ---- | -------- | ----------------- | ------- | ---------- | ----------- |
| 1      | 0.00013 | 0.0127  | 1333 | 36.46    | 11.776            | 3.27+06 | 0.013      |             |
| 2      | 0.00008 | 0.0115  | 400  | 6.46     | 9.51              | 4.4+06  | 0.0119     |             |
| 3      | 0.0001  | 0.012   | 750  | 63.54    | 21.32             | 7.89+06 | 0.0122     |             |

| Pipe # | e/D     | Turb. f | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​  | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------- | ---- | -------- | ----------------- | ------- | ---------- | ----------- |
| 1      | 0.00013 | 0.013   | 1333 | 36.46    | 11.64             | 3.27+06 | 0.013      | 82.28       |
| 2      | 0.00008 | 0.0119  | 400  | 6.46     | 9.35              | 4.4+06  | 0.0119     | 183.56      |
| 3      | 0.0001  | 0.0122  | 750  | 63.54    | 21.15             | 7.89+06 | 0.0122     | 265.74      |

Check flow rate sum.
$$
\sum Q=Q_{1}+Q_{2}-Q_{3}=82.28+183.56-265.74=0.1\frac{\text{ ft}^3}{\text{s}}
$$
close enough! 

#### Problem 2
![[Hydraulics HW4-2]]

Inflow from $Q_a=1 \frac{\text{ m}^3}{\text{s}}$ , from a tank 355 meters high, $e=0.36 \text{ mm}$

Sample Calc for pipe AB
$V=\frac{Q}{A}$
$$
h_{f}=f \frac{L}{D} \frac{V^2}{2g}=[f \frac{L}{D} \frac{1}{2gA^2}]Q^2=
KQ^2$$
$\frac{e}{D}=\frac{0.00036}{0.4}=0.0009$
from moody, $f=0.0191$
$$
f \frac{L}{D} \frac{1}{2gA^2}=0.0191 \cdot \frac{300}{0.4}\cdot \frac{1}{2\cdot 9.81\cdot \left( \frac{\pi}{4}\cdot0.4^2 \right)^2}=46 \frac{\text{s}^2}{\text{m}^5}
$$

| Pipe | Q (m3/sec) | Length (m) | Diameter (m) | e/D    | f∗     | K (sec2/m5) |
| ---- | ---------- | ---------- | ------------ | ------ | ------ | ----------- |
| AB   | 0.45       | 300        | 0.4          | 0.0009 | 0.0191 | 46          |
| AC   | 0.55       | 300        | 0.45         | 0.0008 | 0.0186 | 25          |
| BD   | 0.5        | 400        | 0.4          | 0.0009 | 0.0191 | 62          |
| CE   | 0.5        | 400        | 0.4          | 0.0009 | 0.0191 | 62          |
| CB   | 0.05       | 300        | 0.2          | 0.0018 | 0.0228 | 1764        |
| ED   | 0.05       | 300        | 0.2          | 0.0018 | 0.0228 | 1764        |

##### First Iteration

| Loop | Pipe | Q    | K    | $h_{f}$ | $\frac{h_{f}}{Q}$ | New Q |
| ---- | ---- | ---- | ---- | ------- | ----------------- | ----- |
| 1 cw | AB   | 0.45 | 46   | 9.38    | 20.9              | 0.461 |
| 1 cc | AC   | 0.55 | 25   | 7.56    | 13.8              | 0.539 |
| 1 cc | CB   | 0.05 | 1764 | 4.41    | 88.2              | 0.039 |
Correction Factor
$$\Delta Q=\frac{\sum h_{fc}-\sum h_{fcc}}{2\left( \sum \frac{h_{fc}}{Q_{c}}-\sum \frac{h_{fcc}}{Q_{cc}} \right)}$$
$$
\Delta Q=\frac{9.38-7.56-4.41}{2(20.9+13.8+88.2)}=-0.0105
$$
negative $\Delta Q$ means that there's too much counter clockwise, we subtract from the counter clockwise $Q$ and add to the clockwise $Q$.

| Loop | Pipe | Q     | K    | $h_{f}$ | $\frac{h_{f}}{Q}$ | New Q |
| ---- | ---- | ----- | ---- | ------- | ----------------- | ----- |
| 2 cw | CB   | 0.039 | 1764 | 2.75    | 69.6              | 0.043 |
| 2 cw | BD   | 0.5   | 62   | 15.45   | 30.9              | 0.504 |
| 2 cc | CE   | 0.5   | 62   | 15.45   | 30.9              | 0.496 |
| 2 cc | ED   | 0.05  | 1764 | 4.41    | 88.2              | 0.046 |
$$
\Delta Q=\frac{2.75+15.45-15.45-4.41}{2(69.6+30.9+30.9+88.2)}=-0.0038
$$
once again, we add to the clockwise, while subtracting from the counter clockwise.


##### Second Iteration
| Loop | Pipe | Q     | K    | $h_{f}$ | $\frac{h_{f}}{Q}$ | New Q  |
| ---- | ---- | ----- | ---- | ------- | ----------------- | ------ |
| 1 cw | AB   | 0.461 | 46   | 9.77    | 21.206            | 0.464  |
| 1 cc | AC   | 0.539 | 25   | 7.26    | 13.475            | 0.542  |
| 1 cc | CB   | 0.043 | 1764 | 3.26    | 75.852            | 0.0396 |
Correction Factor
$$
\Delta Q=\frac{9.77-7.26-3.26}{2(21.206+13.475+75.852)}=-0.003
$$


| Loop | Pipe | Q      | K    | $h_{f}$ | $\frac{h_{f}}{Q}$ | New Q |
| ---- | ---- | ------ | ---- | ------- | ----------------- | ----- |
| 2 cw | CB   | 0.0396 | 1764 | 2.76    | 69.85             | 0.407 |
| 2 cw | BD   | 0.504  | 62   | 15.75   | 31.248            | 0.505 |
| 2 cc | CE   | 0.496  | 62   | 15.25   | 30.752            | 0.495 |
| 2 cc | ED   | 0.046  | 1764 | 3.73    | 81.144            | 0.045 |
$$
\Delta Q=\frac{2.76+15.75-15.25-3.73}{2(69.85+31.248+30.752+81.144)}=-0.001
$$

Pressure Calculations, $\gamma=9.81\text{ kN/m}$


$$
\frac{P_{A}}{\gamma}+z_{A}+\frac{V^2}{2g}=\frac{P_{B}}{\gamma}+z_{B}+\frac{V^2}{2g}-h_{f}
$$
$$
\frac{P_{B}}{\gamma}=z_{B}-z_{A}=39.5-h_{f}
$$

| Junction | Elevation (m) |     | $h_{f}$ (m) | Elevation Head (m) | Total Head (m) | Pressure (kPa) $H\times \gamma$ |
| -------- | ------------- | --- | ----------- | ------------------ | -------------- | ------------------------------- |
| A        | 355           |     |             |                    |                | 0                               |
| B        | 315.5         | AB  | 9.77        | 39.5               | 29.73          | 291.6                           |
| C        | 313.8         | AC  | 7.26        | 41.2               | 33.94          | 332.95                          |
| D        | 312.3         | ABD | 9.77+15.75  | 42.7               | 17.18          | 168.53                          |
| E        | 314.1         | ACE | 7.26+15.25  | 40.9               | 18.39          | 180.401                         |

Junction D does not reach the required 170 kPa minimum. 