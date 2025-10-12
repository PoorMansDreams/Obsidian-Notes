 29.90000000 29.90000000 29.90000000 29.90000000 29.90000000 29.90000000 #hydraulics

#### Problem 1

For the following system, continue the solution provided below for one new guess of HJ. (What is your updated guess for HJ given the calculated. Explain your reasons

![[Hydraulics HW4-1]]

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
Check flow rate sum.
$$
\sum Q=Q_{1}-Q_{2}-Q_{3}
$$
Using Revised $f$

| Pipe # | e/D     | f*     | L/D  | hf​ (ft) | Velocity (ft/sec) | $R_N$​   | Revised f∗ | Q (ft³/sec) |
| ------ | ------- | ------ | ---- | -------- | ----------------- | -------- | ---------- | ----------- |
| 1      | 0.00013 | 0.0132 | 1333 | 29.9     | 10.68             | 2.97E+06 | 0.0132     | 75.49       |
| 2      | 0.00008 | 0.0141 | 400  | 0.1      | 1.18              | 5.48E+05 | 0.0141     | 23.17       |
| 3      | 0.0001  | 0.0123 | 750  | 70.1     | 22.42             | 8.30E+06 | 0.0123     | 281.74      |
