Horizontal: horizontal position of roadway point; plan view (arc)
Vertical: vertical elevation of roadway point: profile view. (parabola)

For Horizontal Alignment, the X axis is the path along the stations. The Y axis is how much it offsets from the station alignment, (left right)

for Vertical Alignments, the X axis is the path along the stations, the Y axis (technically Z) is how much is goes up/down/elevation 

![[Pasted image 20260917192542.png]]

- The Main influential factors
	- Economical consideration: earthwork
	- Grade Control
	- Safety: enough sight distance 

<center>Maximum Grades for Type of Highway and Terrain Conditions</center>

| **Type of Terrain** | **Freeways and Expressways** | **Rural Highways** | **Urban Highways** |
| ------------------- | ---------------------------- | ------------------ | ------------------ |
| **Level**           | 3%                           | 4%                 | 6%                 |
| **Rolling**         | 4%                           | 5%                 | 7%                 |
| **Mountainous**     | 6%                           | 7%                 | 9%                 |

#### Vertical Alignment Components
- Has two grade lines, 
	- +G - Going uphill
	- -G - Going downhill 
- We want curved lines (rounded top area) so we don't go flying
- Types of vertical curves
![[Pasted image 20260917194739.png]]
Parts of a vertical curve
![[Pasted image 20260917194927.png]]

$$
\begin{align*}
\text{PVI} &= \text{Point of vertical intersection } (1) &  \\
E_{\text{PI}} &= \text{Elevation of PVI } (2) \\
\text{PVC} &= \text{Point of vertical curvature } (1)  \\
E_{\text{PC}} &= \text{Elevation of PVC } (2)\\
\text{PVT} &= \text{Point of vertical tangency } (1) \\
E_{\text{PT}} &= \text{Elevation of PVT } (2) \\
G_1 &= \text{Grade of initial tangent in percent} \\
G_2 &= \text{Grade of final tangent in percent} \\
L &= \text{Length of vertical curve } (3) \\
A &= \text{Algebraic difference in grade between } G_1 \text{ and } G_2 \\
K &= \text{Vertical curve length coefficient as determined for stopping sight distance } (4) \\
x &= \text{Horizontal distance to point on curve, measured from PVC } (3) \\
E_x &= \text{Elevation of point on curve located at distance } x \text{ from PVC } (2) \\
x_m &= \text{Location of min/max point on curve, measured from PVC } (3) \\
E_m &= \text{Elevation of min/max point on curve at distance } x_m \text{ from PVC } (2) \\
e &= \text{External distance} = \text{middle ordinate} \\
y &= \text{Offset of curve from initial grade line}\\
m &= \text{ the max or min elevation will occur when the slope is equal to zero, rarely at } \frac{L}{2} 
\end{align*}

$$

A formula that describes the elevation from grade is
$$
E_{b}=E_{a}+|x_{b}-x_{a}|\times G
$$
![[Grade Ex]]

Where $E$ is the elevation, $x$ is the horizontal distance.

![[Pasted image 20260917195846.png]]

![[Pasted image 20260917200952.png]]

$$
\begin{align}
\text{PVC Sta} &= \text{PVI Sta} - \frac{L}{2} = 320 - 90 = 230 \Rightarrow \underline{\text{Sta } 2+30} \\[5pt]
\text{PVT Sta} &= \text{PVC Sta} + L = 230 + 180 = 410 \Rightarrow \underline{\text{Sta } 4+10}
\end{align}
$$

$$
\text{Elevations for the PVC and PVT are}
\begin{align}
E_{PVC} &= E_{PVI} - \left(\frac{G_1}{100}\right)\left(\frac{L}{2}\right) = 320.40 - 0.03(90) = \underline{317.70\text{ ft}} \\[5pt]
E_{PVT} &= E_{PVI} - \left(\frac{G_2}{100}\right)\left(\frac{L}{2}\right) = 319.500 - 0.02(45) = \underline{318.60\text{ ft}}
\end{align}

$$

$$
\text{Location of high point can be calculated as follows:}
\begin{align*}
x_m &= \left| \frac{G_1 \times L}{G_2 - G_1} \right| = \left| \frac{3.0 \times 180}{-2.0 - 3.0} \right| = 108.00\text{ ft} \\[5pt]
\text{High point Sta} &= \text{PVC Sta} + x_m = 230 + 108 = 338 \Rightarrow \underline{\text{Sta } 3+38}
\end{align*}
$$

$$
\text{Elevation of high point can be calculated as follows:}
\begin{align*}
E_x &= E_{PVC} + \left(\frac{G_1}{100}\right) x_m + \frac{(G_2 - G_1){x_m}^2}{200L} \\[5pt]
E_x &= 317.70 + \left(\frac{3}{100}\right)(108) + \frac{(-2.0 - 3.0)(108)^2}{200(180)} = \underline{319.32\text{ ft}}
\end{align*}
$$


