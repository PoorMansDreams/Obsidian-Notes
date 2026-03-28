

Problem Example 2 Cantilever wall 

![[Problem 2 Xample Geowall|500]]

Using Rankine's method 
$$
K_{a}=\frac{1-\sin 33}{1+\sin 33}=0.295
$$
then we can find the lateral soil force
$$
\begin{align}
e_{1}=(200+100\cdot0)\cdot 0.295= 59\\
e_{2}=(200+100\cdot 21)\cdot 0.295=678.5
\end{align}
$$
Now we have to find ALL the forces (all are in $\text{lb/ft}$)
$$
\begin{align}
W_{1}=2'\cdot 19'\cdot 150= 5700\\
W_{2}=20'\cdot 2' \cdot 150 = 6000\\
W_{3}= 15' \cdot 19' \cdot 100 =  28500\\
W_{4} = 3' \cdot 2' \cdot 100 =  600\\ \\
Q_{LL}=200\cdot 15'= 3000 \\ \\
E_{a_{1}}=21\cdot e_{1} =1239\\
E_{a_{2}}=\frac{1}{2}\cdot 21 \cdot (e_{2}-e_{1})=6504.75
\end{align}
$$
for the "E" forces, it was split into 2 

for the moment arms for "O" or for **overturning**, we calculate the distances, which are 
$$
\begin{align}
W_{1}=4' (-) \\
W_{2}=10'(-) \\
W_{3}=12.5(-) \\
W_{4}=1.5(-) \\
Q_{LL}=12.5(-) \\
E_{a_{1}}=10.5(+) \\
E_{a_{2}}=7(+)
\end{align}
$$

(+) is counterclockwise, (-) is clockwise 

for the moment arms for "c" or for **overstressing**. we calculate the distances, which are
$$
\begin{align}
W_{1}=6' (-) \\
W_{2}=0' \\
W_{3}=2.5(-) \\
W_{4}=8.5(+) \\
Q_{LL}=2.5(-) \\
E_{a_{1}}=10.5(+) \\
E_{a_{2}}=7(+)
\end{align}
$$

Check for sliding...
$$
F.S.= \frac{(W_{1}+W_{2}+W_{3}+\cancel{W_{4}}+\cancel{Q_{LL}})\times \mu_{\text{base}}+\cancel{c'\times B}}{E_{a_{1}}+E_{a_{2}}}
$$
we don't include weight where the soil is on top of the beam (it could be excavated) treat it as a live load, and we don't include a **live load** that helps with the stability. Our cohesion is also zero. 

$$
F.S.=\frac{(5700+6000+28500)\times 0.5\text{ (given)}}{1239+6504.75}=2.595
$$

Check for Overturning...

$$
F.S.=\frac{W_{1}\cdot 4+W_{2}\cdot 10+ W_{3}\cdot 12.5 +\cancel{W_{4}\cdot 1.5 + Q_{LL} \cdot 12.5}}{E_{a_{1}}\cdot 10.5+E_{a_{2}}\cdot 7}
$$

$$
F.S.=\frac{5700(4)+6000(10)+28500(12.5)}{1239(10.5)+6504.75(7)}=7.5
$$

We don't include Weight 4 and QLL cause they are live loads that aid in stabilizing. Stabilizing (top) are clockwise, while overturning force (bottom) are counter clockwise 

Checking for overstressing...

$$
e=\frac{\Sigma M}{\Sigma N}=\frac{E_{a_{1}}\cdot 10.5+E_{a_{2}}\cdot 7 +W_{1}\cdot 6-W_{3}\cdot 2.5 +W_{4}\cdot 8.5-Q_{LL}\cdot 2.5}{W_{1}+W_{2}+W_{3}+W_{4}+Q_{LL}}
$$

$$
e=\frac{1239(10.5)+6504.75(7)+5700(6)-28500(2.5)+600(8.5)-3000(2.5)}{5700+6000+28500+600+3000}=0.435
$$

we include all the forces because in this case they all matter
now we have to check, 

$$
q_{\frac{max}{min}}=\frac{N}{B}\cdot \left( 1\pm \frac{6e}{B} \right) <q_{all}
$$
$$
q_{max}=\frac{5700+6000+28500+600+3000}{20'}\cdot(1+ \frac{6\cdot 0.435}{20'})=2475.795 \text{ lb/ft}^2 
$$

$$
2475.795 \text{ lb/ft}^2 <q_{all} =\text{5000 lb/ft}^2 \checkmark
$$


$$
B'=B-2e=q_{eq}<q_{all}
$$

$$
B'=20'-2(0.435)=19.13
$$
$$
q_{eq}=\frac{N}{B'}=\frac{5700+6000+28500+600+3000}{19.13}=2289.59 \frac{\text{lb}}{\text{ft}^2} 
$$
$$
q_{eq}>q_{all} \checkmark
$$

---

Global stability failure

![[Pasted image 20260326165914.png]]FS = 2.353 > 1.5 OK