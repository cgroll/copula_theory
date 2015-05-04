---
layout: default
title: Emerging copula
---

Conditional density: problem in three-dimensional vine

We can easily calculate:

$$c_{23 \vert 1}(u_{2},u_{3} \vert u_{1})$$

Hence, for each value $$ u_{1}$$, we can calculate the likelihood of
observing $$(u_{2},u_{3})$$. This way, we already know how several
value of $$ u_{1}$$ compare to each other in terms of likelihood: some
may be twice as likely as others. Still, we need to translate these
likelihoods into a probability measure, so that we need to normalize
the values:

$$\begin{aligned}
A&=\int_{0}^{1}c_{23 \vert 1}(u_{2},u_{3} ,\vert\ u_{1})\text{d}u_{1}\\
&=\int_{0}^{1}c_{23 \vert 1}(u_{2},u_{3} ,\vert\ u_{1})
	\overline{f}_{1}(u_{1})\text{d}u_{1}\\
&=\int_{0}^{1}c_{123}(u_{1},u_{2},u_{3})\text{d}u_{1}
\end{aligned}$$

Given $$A$$ we get:

$$\begin{aligned}
c_{1 \vert 23}(u_{1} \vert u_{2}, u_{3})&=
	\frac{c_{123}(u_{1},u_{2},u_{3})}{c_{23}(u_{2},u_{3})}\\
&=\frac{c_{123}(u_{1},u_{2},u_{3})}{A}\\
&=\frac{c_{23 \vert 1}(u_{2},u_{3} \vert u_{1}) \overline{f}_{1}(u_{1})}{A}
\end{aligned}$$


The density of the **emerging copula** can be derived by integration: 

$$\begin{aligned}
c_{23}(u_{2},u_{3})&= \int_{0}^{1}\overline{f}_{23|1}
\left(u_{2},u_{3},\vert\ u_{1}\right) \text{d}u_{1}\\
&=\int_{0}^{1}c_{23|1}
  	\left(\overline{F}_{2\vert 1}(u_{2}\vert u_{1}), \overline{F}_{3\vert 1}(u_{3}\vert
  	u_{1}), \vert\ u_{1}\right)
  	\ \overline{f}_{2\vert 1}(u_{2}\vert u_{1})
	\ \overline{f}_{3\vert 1}(u_{3}\vert
	u_{1}) \text{d}u_{1}\\
&=\int_{0}^{1}c_{23;1}
	\left(\overline{F}_{2\vert 1}(u_{2}\vert u_{1}),
	\overline{F}_{3\vert 1}(u_{3}\vert u_{1})\right)
	\ \overline{f}_{2\vert 1}(u_{2}\vert u_{1})
	\ \overline{f}_{3\vert 1}(u_{3}\vert
	u_{1}) \text{d}u_{1}\\
&=\int_{0}^{1}c_{23;1}
	\left(\overline{F}_{2\vert 1}(u_{2}\vert u_{1}),
\overline{F}_{3\vert 1}(u_{3}\vert u_{1})\right)
	\ c_{12}(u_{1},u_{2})
	\ c_{13}(u_{1},u_{3}) \text{d}u_{1}
\end{aligned}$$

Note:

- $$F_{2\vert 1}$$: distribution of $$X_{2\vert 1}$$ 
- $$\overline{F}_{2\vert 1}$$: distribution of $$U_{2\vert 1}$$

Conditional distributions can be hard to derive if they do not align
with the density decomposition that was used for the vine:

$$\begin{aligned}
\overline{f}_{1 \vert 23}(u_{1} \vert u_{2}, u_{3})&=
\frac{\overline{f}_{123}(u_{1},u_{2},u_{3})}
	{\overline{f}_{23}(u_{2},u_{3})}\\
	&=\frac{c_{123}(u_{1},u_{2},u_{3})}
	{c_{23}(u_{2},u_{3})}
\end{aligned}$$


Univariate Conditional distributions aligning with the chosen density
decomposition are easy to infer:

$$\begin{aligned}
f_{2 \vert 1}(x_{2}\vert x_{1})&=\frac{f_{12}(x_{1},x_{2})}{f_{1}(x_{1})}\\
&=\frac{c_{12}(F_{1}(x_{1}), F_{2}(x_{2}))
	f_{1}(x_{1})f_{2}(x_{2})}{f_{1}(x_{1})}\\
&=c_{12}(F_{1}(x_{1}), F_{2}(x_{2})) f_{2}(x_{2})
\end{aligned}$$

$$\begin{aligned}
f_{3 \vert 1}(x_{3}\vert x_{1})&=
c_{13}(F_{1}(x_{1}), F_{3}(x_{3})) f_{3}(x_{3})
\end{aligned}$$

$$\begin{aligned}
f_{3|12}(x_{3} \vert x_{1},x_{2})&=\frac{f_{23 \vert 1}(x_{2},x_{3} \vert x_{1})}
	{f_{2 \vert 1}(x_{2} \vert  x_{1})}\\
&=\frac{c_{23 \vert 1}(F_{2 \vert 1}(x_{2} \vert x_{1}), F_{3 \vert
1}(x_{3} \vert x_{1}))
	f_{2 \vert 1}(x_{2} \vert x_{1}) f_{3 \vert 1}(x_{3} \vert x_{1})}
	{f_{2 \vert 1}(x_{2} \vert  x_{1})}\\
&=c_{23 \vert 1}(F_{2 \vert 1}(x_{2} \vert x_{1}), F_{3 \vert
1}(x_{3} \vert x_{1}))
	 f_{3 \vert 1}(x_{3} \vert x_{1})
\end{aligned}$$

Conditional distributions follow a recursive structure:

$$\begin{aligned}
f_{i+1 \vert 1,...,i}(x_{i+1} \vert x_{1},\ldots,x_{i})
=&c_{i,i+1 \vert 1,\ldots,i-1}(u_{i \vert 1,\ldots,i-1},u_{i+1 \vert 1,\ldots,i-1} ,\vert\ x_{1},\ldots,x_{i-1})\\ 
&f_{i \vert 1,\ldots, i-1}(x_{i} \vert x_{1}, \ldots, x_{i-1})
\end{aligned}$$

Thereby, we define:

$$u_{i \vert 1,\ldots,i-1}:= F_{i \vert 1,\ldots,i-1}(x_{i} \vert x_{1},\ldots,x_{i-1})$$


## Emerging copula example: two-dimensional conditioning set

$$\begin{aligned}
c_{34}&=\int_{0}^{1}\int_{0}^{1}c_{1234}(u_{1},u_{2},u_{3},u_{4})
	\text{d}u_{1}\text{d}u_{2}\\
&=\int_{0}^{1}\int_{0}^{1} \overline{f}_{34 \vert 12}(u_{3},u_{4}
\vert u_{1},u_{2})
	c_{12}(u_{1},u_{2})
	\text{d}u_{1}\text{d}u_{2}\\
&=\int_{0}^{1}\int_{0}^{1} \overline{f}_{4 \vert 123}(u_{4} \vert
u_{1},u_{2},u_{3})
	\overline{f}_{3 \vert 12}(u_{3} \vert u_{1},u_{2})c_{12}(u_{1},u_{2})
	\text{d}u_{1}\text{d}u_{2}\\
&=\int_{0}^{1}\int_{0}^{1}c_{24}(u_{2},u_{4})
	\ c_{14;2}(u_{1 \vert 2}, u_{4 \vert 2})\ c_{34;12}(u_{3 \vert 12}, u_{4\vert 12}) c_{13}(u_{1}, u_{2})\
c_{23;1}(u_{2 \vert 1},u_{3 \vert  1})c_{12}(u_{1},u_{2})\text{d}u_{1}\text{d}u_{2}
\end{aligned}$$

because of


$$\begin{aligned}
f(x_{4} \vert x_{1},x_{2},x_{3})=&f(x_{4})\ c_{24}(F(x_{2}),F(x_{4}))
	\ c_{14;2}(F(x_{1} \vert x_{2}), F(x_{4} \vert x_{2}))\\
&\ c_{34;12}(F(x_{3} \vert x_{1}, x_{2}), F(x_{4} \vert x_{1},x_{2}))
\end{aligned}$$

$$\begin{aligned}
\overline{f}(u_{4} \vert u_{1},u_{2},u_{3})=&c_{24}(u_{2},u_{4})
	\ c_{14;2}(u_{1 \vert 2}, u_{4 \vert 2})\ c_{34;12}(u_{3 \vert 12}, u_{4\vert 12})
\end{aligned}$$

$$\begin{aligned}
f(x_{3} \vert  x_{1},x_{2})&=f(x_{3})\ c_{13}(F(x_{1}), F(x_{2}))\
c_{23;1}(F(x_{2} \vert x_{1}), F(x_{3} \vert  x_{1}))
\end{aligned}$$

$$\begin{aligned}
\overline{f}(u_{3} \vert  u_{1},u_{2})&=c_{13}(u_{1}, u_{2})\
c_{23;1}(u_{2 \vert 1},u_{3 \vert  1})
\end{aligned}$$
