---
layout: default
title: Gaussian copula
---

Gaussian copula 
===============

Parameter restrictions: \\(-1<\rho<1\\)

cdf [[Joe14]](#refs)
---

$$C(u_{1},u_{2})=\Phi_{2}\left( \Phi^{-1}(u_{1}), \Phi^{-1}(u_{2})\right),$$

where \\(\Phi_{2}\\) denotes the cdf of the 2-dimensional normal
distribution with correlation coefficient \\(\rho\\), and \\(\Phi\\)
denotes the cdf of the univariate standard normal distribution.

pdf
---

$$c(u_{1},u_{2})=\frac{\phi_{2}(\Phi^{-1}(u_{1}),
\Phi^{-1}(u_{2}))}{\phi(\Phi^{-1}(u_{1}))\phi(\Phi^{-1}(u_{2}))},$$

where \\(\phi_{2}\\) denotes the pdf of the 2-dimensional normal
distribution with correlation coefficient \\(\rho\\), and \\(\phi\\)
denotes the pdf of the univariate standard normal distribution.

References<a name="refs"></a>
----------
<iframe src="../refs/html_refs/gauss.html" width="600" height="200"></iframe>
