## Problem 1 
![[Pasted image 20260210145756.png]]



![[Pasted image 20260210210203.png]]
Drawing done in AutoCAD

Solved for the angles at the toe and crown of the slope
$$
33+y=42+x
$$
$$
33+y+42+x+38=180^\circ
$$
$$
y=9+x
$$
$$
33+9+x+42+x+38=180^\circ
$$
$$
x=29, 42+29=71^\circ
$$
$$
y=38, 33+38=71^\circ
$$
Both angles at the toe and crown at $71^\circ$ 
Factor of safety equation is
$$
FS=\frac{clR}{\sum W_{i}x_{i}}
$$
 $\gamma=118.5\text{ pcf}$
 $c=S_{u}=820\text{ psf}$
 $R=29.8374$
from the drawing, It is calculated that 
$$
A_{t}=H\times x_{crest}\times \frac{1}{2}=13\times 10.9546\times \frac{1}{2 }=71.2049\text{ ft}^2
$$
$$
A_{s}=\frac{1}{2}R^2\theta_{\text{rad}}-\frac{1}{2}R^2\sin \theta=\frac{1}{2}\times 29.8374^2\times38^\circ\times \frac{\pi}{180}-\frac{1}{2}\times 29.8374\sin 38^\circ=21.1722\text{ ft}^2
$$
$$
\begin{align}
x_{t}=17.6322 \\
x_{s}=19.3258 \\
l=R\theta= 29.8374\times 38^\circ\times \frac{\pi}{180}=19.7889 \\
\end{align}
$$
$$
W_{t}=118.5 \frac{\text{ lb}}{\text{ ft}^3}\times 1\text{ ft}\times 71.2049\text{ ft}^2=8437.7806\text{ lb}
$$
$$
W_{s}=118.5 \frac{\text{ lb}}{\text{ ft}^3}\times 1\text{ ft}\times 21.1722\text{ ft}^2=2508.9057\text{ lb}
$$
note that the 1ft is the "thickness" of the soil (into the page)
$$
FS=\frac{clR}{\sum W_{i}x_{i}}=\frac{820 \frac{\text{ lb}}{\text{ft}^2}\times 19.7889\text{ ft}\times 29.8374\text{ ft}}{8437.7806\text{ lb}\times 17.6322 +2508.9057\text{ lb} \times 19.3258}=\boxed{2.45}
$$
---
## Problem 2

![[Pasted image 20260216230717.png]]
![[Pasted image 20260217021446.png]]
To account for the weight of the block on top of the slope, 
$$
410 \frac{\text{lb}}{\text{ft}^2}\times 12.5317\text{ ft}\times 1\text{ ft}=5137.997\text{ lb}
$$
sample calculations for the top clay layer
$$
A_{t_{1}}=H\times x_{crest}\times \frac{1}{2}=19.7\times 17.4317\times \frac{1}{2 }=171.7\text{ ft}^2
$$
$$
A_{t_{2}}=H\times \text{B}\times \frac{1}{2}=19.7\times 21.9013\times \frac{1}{2 }=215.0561\text{ ft}^2
$$
$$
A_{s}=\frac{1}{2}R^2\theta_{\text{rad}}-\frac{1}{2}R^2\sin \theta= \frac{1}{2}\times 33.5555^2\times 40^\circ\times \frac{\pi}{180^\circ}-\frac{1}{2}\times 33.5555^2\sin(40^\circ)=31.7692\text{ ft}^2
$$

Weight for each area
$$
W_{t_{1}}=118.5 \frac{\text{ lb}}{\text{ ft}^3}\times 1\text{ ft}\times 171.7\text{ ft}^2=20346.45\text{ lb}
$$
$$
W_{t_{2}}=118.5 \frac{\text{ lb}}{\text{ ft}^3}\times 1\text{ ft}\times 215.0561\text{ ft}^2=25484.14785\text{ lb}
$$
$$
W_{s}=118.5\frac{\text{ lb}}{\text{ ft}^3} \times 1 \text{ ft} \times 31.7692\text{ ft}^2=3764.6502\text{ lb}
$$

sample calculations for moment of top clay layer
$$
M_{t_{1}}=20346.45\text{ lb}\times 23.0692\text{ ft}=469376.3243 \text{ lb-ft}
$$
$$
M_{t_{2}}=25484.14785\text{ lb}\times 11.7486\text{ ft}=299403.0594 \text{ lb-ft}
$$
$$
M_{s}=3764.6502\text{ lb}\times 27.5710 \text{ ft}=103795.1707 \text{ lb-ft}
$$

"CLR" of the top clay layer
$$
c_{1}l_{1}R_{1}=820\frac{\text{lb}}{\text{ft}^2} \times 23.5809\times 33.5555=648840.4898
$$
Final calculation
$$
FS=\frac{\sum M_{R}}{\sum M_{D}}=\frac{\sum c_{i}l_{i}R}{\sum W_{i}x_{i}}= \\
$$
$$
\frac{820\frac{\text{lb}}{\text{ft}^2} \times 23.5809\times 33.5555+1230\frac{\text{lb}}{\text{ft}^2}\times 29.1279\times 33.5555}{5137.997\cdot 26.6342+20346.45\cdot 23.0692+25484.14785\cdot 11.7486+3764.6502\cdot 27.5710+39683.1627+54757.8201} \\
$$
$$
FS= 1.68
$$
---
## Problem 3 
Determine the factor of safety for the slope shown in the figure below, for the marked trial slip surface, using the method of slices. (HW3 problem 3)

Here is just an example what the drawing could look like 
![[Act3 Example|800]]
![[Pasted image 20260212223052.png]]
Drawing of the slope

Sample calculations
$$
\text{Area}=b\cdot h_{\text{avg}}=1.2612 \text{ ft}\times 0.7648 \text{ ft}= 0.965 \text{ft}^2
$$
$$
W=A\times \gamma_{\text{avg}}=0.965\text{ ft}^2\times 118.5 \frac{\text{lb}}{\text{ft}^3} =114.301\frac{\text{lb}}{\text{ft}}
$$
$$
Wx=114.301 \frac{\text{lb}}{\text{ft}}\times -20.818\text{ ft}=-2379.52 \frac{\text{lb-ft}}{\text{ft}}
$$
$$
l_{1}=\frac{b}{\cos \alpha}=\frac{1.2612}{\cos 50^\circ}=1.962\text{ ft}
$$
for slice 18,
$$
W\cos \alpha \tan \phi=4166.833\cos(58)\tan(12)=469.34 \frac{\text{lb}}{\text{ft}}
$$


| Slice | $b$    | $h_{\text{avg}}$ | Area     | $\gamma_{\text{avg}}$ | $W$      | x        | $\phi$ | $W\cos \alpha \tan \phi$ | $Wx$     |
| ----- | ------ | ---------------- | -------- | --------------------- | -------- | -------- | ------ | ------------------------ | -------- |
| 1     | 1.2612 | 0.7648           | 0.964566 | 118.5                 | 114.301  | -20.818  | 0      | 0                        | -2379.52 |
| 2     | 2.7757 | 2.8827           | 8.00151  | 118.5                 | 948.179  | -18.7995 | 0      | 0                        | -17825.3 |
| 3     | 2.7757 | 5.2624           | 14.60684 | 118.5                 | 1730.911 | -16.0238 | 0      | 0                        | -27735.8 |
| 4     | 2.7757 | 7.0723           | 19.63058 | 118.5                 | 2326.224 | -13.2481 | 0      | 0                        | -30818   |
| 5     | 2.7757 | 8.4407           | 23.42885 | 118.5                 | 2776.319 | -10.4723 | 0      | 0                        | -29074.4 |
| 6     | 2.7757 | 9.4392           | 26.20039 | 118.5                 | 3104.746 | -7.6966  | 0      | 0                        | -23896   |
| 7     | 2.7757 | 10.1102          | 28.06288 | 118.5                 | 3325.452 | -4.9209  | 0      | 0                        | -16364.2 |
| 8     | 3.533  | 10.5088          | 37.12759 | 118.5                 | 4399.619 | -1.7665  | 0      | 0                        | -7771.93 |
| 9     | 2.0184 | 10.5569          | 21.30805 | 118.5                 | 2525.004 | 1.0092   | 0      | 0                        | 2548.234 |
| 10    | 2.7757 | 10.1397          | 28.14477 | 118.5                 | 3335.155 | 3.4063   | 0      | 0                        | 11360.54 |
| 11    | 1.8058 | 9.9759           | 18.01448 | 118.5                 | 2134.716 | 5.6971   | 0      | 0                        | 12161.69 |
| 12    | 2.45   | 20.8595          | 51.10578 | 112                   | 5723.847 | 7.825    | 0      | 0                        | 44789.1  |
| 13    | 2.45   | 23.2833          | 57.04409 | 110                   | 6274.849 | 10.275   | 0      | 0                        | 64474.08 |
| 14    | 1.6214 | 24.0129          | 38.93452 | 109                   | 4243.862 | 12.3107  | 0      | 0                        | 52244.92 |
| 15    | 2.7757 | 22.7106          | 63.03781 | 108                   | 6808.084 | 14.5092  | 0      | 0                        | 98779.85 |
| 16    | 2.7757 | 20.6629          | 57.35401 | 107                   | 6136.879 | 17.285   | 0      | 0                        | 106076   |
| 17    | 2.7757 | 17.951           | 49.82659 | 106.7                 | 5316.497 | 20.0607  | 0      | 0                        | 106652.7 |
| 18    | 2.7757 | 14.1621          | 39.30974 | 106                   | 4166.833 | 22.8364  | 12     | 469.3429                 | 95155.45 |
| 19    | 2.7757 | 5.9621           | 16.549   | 106                   | 1754.194 | 25.6121  | 12     | 83.87648                 | 44928.59 |
The sum of $W\cos \alpha \tan \phi$ is 553.2194 lb/ft
The sum of $Wx$ is 483305.9 lb-ft/ft

$$
\sum M_{D}=\sum W_{i}x_{i}=483305.9 \frac{\text{lb-ft}}{\text{ft}}
$$
$$
\sum M_{R}=\left[ \sum c_{i}l_{i}+\sum W_{i}\cos \alpha_{i} \tan \phi_{i}  \right] R
$$

$$
\begin{align}

\sum M_{R}&= \left( 27\text{ ft}\times 1230\text{ psf} \times 105^\circ\times \frac{\pi}{180}+27\text{ ft} \times 615\text{ psf}\times 37^\circ \times \frac{\pi}{180}+553.2194 \right)\times 27  \\
\sum M_{R}&=1947693 \frac{\text{lb-ft}}{\text{ft}}
\end{align}
$$
finally, we can calculate our FS,
$$
\text{FS}=\frac{\sum M_{r}}{\sum M_{D}}= \frac{1947693  \frac{\text{lb-ft}}{\text{ft}}}{483305.9 \frac{\text{lb-ft}}{\text{ft}}}=4.03
$$
The slope is pretty strong

---


