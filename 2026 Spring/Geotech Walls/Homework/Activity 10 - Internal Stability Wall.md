
Each $S_{v}$ is 8 inches, At a wall height of 20 feet, this will give us 30 "slices" or layers. 
The wall also uses geogrids, aka geosynthetics. We use the table that gives us $\frac{kr}{ka}$. $\phi_{r}=30$

$$
k_{r}=k_{a}\times \frac{k_{r}}{k_{a}}=\frac{1-\sin \phi}{1+\sin \phi}\times 1
$$

note, $\frac{k_{r}}{k_{a}}=1$ given from table. $k_{a}$ is the active lateral earth pressure coeff

After calculating the pressure from soil, $\sigma_{v}=\text{depth}\times \gamma$, we can calculate $\sigma_{n}$ , which is the horizontal stresses in the reinforced soil

$$
\sigma_{n}=k_{r}\times \sigma_{v}
$$

For $T_{max}$, which is how much tension the soil will put on to the reinforcements, we need to calculate for each slice.

$$
T_{max}=\sigma_{n}\times S_{v}
$$

For our $T_{r}$ we will use the equation, this is how much the reinforcement can **give** 

$$
T_{al} = \frac{T_{ult}}{RF} = \frac{T_{ult}}{RF_{CR} * RF_{D} * RF_{ID}}=\frac{4000}{2.5\cdot 1.3 \cdot 1.1}=1118.88 \frac{\text{lb}}{\text{ft}}=T_{r}
$$

F*, scaling factor is $0.8\tan(\phi_{r})=0.4618$ for geogrids (given), otherwise we'd use chart on slide #51

To find $P_{r}$ we need to find $L_{e}$ which means we'll need to find $L_{a}$

$$
L_{a}=\frac{H-Z}{\tan\left( 45+\frac{\phi_{r}}{2} \right)} 
$$

$$
L_{e}=L_{reinf}-La=L_{reinf}-\frac{H-Z}{\tan\left( 45+\frac{\phi_{r}}{2} \right)} 
$$

now finally calculate

$$
P_{r}=2\times L_{e}\times \sigma_{v} \times \alpha \times F*
$$
$\alpha$ is given, depends on reinforcement type. 

we need to do three checks, 

$T_{max}<T_{reinf}$
$T_{max}<P_{reinf}$
$T_{max}<T_{connection}$


NOTE, there is a $\frac{s_{v}}{2}$ top layer and bottom layer, (4 inches of top cap and bottom toe) 

![[Pasted image 20260413212931.png]]
Final Results: 
$$
S_{v}=8 \text{ in}
$$

$$
L_{reinf}=12\text{ft}
$$


When doing external wall calculations,

For sliding,
Wall Height should be 70% of the height, but could be higher to increase weight
Could also increase wall width, to increase weight 

can't change geogrids, but we can change the Sv of the geogrid (spacing)
