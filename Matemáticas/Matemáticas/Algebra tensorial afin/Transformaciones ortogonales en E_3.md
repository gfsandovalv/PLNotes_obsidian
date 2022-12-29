### <font color="#f79646">Transformaciones ortogonales en $E_3$</font>

Consideremos una transformación desde un sistema de coordenada rectangular a otro, asumiendo que estos sistemas tienen un origen común en el punto $O$ de espacio euclídeono tridimensional $E_3$. Los vectores unitarios en las direcciones positivas de los ejes $OX^1$,$OX^2$,$OX^3$ son denotados por $\vec{e_1}$,$\vec{e}_2$,$\vec{e_3}$
$$\begin{equation}
 \vec{e_i}\cdot\vec{e_j}=\delta_{ij} \hspace{3cm}(i,j=1,2,3)
\end{equation}\tag{1}$$

Es decir que los vectores $\vec{e_i}$ constituyen una base ortonormal de $E_3$, lo cual significa que cualquier vector de $E_3$ puede ser expresado como una combinación lineal de los vectores bases. En particular, para los vectores bases de otra base ortonormal centrada en $O$, denotada por $\vec{f_i}$   ($i=1,2,3$), podemos escribir:

$$\begin{eqnarray*}
 \begin{array}{c}
  \vec{f_1}=a_11\vec{e_1}+a_12\vec{e_2}+a_13\vec{e_3}\\
 \vec{f_2}=a_21\vec{e_1}+a_22\vec{e_2}+a_23\vec{e_3}\\
 \vec{f_3}=a_31\vec{e_1}+a_32\vec{e_2}+a_33\vec{e_3}
\end{array}
&\Rightarrow&
\begin{array}{lcr}

\left(\begin{array}{c}
   \vec{f_1}\\
  \vec{f_2}\\
  \vec{f_3}
  \end{array}
\right)
& = &
\left(
\begin{array}{c c c}
a_11 & a_12 & a_13\\
a_21 & a_22 & a_23 \\
a_31 & a_32 & a_33
\end{array}
\right)
\left(\begin{array}{c}
    \vec{e_1}\\
    \vec{e_2}\\
    \vec{e_3}
  \end{array}
\right)
\end{array}
 \end{eqnarray*}
$$
 Donde los $a_{ik}$ son parámetros reales que dependen de la dirección de los vectores $\vec{f_i}$ con respecto a las bases $\{\vec{e_j}\}$ . 
 De modo más compacto podemos escribir
 $$\vec{f_j}=\sum^{3}_{i=1}a_{ji}\vec{e_i}
 \tag{2}$$
 Claramente esta transformación es caracterizada completamente por la matriz de $3\times 3 (a_{ik})$, cuyos elementos poseen una simple interpretación geométrica: Cuando los productos escalares de $\vec{f_j}$ con $\vec{e_k}$ son construidos y la relación (1) es tomada en cuenta tenemos:
$$ \vec{f_j}\cdot\vec{e_k}=\sum^{3}_{i=1}a_{ji}\vec{e_i}\cdot=\sum^{3}_{i=1}a_{ji}\delta_{ik}=a_{jk}
 $$
 $$\begin{equation}
 \vec{f_j}\cdot\vec{e_k}=a_{jk}
\end{equation}\tag{3}$$
y puesto que $\vec{f_j}$ y $\vec{e_j}$ son vectores unitarios, tenemos:
$$a_{jk}=\vec{f_j}\cdot\vec{e_k}=\mid\vec{f_j}\mid\mid\vec{e_k}\mid\cos(\vec{f_j},\vec{e_k})\hspace{2 cm}
$$
$$ a_{jk}=\cos(\vec{f_j},\vec{e_k})\hspace{2cm}(j,k=1,2,3)
\tag{4}$$
De modo que los coeficientes $a_{jk}$ en (3) son simplemente los cosenos de los ángulos entre los diferentes vectores bases de dos sistemas ortonormales, lo cual implica que los $a_{jk}$ no pueden asumir valores arbitrarios ser independientes uno de los otros. En realidad existe un conjunto de relación entre ellos el que puede ser obtenido como sigue:
Para la base ortonormal $\{\vec{f_j}\}$ se tiene
$$
 \vec{f_i}\cdot\vec{f_j}=\delta_{ij}\hspace{3 cm}
$$
de modo que, de acuerdo con (2)
$$\begin{eqnarray*}
\delta_{jk}&=&\left[\sum^{3}_{i=1}a_{ji}\vec{e_i}\right]\left[\sum^{3}_{l=1}a_{hl}\vec{e_l}\right]=\sum^{3}_{i=1}\sum^{3}_{l=1}a_{ji}a_{kl}(\vec{e_i}\vec{e_l})\\
 \delta_{jk}&=&\sum^{3}_{i=1}\sum^{3}_{l=1}a_{ji}a_{kl}\delta_{il}=\sum^{3}_{i=1}a_{ji}a_{ki}
\end{eqnarray*}$$
$$
 \delta_{jk}=\sum^{3}_{i=1}a_{ji}a_{ki}
\tag{5}$$
La traspuesta $a_{jl}$ de los elementos $a_{lj}$ de la matriz $(a_{lj})$ es denotada por $a^T_{lj}$, por lo que (5) puede ser escrita como
$$\begin{equation}
\sum^{3}_{i=3}a_{ji}a^{T}_{ik}=\delta_{jk}\hspace{2 cm}(i,k=1,2,3)
\end{equation}\tag{6}$$
Estas relaciones representan una condición necesria que deben satisfacer los coeficientes $a_{ji}$ en (2) para que (2) represente una transformación desde una base ortonormal a otra. Invirtiendo los argumentos es directo mostrar que (6) es también una condición suficiente. Cualquier transformación lineal que satisfaga (6) es llamado una transformación ortogonal y correspondiente matriz $(a_{ji})$ es llamada matriz ortogonal
$$(6)\hspace{1 cm}\leftrightarrow\hspace{1 cm} AA^T=I$$
Es evidente, de la definición de determinante que:
$$det(a^T_{ji})=det(a_{ij})$$
y por tanto
$$\begin{eqnarray*}
det(a_{ji})det(a^T_{ik})=\left[det(a_{ij})\right]^2=det\delta_{ij}=1
\end{eqnarray*}$$
de modo que el determinante de cualquier matriz ortogonal satisface la condición
$$\begin{equation}
 det(a_{ij})=\pm 1
\end{equation}\tag{7}$$
De modo que $det(a_{ij})\neq0$, y por lo tanto a la inversa de la matriz $(a_{ij})$ existe. De (\ref{6}) vemos que la inversa de una matriz ortogonal es idéntica a su traspuesta
$$(a_{ij})^T=(a_{ij})^{-1}$$
Esto puede ser iludtrado por geometricamente por el hecho que la matriz de la transformación inversa de (2) es en efecto, la traspuesta de la matriz $(a_{ji})$ que caracteriza (2) multiplicando (2) por  $a^T_{kj}$ y luego sumando sobre $j$ de 1 a 3 y considerando (6) tenemos:
$$\begin{eqnarray*}
 \vec{f_j}=\sum^{3}_{i=3}a_{ji}\vec{e_i}&\hspace{1 cm}\lfloor\, a^T_{kj}\hspace{0.5 cm} \lfloor \sum_{j}\\
  \sum^{3}_{j=1}a^T_{ij}\vec{f_j}=\sum^{3}_{j=1}\sum^{3}_{i=1}a^T_{kj}a_{ji}\vec{e_i}=\sum^{3}_{i=3}\delta_{ki}\vec{e_i}&
\end{eqnarray*}$$
$$\begin{equation}
 \vec{e_k}=\sum^{3}_{j=1}a^{T}_{kj}\vec{f_j}
\end{equation}\tag{8}$$
Esta relación expresa los vectoresbases $\vec{e_k}$ en términos de los $\vec{f_j}$ y representa el inverso de la transformación ortogonal (2). Además en la misma manera en que (2) de lugar a (4) tenemos:
$$
\vec{e_k}\cdot\vec{f_i}=\sum^{3}_{j=1}a^T_{kj}\vec{f_j}\cdot\vec{f_i}=\sum^{3}_{j=1}a^T_{kj}\delta_{ji}=a^T_{ki}
$$
$$\begin{equation*}
 \Rightarrow \hspace{3 cm}a^T_{ki}=\vec{e_i}\vec{f_i}=\mid\vec{e_k}\mid\mid\vec{f_i}\mid\cos(\vec{e_k},\vec{f_i})\hspace{3 cm}
\end{equation*}$$
$$\begin{equation}
 \Rightarrow \hspace{2 cm}a^T_{ki}=cos(\vec{e_k},\vec{f_i})
\end{equation}\tag{9}$$
Sea $\{\vec{g}_l\}$ la base de vectores de una tercera base ortogonal cuyo origen está localizado en O. Claramente cada vector $\vec{g}_l$ puede ser representado en términos de la base original: 
Por ejemplo
$$ \vec{g}_l=\sum^{3}_{j=1}c_{lj}\vec{f}_{j}
 \tag{10}$$
 Usando (2) tenemos,
$$\tag{11}\vec{g}_l=\sum^{3}_{i=1}\sum^{3}_{j=1}c_{lj}a_{ji}\vec{e}_{i}$$
De modo que si escribimos
$$\begin{equation}
 \vec{g}_l=\sum^{3}_{i=1}b_{li}\vec{e}_{i}
 \end{equation}\tag{12}$$
 tenemos
$$\begin{equation}
b_{li}=\sum^{3}_{j=1}c_{lj}a_{ji}
 \end{equation}\tag{13}$$
la cual prueba que la matriz $b_{li}$ es el producto de las matrices $(c_{li})$ y $(a_{ji})$.

La transformación caractericazada por la matriz $b_{li}$ es llamada el producto de las transformaciones (10) y (2). Por lo tanto, puesto que $b_{li}$ es ortogonal por construcción, se sigue que el producto de cualquier par de transformaciones ortogonales es denuevo ortogonal. También, puesto que el producto de matrices satisface obviamente una ley asociativa, podemos inferir que el conjunto de todas las transformaciones ortogonales en $E_3$ está dotado con una operación binaria asociativa, a saber, el producto, el cual es tal que el producto de cualquier par de elementos es denuevo un elemento del conjunto. Además, este conjunto contiene un elemento unidad, definido como la transformación identidad cuyos coeficientes son deltas de kronecker, mientras que la existencia del inverso de cada elemento es asegurado. Así tenemos que el conjunto de todas las transformaciones ortogonales en $E_3$  forman un grupo llamado el grupo ortogonal usualmente denotado por $O(3)$