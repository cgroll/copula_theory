---
layout: default
---

# Pair copula construction

Generally, any joint distribution can be decomposed into a product of
conditional distributions with increasing conditioning set:

$$\begin{aligned}
f(x_{1},\ldots,x_{n})&=f(x_{1})\cdot f(x_{2}|x_{1})\cdot \ldots \cdot f(x_{n}|x_{1},\ldots ,x_{n-1})
\end{aligned}$$

$$\begin{aligned}
f(x_{2}|x_{1})&=\frac{f(x_{1},x_{2})}{f(x_{1})}
\end{aligned}$$

Through Sklar's theorem, this can be written in terms of the
underlying copula: 

$$\begin{aligned}
f(x_{1},x_{2})&=c_{12}(F_{1}(x_{1}), F_{2}(x_{2}))f_{1}(x_{1})f_{2}(x_{2})
\end{aligned}$$

Hence, we get:

$$\begin{aligned}
f(x_{2}|x_{1})&=\frac{f(x_{1},x_{2})}{f(x_{1})}\\
&=\frac{c_{12}(F_{1}(x_{1}), F_{2}(x_{2}))f_{1}(x_{1})f_{2}(x_{2})}{f(x_{1})}\\
&=c_{12}(F_{1}(x_{1}), F_{2}(x_{2}))f_{2}(x_{2})
\end{aligned}$$


For a given two-dimensional distribution 

How do we get the individual conditional distributions?


References<a name="refs"></a>
---------

<iframe src="../refs/html_refs/pcc_intro.html" width="600" height="200"></iframe>

