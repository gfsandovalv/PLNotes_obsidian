# Trajectories: Curves in space
A trajectory is a vector valued map (function)  $\mathbf r : I\subseteq \mathbb R \longmapsto \mathbb R^3$ 
$$ \vec r(t) = x(t) \hat{\vec x} + y(t) \hat{\vec y} + z(t) \hat{\vec z}$$

## Tangent vector

The derivative of the trajectorie with respct to the parameter $t$ 
$$ \vec v(t) = \dd{\vec r}{t}$$
is tangent to the trajectory for any value of the parameter $t$ (at any instant).
Let $\vec T$ and $v$ be the direction and magnitud of $\vec v$ respectively, such that $\vec v = v \vec T$. It means that $\vec T$ is calculated by the rule
$$\begin{align}
	\vec T = \dfrac{1}{\abs{\d \vec r/\d t}}\dd{\vec r}{t}
\end{align}
$$
It follows from assumption that $\vec T \cdot \vec T =1$, then 
$$
\begin{align}
	\dd{}{t}\vec T \cdot \vec T &= 0 \\
	\dd{\vec T}{t} \cdot \vec T + \vec T\cdot\dd{\vec T}{t}  &= 0\\
	\Longrightarrow \dd{\vec T}{t} \cdot \vec T &= 0
\end{align}
$$
## Arc lenght: Traveled distance


$$
\begin{align}
	s(t) = \int_{t_0}^t \d t  \abs{\vec v (t)}
\end{align}
$$


# References
1. [Differential geometry of curves and surfaces - Ch 1](file:///home/gabo/Zotero/storage/L3GCRFG6/Carmo%20-%202018%20-%20Differential%20geometry%20of%20curves%20&%20surfaces.pdf)
2. [Curvature](file:///home/gabo/Documents/temp_docs/parametric_equations.pdf)
3. [Thomas Calculus - Ch 13](file:///home/gabo/Zotero/storage/W78VCNQQ/Hass%20et%20al.%20-%202020%20-%20University%20calculus%20early%20transcendentals.pdf)
