
An offshore facility for producing gas is proposed for a site where the bottom is sloping about 14 percent to the south. A plan view of the site and a boring log from the vicinity are attached. Use infinite slope analysis to compute the factor of safety for undrained condition at depth 200 ft below mudline. Assume the ratio of underained shear strength to effective stress for this site to be 0.4. Assume average unit weight of 115 pcf.
![[Pasted image 20260205144849.png]]

We need to find factor of safety, so we use the submerged FS equation.
$$
\begin{align}
FS=\frac{c'}{\gamma' z\cos \beta \sin \beta}+\frac{\tan \phi'}{\tan \beta}
\end{align}
$$
The slope **is** **submerged**, and at a 14% slope, 
![[1.3 Activity inf slope]]
The slope is 200 feet below the mudlines, so $z=200$ feet
From the equation, our $\beta=7.969$
Our ratio of underained shear strength is calculated to be $\frac{S_{u}}{\sigma'}=0.4$
Note that $S_{u}=c'$
and our specific weight or unit weight is 115 pcf
However, our SUBMERGED unit weight will be (115-62.4) = $\gamma'= 52.6 \frac{\text{lb}}{\text{ft}^3}$ 
since it's mud we assume that $\phi$ is 0
now we need to find $S_{u}$
note that $\sigma'=D(\sigma-\gamma_{w})$ where D is depth, this is possible cause the soil is the same throughout the entire site
$$
S_{u}=0.4\times \sigma'=0.4(200\times(115-62.4))= 4208 \frac{\text{lb}}{\text{ft}^2}
$$
$$
FS=\frac{4208}{52.6\times 200 \times \cos (7.969)\sin(7.969)}+\frac{\tan(0)}{\tan(7.969)}=2.91
$$
Our factor of safety is 2.91