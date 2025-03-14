### Procesos de decisión de Markov

Dado un $X_t$ que es un MDP (Markov decision process) de *primer orden*:  

El estado en un tiempo dado solo depende del estado en el tiempo anterior.

Ejemplo de un modelo MDP:  
![](../imagenes/markov/ejemplo.png)  

$p_{ij} = Pr(X_{t+1} = S_i | X_t = S_j)$  
$p_{ij}$ es la probabilidad de ir a el estado $S_i$ desde el estado $S_j$.

La *matriz de probabilidad* del ejemplo es:  
$$ P =
\begin{array}{|c c|}
	0.3 & 0.5\\
	0.7 & 0.5
\end{array}
$$

Dado $P(X_0)$, un vector con las probabilidades de estar en cada estado en el tiempo inicial:  
$P(X_t) = P^tP(X_0)$   
$P(X_{t+1}) = PP(X_t)$  

Si el MDP es *estacionario* entonces en un tiempo lo suficientemente grande:  
$P(X_{t+1}) = P(X_t)$

___

MDP = \<S, A, A$_l$, T, r, S$_t$, $\gamma$>