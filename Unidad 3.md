Algoritmos de búsqueda

1. Problemas de búsqueda: son problemas donde un agente busca una manera de llegar a un objetivo. Ejemplo: encontrar el camino más corto para llegar a una casa.

2. Espacio de estados: es el conjunto de todos los estados o lugares a los que se puede llegar durante la búsqueda. Ejemplo: todas las ciudades de un mapa.

3. Estado inicial: es el punto donde comienza la búsqueda. Ejemplo: la ciudad donde estás actualmente.

4. Acciones: son los movimientos que puedes realizar para pasar de un estado a otro. Ejemplo: avanzar a otra ciudad.

5. Modelo de transición: explica qué sucede cuando realizas una acción, es decir, a qué estado llegas. Ejemplo: si estás en A y tomas el camino hacia B, llegas a B.

6. Prueba de meta: sirve para comprobar si ya llegaste al objetivo. Ejemplo: verificar si llegaste a la ciudad que buscabas.

7. Costo del camino: es el valor de recorrer un camino, que puede representar distancia, tiempo o dinero. Ejemplo: recorrer una carretera cuesta 20 minutos.

8. Solución: es una secuencia de acciones que te lleva desde el estado inicial hasta la meta. Ejemplo: A → B → C.

9. Frontera: es el conjunto de nodos que ya se descubrieron, pero que todavía no se exploran por completo.

10. Nodo: es una representación de un estado dentro del árbol de búsqueda. Puede guardar información del estado, su padre, la acción realizada y el costo acumulado.

11. Agente de resolución de problemas: es quien analiza el problema y busca una secuencia de acciones para alcanzar la meta. En inteligencia artificial, puede ser un programa o sistema.

**Sistemas de busqueda (ciega)**

Búsqueda ciega: es una búsqueda que no tiene información adicional para saber qué camino parece mejor. Solo utiliza los datos del problema.

Búsqueda no informada: es otro nombre para la búsqueda ciega. No utiliza pistas o heurísticas para acercarse a la meta.

Búsqueda en profundidad

Sigue un camino lo más lejos posible y, si no encuentra la meta, regresa para probar otro camino.

Ejemplo: exploras un pasillo hasta el final antes de regresar.

Utiliza una pila (LIFO).

Búsqueda de costo uniforme

Explora primero el camino que tenga el menor costo acumulado, aunque tenga más pasos.
 
Ejemplo: elegir la ruta que cuesta menos dinero, no necesariamente la que tiene menos calles.

Utiliza una cola de prioridad.

**Cola (FIFO)**: el primero en entrar es el primero en salir. Como una fila para comprar boletos.

**Pila (LIFO):** el último en entrar es el primero en salir. Como una pila de platos: tomas primero el que quedó arriba.

**Completitud:** indica si el algoritmo garantiza encontrar una solución cuando existe, bajo las condiciones adecuadas.

**Optimalidad:** indica si garantiza encontrar la mejor solución, por ejemplo, la de menor costo.

**Complejidad en tiempo:** mide cuánto trabajo o cuántos nodos puede necesitar explorar un algoritmo.

**Complejidad en espacio:** mide cuánta memoria necesita para guardar los nodos durante la búsqueda.

Busqueda en amplitud:busca llegar a un punto revisando primero todos los puntos más cercanos al inicio y después los siguientes, hasta encontrar el destino.

![[Pasted image 20261008181258.png]]Busqueda primero el mejor:busca llegar a un punto eligiendo en cada paso el camino que parece acercarlo más al destino, usando una estimación.
![[Pasted image 20261008181549.png]]Dijkstra:busca la ruta más barata desde un punto hasta otro, tomando en cuenta el costo de cada camino para encontrar el menor costo total.
![[Pasted image 20261008181845.png]]