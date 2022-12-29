# Cannonical: Position and momentum
We will show that $[x_i,p_j] = i\hbar\delta_{ij}$.
---- ----
Recalling that $p_j = -i \hbar \ddp{}{x_j} = -i\hbar \del_j$  we have
$$
\begin{align}
	[x_i, p_j] &= -i\hbar [x_i, \del_j] \\
			&= -i\hbar \paren{x_i \del_j - (\del_jx_i)}
\end{align}
$$
In order to see more clearly this product, let us apply it over an arbitrary function $\psi$ (See [[Functions space#Calculation Example: $[X, D_{x}]$]])


$$
\begin{align}
	\paren{x_i \del_j - (\del_jx_i)}\psi &= x_i \del_j\psi - \del_j(x_i \psi) \\
		&= x_i \del_j\psi - (\del_j x_i) \psi - x_i \del_j \psi \\
		&= -\delta_{ij}\psi
	
\end{align}
$$
Finally, 
$$
\begin{align}
	[x_i, p_j]\psi &= -i\hbar\paren{-\delta_{ij}\psi} \\
	\Longrightarrow \Aboxed{[x_i, p_j] &= i\hbar\delta_{ij}}
\end{align}
$$

# Angular momentum
## $[L_i,L_j] = L_k$.

$$
\begin{align}
	[L_i,L_j] &= [ \epsilon_{ist}x_s p_t , \epsilon_{jmn}x_m p_n ] \\
		&= \epsilon_{ist}\epsilon_{jmn}[ x_s p_t , x_m p_n ] \\
\end{align}
$$


The last commutator is expanded,
$$
\begin{align}
	[ x_s p_t, x_m p_n ] &= x_s [  p_t, x_m p_n ] + [ x_s, x_m p_n ] p_t\\
		&= x_s x_m \cancel{[  p_t, p_n ]} + x_s [  p_t, x_m ]p_n  + x_m [ x_s, p_n ] p_t + \cancel{[ x_s, x_m ]}p_n p_t \\
		&= -x_s [x_m, p_t]p_n + x_m[ x_s, p_n]p_t \\
		&= -x_s(\delta_{mt})p_n + x_m(\delta_{sn})pt \\
		&= i\hbar \paren{x_m p_t \delta_{sn} - x_s p_n \delta_{mt}}
\end{align}
$$
Returning to the whole expression,   
$$
\begin{align}
	[L_i,L_j] &=i\hbar\epsilon_{ist}\epsilon_{jmn} \paren{x_m p_t \delta_{sn} - x_s p_n \delta_{mt}} \\
		&=i\hbar \paren{\epsilon_{ist}\epsilon_{jmn}x_m p_t \delta_{sn} - \epsilon_{ist}\epsilon_{jmn}x_s p_n \delta_{mt}}
\end{align}
$$
Using [[Levi-Civita symbol]] properties

$$
\begin{align}
	[L_i,L_j] &= i\hbar\paren{\det\paren{\begin{bmatrix}
	\delta_{tj}&\delta_{tm}\\\delta_{ij}&\delta_{im}
	\end{bmatrix}}x_m p_t - \det\paren{\begin{bmatrix}
	\delta_{in}&\delta_{ij}\\\delta_{sn}&\delta_{sj}
	\end{bmatrix}}x_s p_n} \\
	&= i\hbar\paren{\paren{\delta_{tj}\delta_{im} - \delta_{ij}\delta_{tm}}x_m p_t - \paren{\delta_{in}\delta_{sj} - \delta_{sn}\delta_{ij}}x_sp_n} \\
	&= i\hbar \paren{x_i p_j - \cancel{x_tp_t\delta_{ij}} - x_jp_i + \cancel{x_s p_s\delta_{ij}}} \\
	&=  i\hbar \paren{x_i p_j -  x_jp_i } \\
	&= i\hbar \epsilon_{ijk} \,x_i p_j \\
	&= i\hbar\epsilon_{ijk}L_k
\end{align}
$$

## $[\vec L^2,L_k] = 0$
$$
\begin{align}
	[\vec L^2,L_k] &= [L_i L_i,L_k] \\
		&= L_i[L_i,L_k] + [L_i,L_k]L_i \\
		&= i\hbar \paren{\epsilon_{ijk} L_i L_k + \epsilon_{ijk}L_k L_i} \\
		&= i\hbar\epsilon_{ijk}\{L_i,L_k\}
\end{align}
$$
The anticommutator $\{\, ,\,\}$ is symmetric. When it is contracted with Levi-Civita symbol, which is antisymmetric in all its indexes, the result is zero. 
#TODO show contraction of symmetric and antisymmetric tensors


