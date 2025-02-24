## Planeación o busquedas

Si se quiere encontrar el camino con el menor costo de un nodo a otro se utilizan *algoritmos de busqueda*.

Modelamos un grafo donde los nodos son un estado y las aristas son las acciones.

Analizamos los nodos para ver a que otros nodos podemos llegar al realizar acciones legales.

Se guarda en una *frontera* los 
nodos no explorados.

**Plan**: Secuencia de acciones

#### Algoritmo general de busqueda
![](../imagenes/busquedas/pseudocodigo.png)  
### Depth First Search (DFS) / A lo profundo

La frontera se implementa con una **pila** (una estructura **LIFO**) y se expande checando el tope de la pila, o sea el último elemento.

![](../imagenes/busquedas/DFS.png)  
**Orden en el que se checan los nodos**

### Breadth First Search (BFS) / A lo ancho

La frontera se implementa con una **cola** (una estructura **FIFO**) y se expande checando el elemento que lleva más tiempo en la cola.

![](../imagenes/busquedas/BFS.png)  



### Uniform Cost Search (UCS) / Costo uniforme
c(n)
...
### Algoritmo Greedy
h(n)
...
### A* / A estrella / A-sterisco
c(n)+h(n)
...