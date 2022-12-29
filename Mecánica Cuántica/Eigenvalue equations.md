# Ladder operators

$L_{\pm} = L_x \pm i L_y$
## Properties
### $[\vec L^2, L_\pm]$ = 0
$$
	[\vec L^2,L_x \pm i L_y] = [\vec L^2, L_x] \pm i [\vec L^2, L_y] =0
$$

### $[L_+, L_-] = 2\hbar L_z$

$$
\begin{align}
	[L_+, L_-] &= \commu{(L_x + i L_y)}{(L_x - i L_y)} \\
		&= L_x^2 - iL_xL_y + iL_yL_x - i^2 L_y^2 \\
		&\qquad - L_x^2 - i L_xL_y + iL_yL_x + i^2L_y^2 \\
		&= 2i[L_y, L_x] \\
		&= -2i[L_x, L_y] \\
		&= -2i^2\hbar L_z \\
		&= 2\hbar L_z
\end{align}
$$
### $[L_z, L_\pm] = \pm \hbar L_\pm$
$$
\begin{align}
	[L_z,L_x \pm i L_y] &= [L_z, L_x] \pm i [L_z, L_y] \\
		&= i\hbar L_y \pm i^2\hbar (-1) L_x \\
		&= i\hbar L_y \pm \hbar L_x \\
		&= \hbar\paren{\pm L_x + i L_y}
\end{align}
$$
The two cases in the last line are
$$
\begin{cases}
	\begin{align}
		+L_x + iL_y &= L_+ \\
		-L_x + iL_y &= -L_-
	\end{align}
\end{cases}
$$
then $[L_z, L_\pm] = \pm\hbar L_\pm$ 


# Eigenvalue equations of $\vec L$ and $L_z$

[[CSCO]]
$$
\begin{align}
	\vec L^2 \ket{\alpha, \beta} &= \hbar^2\alpha\ket{\alpha, \beta} \\
	L_z \ket{\alpha, \beta} &= \hbar\beta\ket{\alpha, \beta}
\end{align}
$$
The state vector $L_\pm\ket{\alpha,\beta}$ is eigenvector of $\vec L^2$
$$
	\vec L^2 \paren{L_\pm\ket{\alpha,\beta}} =  \vec L^2 L_\pm\ket{\alpha,\beta} = \hbar^2\alpha\paren{\ket{\alpha,\beta}}
$$
The same state is eigenvector of $L_z$ but the eigenvalue changes
$$
\begin{align}
	L_z \paren{L_\pm\ket{\alpha,\beta}} &= \paren{L_\pm L_z + [L_z, L_\pm]}\ket{\alpha,\beta} \\
	&= \paren{L_\pm L_z + \hbar L_\pm}\ket{\alpha,\beta} \\
	&= L_\pm \paren{L_z + \hbar}\ket{\alpha,\beta} \\
	&= \hbar L_\pm (\beta\pm 1)\ket{\alpha,\beta} \\
	&= \hbar  (\beta\pm 1)L_\pm \ket{\alpha,\beta}
\end{align}
$$
This means when projecting the state $L_\pm\ket{\alpha,\beta}$ over $z$ component of $L_z$, the eigenvalue of the latter is raised (or lowered) by one unit $\hbar$.

# $\beta$ is bounded by $\alpha$
$$
\begin{align}
	\braket{\paren{\vec L^2 - L_z^2}}{\alpha,\beta} = \braket{\paren{L_x^2 + L_y^2}}{\alpha,\beta} &\geq 0	\\
	\then \hbar^2\paren{\alpha-\beta^2} \normbraket{\alpha,\beta} &\geq 0 \\
	\hbar\paren{\alpha - \beta^2} &\geq 0 \\
	 \alpha &\geq \beta^2 \\	 
\end{align}
$$
From the last one is obtained that
$$
	\sqrt{\alpha} \geq \beta \quad\text{and}\quad \sqrt{\alpha} \geq -\beta 
$$
$$
\begin{align}
	\sqrt{\alpha} \geq -\beta \longrightarrow -\sqrt{\alpha}&\leq\beta \\
	\then -\sqrt{\alpha} \leq \beta &\leq\sqrt{\alpha} \\
	\then \abs{\beta}&\leq \sqrt\alpha
\end{align}
$$
## $\beta_\max$ and $\beta_\min$ 

The vector $\ket{\alpha, \beta}$ with the values of $\beta_\max$ and $\beta_\min$ should satisfy 
$$L_+ \ket{\alpha, \beta_\max} = L_- \ket{\alpha, \beta_\min} = 0$$
Let us calculate the product $L_+ L_-$ and its commuted counterpart.
$$
\begin{align}
	L_+ L_- &= (L_x + iL_y)(L_x - iL_y) \\
		&=L_x^2 - i^2L_y^2 + iL_y L_x - iL_x L_y \\
		&= L_x^2 + L_y^2 + i[L_y, L_x] \\
		&= \vec L^2 - L_z^2 + i(-i)\hbar L_z \\
		&= \vec L^2 - L_z^2 + \hbar L_z
\end{align}
$$
By changing the signs $L_- L_+  = \vec L^2 - L_z^2 - \hbar L_z$. Now, from the relation $\ket{\alpha, \beta_\max}$ and \ket{\alpha, \beta_\min} we get 
$$
\begin{align}
	L_- L_+ \ket{\alpha, \beta_\max} = \paren{\vec L^2 - L_z^2 - \hbar L_z}\ket{\alpha, \beta_\max} &=0\\
		\then \paren{\hbar^2\alpha - (\hbar\beta_\max)^2 - \hbar^2\beta_\max} \ket{\alpha, \beta_\max} &= 0\\
		\then \hbar^2\paren{\alpha - \beta_\max^2 - \beta_\max}\ket{\alpha, \beta_\max} = 0
\end{align}
$$

> [!NOTE] Note:
> The second line is obtained by having in mind that $\hbar\beta$ is the eigen value of $L_z$
> 

For non null state (but otherwise arbitrary) $\ket{\alpha, \beta_\max}$
$$
\begin{align}
	\paren{\alpha - \beta_\max^2 - \beta_\max} = 0 \\
	\then \Aboxed{\alpha=\beta_\max(\beta_ \max + 1)}
\end{align}
$$
Similarly is obtained for $\ket{\alpha,\beta_\min}$ 
$$\begin{align}
	L_+ L_- \ket{\alpha, \beta_\min} = \paren{\vec L^2 - L_z^2 + \hbar L_z}\ket{\alpha, \beta_\min} &=0 \\
	\then \hbar^2\paren{\alpha - \beta_\min^2 + \beta_\min} &= 0 \\
	\then \Aboxed{\alpha = \beta_\min(\beta_\min - 1)}
\end{align}$$
# Summary
Knowing this, we rename those extreme values $\{\beta_\max, -\beta_\min\}\rightarrow l$ and $\beta\rightarrow m$ to get in summary

$$
\begin{align}
	\vec L^2 \ket{l,m} &= \hbar^2 l(l+1) \ket{l, m} \\
     L_{z} \ket{l, m} &= \hbar m \ket{l, m}    \\
     \abs m &\le l
\end{align}
$$
# References

[Quantum Mechanics: concepts and applycations, Zettili - Ch 5](file:///home/gabo/Zotero/storage/HWQRMLQL/Zettili%20-%202009%20-%20Quantum%20mechanics%20concepts%20and%20applications.pdf)
[Theoretical Physics 7, Nolting. Ch 5](file:///home/gabo/Zotero/storage/C6NX664M/Nolting%20-%202017%20-%20Theoretical%20Physics%207%20Quantum%20Mechanics%20-%20Methods.pdf)
