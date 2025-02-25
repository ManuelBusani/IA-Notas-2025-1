## Juegos con adversarios

### Maneras de clasificarlos

* ¿Es *determinista* o *estocástico*?
* ¿Es perfectamente observable?
* El número de jugadores (al menos 2)
* ¿Es por *equipos* o *individuales*?
* ¿Es de *suma cero*?
> **Suma cero**: la suma de las ganancias de todos los jugadores es 0, o sea que cuando alguien gana los adversarios pierden, por ejemplo ajedrez.

### Modelo
* P := 'conjunto de jugadores' 
* S := 'conjunto de estados'
* s<sub>0</sub> := 'el estado inicial', tal que s<sub>0</sub> ∈ S
* A := conjunto de acciones
* Acciones legales: S x P ⇾ P(A)
* Transición: S x A x P ⇾ S
* es_terminal: S ⇾ {TRUE, FALSE}
* Ganancia: S x P ⇾ R

### Minmax
Se asume que el rival va  a minimizar la ganancia, o sea que va a realizar la mejor acción.
```
valor(estado):
	# estado terminal, por ejemplo jaque mate en ajedrez
	if es_terminal(estado): 
		return utilidad

	# turno del jugador 1 que busca maximizar utilidad
	if turnoj1:
		v = -∞	
		for sucesor in estado.hijos:
			v = max(v, valor(sucesor))
		return v
		
	# turno del jugador 2 que busca minimizar utilidad
	v = +∞	
	for sucesor in estado.hijos:
		v = min(v, valor(sucesor))
	return v	
```
![](../imagenes/juegos/minmax.png)