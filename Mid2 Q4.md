**Question 4**: Let $K_1, K_2$ be  two non-empty, compact, disjoint sets in $\mathbf{R}^K$. Prove that 
$$
\inf\{|x_1- x_2| , x_1 \in K_1, x_2 \in K_2\} > 0
$$
**Proof:**
Define $\alpha = \inf\{|x_1- x_2| , x_1 \in K_1, x_2 \in K_2\}$
Since $|x_1- x_2| \geq 0$, it is impossible for $\alpha <0$. 
Suppose $\alpha = 0$, then there exists sequences $\{x_n\} \subset K_1, \{y_n\} \subset K_2$, s.t. $|x_n- y_n| \to 0$
Since $K_1, K_2$ are compact, there exists $\{x_{n_k}\} \subset \{x_n\}$ and $\{x_{n_k}\} \to x \in K_1$. Likewise, there exists $\{y_{n_{k_l}}\} \subset \{y_{n_k}\}$ and $\{y_{n_{k_l}}\} \to y \in K_2$.

Thus we have  $\{x_{n_{k_l}}\} \to x \in K_1$,  $\{y_{n_{k_l}}\} \to y \in K_2$, and $|x_{n_{k_l}}- y_{n_{k_l}}| \to 0$

Hence we should have: 
$\forall \varepsilon > 0 ,\exists N_1 \in \mathbf{N}^+$, s.t. $\forall n>N_1 , |x_{n_{k_n}} - x| < \frac{\varepsilon}{2}$. 
$\forall \varepsilon > 0 ,\exists N_2 \in \mathbf{N}^+$, s.t. $\forall n>N_1 , |y_{n_{k_n}} - y| < \frac{\varepsilon}{2}$. 
Then take $N := \max(N_1,N_2)$, then $\forall n^*>N , |y_{n_{k_{n^*}}} - y| < \frac{\varepsilon}{2}, |x_{n_{k_{n^*}}} - x| < \frac{\varepsilon}{2}$.

Suppose $x \neq y$, then $|x-y|>0$
By  $|x_{n_{k_l}}- y_{n_{k_l}}| \to 0$, $\forall  0<\varepsilon < |x-y|$, we can find $M \in \mathbf{N}^+$ ,s.t. $\forall m>\max(M,N), |x_{n_{k_m}}- y_{n_{k_m}}| <\varepsilon< |x-y|$

By triangle inequality, $|x-y|-|x_{n_{k_m}}  - y_{n_{k_m}} | \leq |x_{n_{k_m}} - x -y_{n_{k_m}} + y| \leq |x_{n_{k_m}} - x|  + |y_{n_{k_m}} - y|  \leq \varepsilon \implies$ $|x_{n_{k_m}}  - y_{n_{k_m}} | \geq |x-y| - \varepsilon$ 

Take $\varepsilon = \frac{|x-y|}{3}$, then we should have both $|x_{n_{k_m}}- y_{n_{k_m}}| <\frac{|x-y|}{3}$ and  $|x_{n_{k_m}}- y_{n_{k_m}}| \geq \frac{2|x-y|}{3}$, which is impossible. 

Thus we have $x = y$, which means there are sequence $\{x_{n_{k_m}}\} \subset K_1$, $\{y_{n_{k_m}}\} \subset K_2$ , and they converge to the same value , denote as $\beta.$ Thus $\beta \in LP(K_1), \beta \in LP(K_2)$

Since  $K_1, K_2$ are disconnect, compact sets in $\mathbf{R}^K$, thus $K_1, K_2$, and $K_1 \cap K_2 = \emptyset \implies LP(K_1) \cap LP(K_2) = \emptyset$. While the deduction above shows that $\beta \in LP(K_1)\cap LP(K_2)$, contradicting with $LP(K_1) \cap LP(K_2) = \emptyset$.

Thus we have 
