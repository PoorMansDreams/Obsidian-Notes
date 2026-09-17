Earthwork volumes can only be found with cross sections (has a depth) , profiles only provide elevation (a line)

#### End Areas Method (preliminary)
$$
V_{1}=d (\frac{A_{1}+A_{2}}{2})
$$


If there are multiples we can just sum of the volumes. $d$ is the length (across)

At station 0+600, the cross section area is 100m$^2$ of fill. At station 0+700, the area is 150m$^2$ of cut. The grade point is at station 0+635. What is the volume of cut and fill between stations 0+600 and 0+700.

Note that the station at 0+600, it is **fill**, and station 0+700, it is **cut**. The grade point is the point where there is no fill or cut. 

![[Cut-Fill Ex]]
For the sake of simplicity, we imagine the fill area to be perfectly rectangular 
$$
\begin{align}
V_{f}=100 \text{ m}^2\times 35\text{ m}=3500\text{ m}^3 \\ \\

V_{c}=150 \text{ m}^2\times 65\text{ m}=9750\text{ m}^3

\end{align}
$$

| Station  | Cut Area | Fill Area | L (m) |                   V cut                   |                  V fill                  |
| :------: | :------: | :-------: | :---: | :---------------------------------------: | :--------------------------------------: |
|  20+00   |    -     |  173.21   |       |                                           |                                          |
|          |          |           | 10.5  |                     0                     | $V_{f}=10.5\times\frac{173.21+43.56}{2}$ |
| 20+10.5  |    0     |   43.56   |       |                                           |                                          |
|          |          |           |  11   |     $V_{c}=11\times\frac{0+14.32}{2}$     |   $V_{f}=11\times\frac{43.56+9.63}{2}$   |
| 20+21.50 |  14.32   |   9.63    |       |                                           |                                          |
|          |          |           | 6.95  |  $V_{c}=6.95\times\frac{14.32+63.73}{2}$  |    $V_{f}=6.95\times\frac{9.63+0}{2}$    |
| 20+28.45 |  64.73   |     0     |       |                                           |                                          |
|          |          |           | 11.55 | $V_{c}=11.55\times\frac{63.73+187.42}{2}$ |                    0                     |
|  20+40   |  187.42  |     -     |       |                                           |                                          |
|          |          |           |       |                                           |                                          |

#### Prismoidal Formula
$$
\begin{align}
V=d\times \frac{A_{1}+4A_{m}+A_{2}}{6} \\
V=L\times \frac{A_{1}+4A_{m}+A_{2}}{3}
\end{align}

$$
L is the length from the midsection of d 
The area of $A_{m}$ is calculated through the averaging of the height $h_{1}-h_{2}$, $b_{1}-b_{2}$ etc. $A_{m}=\frac{A_{1}+A_{2}}{2}$

A limitation of this method is that we cannot use it when the number of sections is not odd. The number of sections **must** be odd. 

![[Pasted image 20260916180258.png]]

$$
\begin{align}
A_{1}=\frac{0.75+4.75}{2}\times 7 =19.25 \\
A_{2}=\frac{0.75+2.75}{2}\times 3 =5.25 \\
b_{m_{1}}=\frac{4.75+2.75}{2}=3.75 \\ 
b_{m_{2}}= \frac{0.75+0.75}{2}=0.75  \\
h_{m}= \frac{7+3}{2}=5\\ 
A_{m}=\frac{3.75+0.75}{2}\times 5=11.25 \\

V=17\times \frac{19.25+ 11.25+5.25}{6}= 26.375\\

\end{align}
$$

#### Volumes from Cross Sections
Easy to use, simply 
$$
V=\text{mean height}\times \text{plan area}
$$

![[Pasted image 20260916182348.png|473]]

The single/double/triple depth means how many areas that corner or depth touches, so for single depth, it would be 4.76, 8.10, 6.07, 1.98, and 3.55.

for double, it would be 5.14, 6.72, 3.21, 2.31

$$
V=\frac{765}{4}[(16.54+15.4+16.17+13.38)+2(16.32+17.25+15.55+15.84)+4(12.95)]=46513.9
$$