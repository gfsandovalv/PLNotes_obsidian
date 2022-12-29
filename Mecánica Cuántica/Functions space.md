# Wave functions space $\mathcal F$
$\d^3r\abs{\psi(\vec r, t)}^2$ is the probability of finding a particle at region $\d^3 \vec r = \d{x}\d{y}\d{z}$ about the point $\vec r$, at time $t$. Hence, it must satisfy

$$\int \d^3r \,  \abs{\psi(\vec r, t)}^2 = 1$$
This means that $\psi$ is squared-integrable ($\psi \in L^2$).
#TODO link to probaility axioms
## Inner product

> [!Definition]
> Let $\psi$ and $\phi$ be elemets of $\mathcal F$. The complex number 
> $$\int \d^3r \,\psi^*(\vec r)\phi(\vec r) $$ is called inner or scalar product of $\psi$ and $\phi$ and it is dennoted by $(\psi, \phi)$ 

#TODO show that it allways converges given that $\psi$ and $\phi$ be elemets of $\mathcal F$
#TODO add properties of inner product
## Linear operators

> [!Definition] 
> A linear operator is a mapping $A:\psi \mapsto \phi$, where $\psi,\phi\in\mathcal F$. 
> $A$ satisfies linearty, this is $A\paren{\lambda_{1}\psi_{1} + \lambda_{2}\psi_{2}} = \lambda_{1}A\psi_{1} + \lambda_{2}A\psi_{2}$, where $\lambda_{1},\lambda_{2}\in\complexes$

### Some examples
1. Parity operator $\Pi$.
	$\Pi \psi(x,y,z) = \psi(-x, -y, -z)$
2. Multiplication by $x$, $X$
	$X\psi(x,y,z) = x\psi(x,y,z)$
3. Derivative with respect to $x$, $D_{x}$
	$D_{x}\psi(x,y,z) = \ddp{\psi(x,y,z)}{x}$
### Product of operators and comutators
The product of two operators $A$ and $B$ acting over a function $\psi$ is calculated by virtue of associativity $(AB)\psi = A(B\psi)$. In general, $AB\neq BA$. We define the commutator as the difference $[A,B] = AB - BA$. If $[A, B] = 0$ it is said that the operators commute. 

#### Calculation Example: $[X, D_{x}]$
$$
\begin{align}
	[X,D_{x}]\psi(\vec r) &= \paren{x\ddp{}{x}-\ddp{}{x}x}\psi(\vec r) \\
	 & = x\ddp{}{x}\psi(\vec r)-\ddp{}{x}(x\psi(\vec r))  \\
	 & = x\ddp{}{x}\psi(\vec r) - \psi(\vec r) - x\ddp{}{x}\psi(\vec r) \\
	 & = -\psi(\vec r)
\end{align}
$$
This means, since $\psi(\vec r)$ is arbitrary, $[X,D_{x}] = -1$

Another example is shown in ![[Commutation Relations#Angular momentum]]
