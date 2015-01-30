---
layout: default
title: Asymmetric FGM copula
---

# Asymmetric FGM copula

cdf
---

Following (#refs): ask MALTE

$$C(u_{1},u_{2})=u_{1}u_{2} + a u_{1}u_{2}(1 - u_{1} - u_{2} -
u_{1}u_{2})u_{2}(1 - u_{1})$$ 


pdf
---



Wolfram
-------
### cdf:

u*v + a*u*v*(1 - u - v - u*v)*v*(1 - u )

### vfun:

v + a v^2 - 4 a u v^2 + 3 a u^2 v^2 - a v^3 + 3 a u^2 v^3

### hfun:

3 a u^3 v^2+2 a u^3 v-4 a u^2 v-3 a u v^2+2 a u v+u

### pdf:

1 + a v (2 - 8 u - 3 v + u^2 (6 + 9 v))
