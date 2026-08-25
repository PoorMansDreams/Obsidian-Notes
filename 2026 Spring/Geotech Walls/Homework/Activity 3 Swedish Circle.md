1. 
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
