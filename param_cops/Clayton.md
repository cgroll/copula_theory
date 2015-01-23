---
layout: default
title: Clayton copula
---

Clayton 
=======

- Symmetric to main diagonal

cdf
---

Following [[ACFB]](#refs):

$$C(u_{1},u_{2})=\left( u_{1}^{-\theta} + u_{2}^{-\theta} -1
\right)^{-\frac{1}{\theta}},\\$$

$$0<\theta$$

h-function
----------

$$\begin{aligned}
h(u_{1},u_{2})&=\frac{\partial C(u_{1},u_{2})}{\partial u_{2}}\\
&=-\frac{1}{\theta}(-\theta)u_{2}^{-\theta-1}\left( u_{1}^{-\theta} +
u_{2}^{-\theta} -1 \right)^{-\frac{1}{\theta}-1} \\
&=u_{2}^{-\theta-1}\left( u_{1}^{-\theta} +
u_{2}^{-\theta} -1 \right)^{-\frac{1}{\theta}-1}
\end{aligned}$$

pdf
---

$$\begin{aligned}
c(u_{1},u_{2})&=\frac{\partial h(u_{1},u_{2})}{\partial u_{1}}\\
&=\frac{\partial \left(u_{2}^{-\theta-1}\left( u_{1}^{-\theta} +u_{2}^{-\theta} -1 \right)^{-\frac{1}{\theta}-1}\right)}{\partial u_{1}}\\
&=(-\theta)\left(-\frac{1}{\theta}-1\right)\left( u_{1}u_{2} \right)^{-\theta-1}\left( u_{1}^{-\theta} +
u_{2}^{-\theta} -1 \right)^{-\frac{1}{\theta}-2}\\
&=(1+\theta)(u_{1}u_{2})^{(-1-\theta)}\left(
u_{1}^{-\theta} + u_{2}^{-\theta} -1  \right)^{-\frac{1}{\theta} - 2}
\end{aligned}$$


v-function
----------

$$\begin{aligned}
v(u_{2},u_{1})&=h(u_{2}, u_{1})
\end{aligned}$$

inverse h-function
------------------

$$\begin{aligned}
h(y, u_{2})&=u_{1} &\Leftrightarrow\\
u_{2}^{-\theta-1}\left( y^{-\theta} + u_{2}^{-\theta} -1
\right)^{-\frac{1}{\theta}-1}&=u_{1} &\Leftrightarrow \\
\left( y^{-\theta} + u_{2}^{-\theta} -1\right)^{-\frac{1+\theta}{\theta}}&=u_{1}u_{2}^{\theta+1} &\Leftrightarrow  \\
\left( y^{-\theta} + u_{2}^{-\theta} -1 \right)&= \left( u_{1}u_{2}^{\theta+1}\right)^{-\frac{\theta}{1+\theta}}  &\Leftrightarrow \\
y^{-\theta} &= \left( u_{1}u_{2}^{\theta+1}\right)^{-\frac{\theta}{1+\theta}} - u_{2}^{-\theta} +1&\Leftrightarrow  \\
y &= \left( \left(u_{1}u_{2}^{\theta+1}\right)^{-\frac{\theta}{1+\theta}} -u_{2}^{-\theta} +1 \right)^{-\frac{1}{\theta}}&\Leftrightarrow  \\
h^{-1}(u_{1},u_{2}) &= \left( \left(u_{1}u_{2}^{\theta+1}\right)^{-\frac{\theta}{1+\theta}} -u_{2}^{-\theta} +1 \right)^{-\frac{1}{\theta}}
\end{aligned}$$

inverse v-function
------------------

$$v^{-1}(u_{2},u_{1})=h^{-1}(u_{2},u_{1})$$

References<a name="refs"></a>
----------

<iframe src="../refs/html_refs/clay.html" width="600" height="200"></iframe>

