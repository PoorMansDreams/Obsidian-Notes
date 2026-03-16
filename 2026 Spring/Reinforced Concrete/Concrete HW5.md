![[Pasted image 20260316000529.png]]
To determine deflection, we need to find 
$$\Delta_{d+l}=\frac{7700\times 12^3}{E_{c}I_{e}}$$
We can find our $E_c$ easily, which is just $3.60\times 10^6\text{ psi}.$ 

But we have to find $I_{e}$ which means we will have to do integration. 
We will also have to find 
$$
M_{cr}=\frac{f_{r}I_{g}}{y_{t}}
$$
$$
f_{r}=7.5\lambda \sqrt{ f'c }=7.5(1)\sqrt{ 4000 }=474.34
$$
**Note**, there is two negative moments and one positive moment. (Fixed beam) use equation
$$
I_{e}=0.50I_{e}^++0.25(I_{e_{1}}^-+I_{e_{2}}^-)
$$
Moments are given, so we have to calculate $\bar{y}$ , $y_{t}$ , $I_{g}$

---

For middle , $M_{2}=170 \text{ kip-ft}$

**Uncracked section,** 
$$
\begin{align}


\bar{y}&=\frac{\frac{1}{2}bt_{f}^2+b_{w}(h-t_{f})\left( t_{f}+\frac{h-t_{f}}{2} \right)}{bt_{f}+b_{w}(h-t_{f})} & b&=30\text{"} & t_{f}&=5\text{"} &b_{w}&=12\text{"} & h=30\text{"} \\ 

\bar{y}&=\frac{\frac{1}{2}\left(30\right)\left(5\right)^{2}+12\left(30-5\right)\left(5+\frac{30-5}{2}\right)}{30\left(5\right)+12\left(30-5\right)} \\

\bar{y}&=12.5 \\
y_{t}&=h-\bar{y}=30-12.5=17.5\text{"}

\end{align}
$$
now we can calculate for $I_{g}^+$
$$
\begin{align}
I_{g}^+&=\sum I_{o}+\sum Ad^2 \\
I_{g}^+&=\frac{bt_{f}^3}{12}+\frac{b_{w}(h-t_{f})^3}{12}+bt_{f}\left( \bar{y}-\frac{t_{f}}{2} \right)^2+b_{w}(h-t_{f})\left( \frac{h-t_{f}}{2}+t_{f}-\bar{y} \right)^2 \\
I_{g}^+&=\frac{30\left(5\right)^{3}}{12}+\frac{12\left(30-5\right)^{3}}{12}+30\left(5\right)\left(12.5-\frac{5}{2}\right)^{2}+12\left(30-5\right)\left(\frac{30-5}{2}+5-12.5\right)^{2} \\
I_{g}^+&=38437.5\text{ in}^4
\end{align}

$$
Now we calculate $M_{cr}$
$$
M_{cr}^+=\frac{f_{r}I_{g}}{y_{t}}=\frac{474.34\times 38437.5}{17.5}=1041853.93\text{ lb-in}
$$
Effective Moment of inertia for **Positive Moment**

Now for **Cracked section**

for the **positive moment part**, (middle section), compression bar at middle section is 2#9's $A's=2\text{ in}^2$
we also have to find $As$ which is for the tension bar, in the middle there are 4#9's, $As=4\text{ in}^2$
and for $n=\frac{E_{s}}{E_{c}}=\frac{29\times 10^6}{3.6\times 10^6}=8.055$ 

$$
\begin{align}
\bar{y}&=\frac{b\bar{y}\left( \frac{\bar{y}}{2} \right)+nAsd+(n-1)A'sd'}{b\bar{y}+nAs+(n-1)A's} & b&=30\text{"} & n&=8.055 &As&=4 & A's&=2 &d=27.5  \\
\bar{y}&=9.12\text{"} &d'&=2.5
\end{align}
$$
This is assuming our $\bar{y}\leq t_{f}$ which it isn't so we'll have to use a different equation

$$

\bar{y} = \frac{\left[ \frac{b t_f^2}{2} + (\bar{y} - t_f) b_w \left( t_f + \frac{\bar{y} - t_f}{2} \right) + (n-1) A'_s d' + n A_s d \right]}{\left[ b t_f + b_w (\bar{y} - t_f) + n A_s + (n-1) A'_s \right]}

$$
using the same variables as before, $(t_{f}=5\text{"})$, 
$$
\bar{y}=6.53\text{" } | \text{ from the top of the T beam, located inside the web}
$$
calculating $I_{cr}^+$

$$
I_{cr}^+=\frac{bt_{f}^3}{12}+\frac{(\bar{y}-t_{f})^3b_{w}}{12}+bt_{f}\left( \bar{y}-\frac{t_{f}}{2} \right)^2+(\bar{y}-t_{f})b_{w}\left( \frac{\bar{y}-t_{f}}{2} \right)^2+(n-1)A's(\bar{y}-d')^2+nAs(d-\bar{y})^2
$$
$$
I_{cr}^+=17161\text{ in}^4
$$

$$
I_{e}^+=(\frac{M_{cr}^+}{M^+})^3I_{g}^++(1-(\frac{M_{cr}^+}{M^+})^3)I_{cr}^+\leq I_{g}^+
$$
$$
I_{e}^+=19995\text{ in}^4
$$

---


similarly, we can solve for the support sections, which will have have a negative moment.
for left side, $M_{1}=250\text{ kip-ft}$ and for right side $M_{2}=200\text{ kip-ft}$

we could use the same equation from last time, but since we're doing the NEGATIVE moment, we have to flip the cross section and ignore the flanges that would be in tension, so basically our new shape will be

the centroid is just going to be the center, so $\bar{y}=15\text{"}$ 
![[HW5 concrete|150]]

$$
\begin{align}
\bar{y}&=\frac{\frac{1}{2}bt_{f}^2+b_{w}(h-t_{f})\left( t_{f}+\frac{h-t_{f}}{2} \right)}{bt_{f}+b_{w}(h-t_{f})} & b&=12\text{"} & t_{f}&=0\text{"} &b_{w}&=12\text{"} & h=30\text{"} \\  \\
\bar{y}&=15\text{"}=y_{t}
\end{align}
$$
For the moment of inertia, we can also use the same equation, or just use
$$
I_{g}^-=\frac{bh^3}{12}+bh\times 0^2=27000\text{ in}^4
$$
d in the $I_{g}$ equation is the distance of the "segment" from $\bar{y}$ , since there's no distance from $\bar{y}$ it's just 0. 
Now we calculate $M_{cr}$
$$
M_{cr}^-=\frac{f_{r}I_{g}}{y_{t}}=\frac{474.34\times 27000}{15}=853812\text{ lb-in}
$$

for the **negative moment** part, compression bar at the **left** side is 2#11, 2#9, 2#9, so $A's=4\cdot 1+2\cdot 1.56=7.12\text{ in}^2$
**NOTE** in this case, our $b=b_{w}=12$
and the $As=2\text{ in}^2$, use the same equations, but this time the flange is 0, so $\bar{y}$ will always be bigger than $t_{f}$, we can use either equation $t_{f}$ 

$$
\bar{y} = \frac{\left[ \frac{b t_f^2}{2} + (\bar{y} - t_f) b_w \left( t_f + \frac{\bar{y} - t_f}{2} \right) + (n-1) A'_s d' + n A_s d \right]}{\left[ b t_f + b_w (\bar{y} - t_f) + n A_s + (n-1) A'_s \right]}=5.67\text{"}
$$

$$
\bar{y}=\frac{b\bar{y}\left( \frac{\bar{y}}{2} \right)+nAsd+(n-1)A'sd'}{b\bar{y}+nAs+(n-1)A's}=5.67\text{"}
$$

now for the $I_{cr_{1}}^-$ remember, $t_{f}=0$
$$
I_{cr_{1}}^-=\frac{bt_{f}^3}{12}+\frac{(\bar{y}-t_{f})^3b_{w}}{12}+bt_{f}\left( \bar{y}-\frac{t_{f}}{2} \right)^2+(\bar{y}-t_{f})b_{w}\left( \frac{\bar{y}-t_{f}}{2} \right)^2+(n-1)A's(\bar{y}-d')^2+nAs(d-\bar{y})^2
$$
$$
I_{cr_{1}^-}=8911.1\text{ in}^4
$$
now, find the $M_{cr}^-$
$$
M_{cr}^-=\frac{474.34\times 27000}{15}=853812
$$
now we try to find $I_{e_{1}}^-$ for the LEFT side
$$
I_{e_{1}}^-=(\frac{M_{cr}^-}{M_{1}^-})^3I_{g}^-+(1-(\frac{M_{cr}^-}{M_{1}^-})^3)I_{cr}^-\leq I_{g}^-
$$
$$
I_{e_{1}}^-=9328.1\text{ in}^4
$$
our $I_{e_{1}}^-$ must be less than or equal to our $I_{g}^-$ so we just use $I_{g}^-$

for the **negative moment** part, compression bar at the **right** side is 2#11, 2#9, 2#8, so $A's=2\cdot 1+2\cdot 1.56+2\cdot 0.79=6.7\text{ in}^2$
**NOTE** in this case, our $b=b_{w}=12$
and the $As=2\text{ in}^2$, use the same equations, but this time the flange is 0, so $\bar{y}$ will always be bigger than $t_{f}$, we can use either equation $t_{f}$ 

---

$$
\bar{y} = \frac{\left[ \frac{b t_f^2}{2} + (\bar{y} - t_f) b_w \left( t_f + \frac{\bar{y} - t_f}{2} \right) + (n-1) A'_s d' + n A_s d \right]}{\left[ b t_f + b_w (\bar{y} - t_f) + n A_s + (n-1) A'_s \right]}=5.74\text{"}
$$

$$
\bar{y}=\frac{b\bar{y}\left( \frac{\bar{y}}{2} \right)+nAsd+(n-1)A'sd'}{b\bar{y}+nAs+(n-1)A's}=5.74\text{"}
$$
so then, our $I_{cr_{2}}^-$ is 
$$
I_{cr_{2}}^-=8880.7\text{ in}^4
$$

now we try to find $I_{e_{2}}^-$ for the RIGHT side


$$
I_{e_{2}}^-=(\frac{M_{cr}^-}{M_{2}^-})^3I_{g}^-+(1-(\frac{M_{cr}^-}{M_{2}^-})^3)I_{cr}^-\leq I_{g}^-
$$

$$
I_{e_{2}}^-=9696.5\text{ in}^4
$$
our $I_{e_{2}}^-$ must be less than or equal to our $I_{g}^-$ so we just use $I_{g}^-$

---
Now we can finally calculate for $I_{e}$
$$
I_{e}=0.50I_{e}^++0.25(I_{e_{1}}^-+I_{e_{2}}^-)
$$
$$
I_{e}=0.50(19995)+0.25(27000+27000)=23497.5\text{ in}^4
$$
---
going back to our original equation

$$\Delta_{d+l}=\frac{7700\times (12\text{ in})^3}{3.60\times 10^3 \frac{\text{lb}}{\text{in}^2} \times 23497.5\text{ in}^4}=0.15729\text{ in}$$
now we need to separate the dead and live loads 
$\omega_{D}=1.65\text{ kip/ft}=19800\text{ lb/in}$
$\omega_{L}=3.3\text{ kip/ft}=39600\text{ lb/in}$

$$
\begin{align}
\Delta_{D}=\frac{\Delta_{D+L}\times \omega_{D}}{\omega_{D}+\omega_{L}}= \frac{0.15729\times19800}{19800+39600}= 0.05243\\
\Delta_{L}=\frac{\Delta_{D+L}\times \omega_{L}}{\omega_{D}+\omega_{L}}=\frac{0.15729\times 39600}{19800+39600}=0.10486
\end{align}
$$
calculate $\rho'$ for MIDSPAN
$$
\rho'=\frac{A's}{b_{w}d}=\frac{2\text{ in}^2}{12\text{ in}\cdot 27.5\text{ in}}=0.00606
$$
$$
\begin{align}
\lambda_{\Delta LT}=\frac{\xi}{1+50\rho'}=\frac{3}{1+50(0.00606)}=2.3 \\
\lambda_{\Delta D}=\frac{\xi}{1+50\rho'}=\frac{2}{1+50(0.00606)}=1.53  \\
\lambda_{\Delta ST}=1 \\
\end{align}
$$
Assuming that 80% is short term, and 20% is long term

$$
\Delta=\Delta_{D}\lambda_{D}+\Delta_{L_{ST}}\gamma_{L_{ST}}+\Delta_{L_{LT}}\gamma_{L_{LT}}
$$
$$
\Delta=0.05243\cdot 1.53+0.10486\cdot 2.3 \cdot 80\% +0.10486\cdot 1 \cdot 20\%=\boxed{0.29\text{ in}}
$$
