## Joint and Conditional Distributions

### 2.3 Joint Distributions
when $X$ and $Y$ are discrete, **Joint Probability Density Function** $f_{X, Y} (x, y)$ is defined as below:
$$f_{X, Y} (x, y) = P(X = x, Y = y)$$


when continuous:  
$`P[(X, Y) \in A] = \iint _A f_{X, Y}(x, y)dxdy`$

--------
joint PDF satisfies:

(1) $f_{X, Y}(x, y) \geq 0$  
(2) $\sum\limits_{x}^{} \sum\limits_{y}^{}f_{X, Y}(x, y) = 1$ (when discrete), $\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}f_{X, Y}(x, y)dxdy = 1$

also, in a k-dimensional space $A \subset R^k$, the probability of $(X_1, X_2, ..., X_k) \in A$ is:
$`P[(X_1, X_2, ..., X_k) \in A] = \begin{cases}
\sum ... \sum\limits_{(x_1, ..., x_k)\in A} f(x_1, x_2, ..., x_k)\quad \text{(when discrete)} \\
\int ... \int_{A} f(x_1, x_2, ..., x_k)dx_1 dx_2 ... dx_k\quad \text{(when continuous)}
\end{cases}
`$

-------
### Thm 2.4
Joint Probability Distribution Function of random variables $X_1, X_2, ..., X_k$ is:  

$$F(x_1, x_2, ..., x_k) = P(X_1 \leq x_1, X_2 \leq x_2, ...,  X_k \leq x_k)$$

when random vector $X = (X_1, X_2, ..., X_k)$ is continuous,  

$$ f(x_1, x_2, ..., x_k) = \frac{\partial^k}{\partial x_1 ... \partial x_k} F(x_1, x_2, ..., x_k) $$

-------
#### **example 2.7**
joint PDF of two variables $X$, $Y$ are:

$$ F_{X, Y}(x, y) = xy (0<x<1, 0<y<1) $$  
calculate $f_{X, Y}(x, y)$ and $P(X^2 < Y)$.

-----
sol:  
$f_{X, Y}(x, y) = \frac{\partial^2}{\partial x \partial y}F_{x, y}(x, y) = 1$  

$P(X^2 < Y) = \int_{0}^{1} \int_{0}^{\sqrt{y}} f_{X, Y}(x, y) dxdy = \frac{2}{3}$

-----

### 2.3.2 Marginal Probability Density Function

for joint PDF $f_{X, Y}(x, y)$ of random variables $X$ and $Y$, marginal PDF refers to the PDF of each random variables, $f_{X}(x)$ and $f_{Y}(y)$.


### Thm 2.4
for joint PDF $f_{X, Y}(x, y)$ of random variables $X$ and $Y$, 
