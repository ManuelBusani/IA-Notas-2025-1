## Notas del 20 al 24 de enero

### Aprendizaje máquina (machine learning)

Desconocemos si existe una función perfecta f: X -> Y.  
Asumimos que existe y hacemos un programa para que haga el programa.  

Tenemos una muestra de datos con distribución desconocida.  

Un error que es una variable aleatoria de distribución desconocida.

E<sub>in</sub>:  
Error en la muestra.
 
E<sub>out</sub>:  
Error ...

función h.  

Hay aprendizaje cuando:
* E<sub>in</sub>(h) approx 0
* E<sub>in</sub>(h) approx E<sub>out</sub>(h)

Mejorar la confianza a cambio de aumentar el error.  

f approx h iff Eout(h) approx 0

Función de crecimiento  

Dimensión VC, es el número de parámetros.  
Se necesita 10 veces la dimensión VC para asegurar que haya aprendizaje.

## Arboles de decisión
Explican los datos segun sus atributos.

### Entropía
Se usa para elegir con que atributo dividir el árbol.

H(Y) = -sum{P(Y=y<sub>i</sub>)*log<sub>2</sub>P(Y=y<sub>i</sub>)}