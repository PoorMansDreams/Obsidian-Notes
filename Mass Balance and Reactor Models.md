#environmental 
Simple Mass Balance
$$
\text{Accumulation Rate}=\text{(Input Rate)-(Output Rate)+(Reaction Rate)}
$$

![[Pasted image 20251027145030.png]]
1.) If there is a Steady-State, conservative (Reaction=0)
$$
\begin{gather*}
C_s Q_s + C_w Q_w = C_m Q_m \quad \text{\small (usually {$C_m$} is unknown)} \\
{C_m} = \frac{C_s Q_s + C_w Q_w}{Q_m} = \frac{C_s Q_s + C_w Q_w}{Q_s + Q_w}
\end{gather*}
$$
$$
=\text{(Input Rate)-(Output Rate)}
$$
Batch Systems with nonconservative Pollutatants
There is no flow since the the operation requires the reactants to stay in one spot (like mixing slowly)
in this case,
$$
\text{(Accumulation Rate)=(Reaction Rate)}
$$
---
Zero-Order reaction rates, the reaction rate is independent o the concentration or the amount of substance present,

![[Pasted image 20251027145549.png]]

A First-Order reaction rate looks like this:
![[Pasted image 20251027150239.png]]

A Second-Order reaction rate looks like this: 
![[Pasted image 20251027150314.png]]
##### Exercise 5.A.2
a species is put in to a batch reactor, where it decays by either zeroth, first, or second reaction rate order. Derive equations for each order.
$$
\begin{align}
&r_{0}=-k  \\
&r_{1}=-kC \\
&r_{2}=-kC^2
\end{align}
$$
since this is a batch reactor, it is just accumulation rate = reaction rate 
for second order,
$$
\begin{gather}
&V \frac{dC}{dt}=-kC^2V \\
&\frac{dC}{C^2}=-k \text{ }dt \\
&\int_{C_{o}}^C \frac{dC}{C^2}=-k\int_{0}^t dt \\
&\left[ -\frac{1}{C} \right]^C_{C_{o}}=-kt \\
&C=\frac{C_{o}}{1+ktC_{o}} \\
\end{gather}
$$
---

##### Steady-State Systems with non conservative Pullutants
![[Pasted image 20251027152047.png]]
![[Pasted image 20251027152112.png]]

These systems are susceptible to shock loading, as they aren't prepared for it.
**Perfect Mixing** : Batch & CSTR, both are continuous operation, will have inflow and outflow.

The system is a continuous system with input and output plus reaction but doesn't have accumulation rate, so 0 accumulation.
$$
\begin{align}
\text{Zero-order, decay rate} = &-Vk \\
\text{Zero-order, generation rate} = &Vk \\
\text{First-order, decay rate} = & -VkC \\
\text{First-order, generation rate} = & VkC \\
\text{Second-order, decay rate} = & -VkC^2 \\
\text{Second-order, generation rate} = & VkC^2 \\
\end{align}
$$
![[Pasted image 20251027152547.png]]

##### Exercise 5.A.5 

For a steady-state efficiency of a CSTR (Continuously-stirred tank reactor) for zeroth, first, second order transformation. 

Accumulation = Input + Output - decay
the accumulation is 0, 
$r_{2}=-k_{2}C^2$
$\theta=\frac{V}{Q}$
$\frac{1}{\theta}=\frac{Q}{V}$
$$
\begin{align}
V \frac{dC}{dt}=&QC_{o}-QC-KC^2V \\
Q(C_{o}-C)=&KC^2V \\
\frac{Q(C_{o}-C)}{V}=&KC^2 \\
\frac{C_{o}-C}{\theta}=&KC^2 \\
K\theta C^2+C-C_{o}=&0 \\
C=&\frac{-1+\sqrt{ 1^2-4(K\theta)(-C_{o}) }}{2(K\theta)}
\end{align}
$$
##### Exercise 5.A.8
Two CSTR in series, a species undergoes first order decay with a rate of k.

a. what is the residence time in a CSTR is required to achieve 90% removal where C is the steady state outlet concentration for a fixed inlet concentration C$_o$
$$
\begin{align*}
C = \frac{C_0}{1 + k\theta} \quad \longrightarrow \quad \frac{C}{C_0} = \frac{1}{1 + k\theta} \quad &= \frac{1}{10}
\end{align*}
$$

to achieve $\frac{C}{C_{0}}=\frac{1}{10}$ the $k\theta$ must be 9, so then 
$$
\theta=\frac{9}{k}
$$
![[Pasted image 20251027154229.png]]

If it is in series, the residence time is just $\theta$ twice, so $2\theta$
![[Pasted image 20251027154325.png]]

