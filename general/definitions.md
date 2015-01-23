---
layout: default
---

## General properties

<div class="theorem"> Let \(F\) be a continuous \(d\)-dimensional
distribution function with marginal distributions
\(F_{1},\ldots,F_{d}\). Then:

<ul>
<li>There exists a unique copula function \(C\) with 
$$\begin{equation}
F(x_{1},\ldots,x_{d})=C(F_{1}(x_{1},\ldots,x_{d}))
\end{equation}$$
for all \(x_{1},\ldots,x_{d}\in \mathbb{R}^{d}\).
</li>
</ul>
</div>


<div class="theorem" markdown="1">**[Sklar's theorem]**
Let $$F$$ be a continuous $$d$$-dimensional
distribution function with marginal distributions
$$F_{1},\ldots,F_{d}$$. Then:

- There exists a unique copula function $$C$$ with 
$$\begin{equation}
F(x_{1},\ldots,x_{d})=C(F_{1}(x_{1},\ldots,x_{d}))
\end{equation}$$
for all $$x_{1},\ldots,x_{d}\in \mathbb{R}^{d}$$.

</div>


Should be outsourced!

### H-volume


### Conditional probabilities



### Definition h- and v-functions

$$\begin{aligned}
h(u_{1},u_{2}):&=C(u_{1}|u_{2})\\
&=\mathbb{P}(U_{1}\leq u_{1}|U_{2}=u_{2})\\
&=\frac{\partial C(u_{1},u_{2})}{\partial u_{2}}\\
&=\partial_{2}C(u_{1},u_{2})
\end{aligned}$$


$$\begin{aligned}
v(u_{2},u_{1}):&=C(u_{2}|u_{1})\\
&=\mathbb{P}(U_{2}\leq u_{2}|U_{1}=u_{1})\\
&=\frac{\partial C(u_{1},u_{2})}{\partial u_{2}}\\
&=\partial_{1}C(u_{1},u_{2})
\end{aligned}$$
