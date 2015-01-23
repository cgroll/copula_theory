---
layout: default
title: Gumbel copula
---

Gumbel
======

- Symmetric to main diagonal

cdf
---

Following [[ACFB]](#refs):

$$C(u_{1},u_{2})=\exp\left(- \left((-\ln u_{1})^{\theta} + (-\ln
u_{2})^{\theta}\right)^{\frac{1}{\theta}}\right),\\$$

$$\theta\in [1,\infty)$$

h-function
----------

$$\begin{aligned}
h(u_{1},u_{2})&=\frac{\partial C(u_{1},u_{2})}{\partial u_{2}}\\
&=C(u_{1},u_{2})\left( -\frac{1}{\theta} \right)\left( (-\ln
u_{1})^{\theta}+(-\ln u_{2})^{\theta}
\right)^{\frac{1}{\theta}-1}\theta(-\ln u_{2})^{\theta-1}(-\frac{1}{u_{2}})\\
&=C(u_{1},u_{2})\frac{1}{u_{2}}(-\ln u_{2})^{\theta-1}\left( (-\ln
u_{1})^{\theta}+(-\ln u_{2})^{\theta}
\right)^{\frac{1}{\theta}-1}
\end{aligned}$$

pdf
---

$$\begin{aligned}
c(u_{1},u_{2})=&\frac{\partial h(u_{1},u_{2})}{\partial u_{1}} \\
=&C(u_{1},u_{2})\frac{1}{u_{1}}(-\ln u_{2})^{\theta-1}\left( (-\ln
u_{1})^{\theta}+(-\ln u_{2})^{\theta}\right)^{\frac{1}{\theta}-1} \\
&\cdot\frac{1}{u_{2}}(-\ln u_{2})^{\theta-1}\left( (-\ln
u_{1})^{\theta}+(-\ln u_{2})^{\theta}
\right)^{\frac{1}{\theta}-1}\\
&+C(u_{1},u_{2})\frac{1}{u_{2}}(-\ln u_{2})^{\theta-1}\left( \frac{1}{\theta}-1 \right) \left( (-\ln
u_{1})^{\theta}+(-\ln u_{2})^{\theta}
\right)^{\frac{1}{\theta}-2}\\
&\cdot \theta(-\ln u_{1})^{\theta-1}\left( -\frac{1}{u_{1}} \right) \\
=&C(u_{1},u_{2})(u_{1}u_{2})^{-1}\left( (-\ln u_{1})(-\ln u_{2})
\right)^{\theta-1}\\
&\cdot\left( \left( (-\ln u_{1})^{\theta}+(-\ln u_{2})^{\theta}
\right)^{\frac{1}{\theta}+\frac{1}{\theta}-2} - \left( \frac{1}{\theta}-1 \right)\theta \left( (-\ln
u_{1})^{\theta}+(-\ln u_{2})^{\theta}\right)^{\frac{1}{\theta}-2}\right) \\
=&C(u_{1},u_{2})(u_{1}u_{2})^{-1}\left( (-\ln u_{1})(-\ln u_{2})
\right)^{\theta-1}\left( (-\ln
u_{1})^{\theta}+(-\ln u_{2})^{\theta}\right)^{\frac{1}{\theta}-2}\\
&\cdot\left( \left( (-\ln u_{1})^{\theta}+(-\ln u_{2})^{\theta}
\right)^{\frac{1}{\theta}} + \theta - 1 \right)
\end{aligned}$$

v-function
----------

$$\begin{aligned}
v(u_{2},u_{1})&=h(u_{2}, u_{1})
\end{aligned}$$

inverse h-function
------------------

Not solveable.

inverse v-function
------------------

Not solveable.

$$v^{-1}(u_{2},u_{1})=h^{-1}(u_{2},u_{1})$$

References<a name="refs"></a>
----------

<iframe src="../refs/html_refs/gumb.html" width="600" height="200"></iframe>


