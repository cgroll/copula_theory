---
layout: default
---

Welcome to my notes on copula theory.

[Parametric copulas](param_cops/index.html)
------------------------------------------

* [Gaussian copula](param_cops/Gaussian.html) documentation
* [Clayton copula](param_cops/Clayton.html) documentation
* [Gumbel copula](param_cops/Gumbel.html) documentation

[Copula modifications](cop_modifications/index.html)
--------------------

## General properties

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
