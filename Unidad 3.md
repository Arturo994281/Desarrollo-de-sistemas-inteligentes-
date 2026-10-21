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
![[Pasted image 20261008181845.png



**ACTIVIDAD 3.2**

- **Algoritmo:** A*
- **Longitud del camino:** **21**
- **Tiempo:** **0.4000 ms**
- **Operaciones:** **197**
En cada movimiento calcula qué camino parece ser el mejor usando:

**f(n) = g(n) + h(n)**

![[Pasted image 20261014155208.png]]




- **Algoritmo:** Ciego
- **Longitud:** **16**
- **Tiempo:** **1.8000 ms**
- **Operaciones:** **973**

encontró un camino de **16 movimientos** desde el punto verde hasta el rojo.
![[Pasted image 20261014155800.png]]![[Pasted image 20261014155811.png]]

la diferencia es que **a*** usa una heurística para tratar de irse por el camino más conveniente, y la ciega no tiene esa ayuda y va checando los caminos por niveles**, por eso la ciega hizo más operaciones y tardó más.

ACT3.3

Actividad 3.3 
Preguntas
**1. Sección “How does machine learning work?”** El artículo menciona tres tipos de aprendizaje. Anótalos y escribe con tus palabras en qué se diferencian.

Aprendizaje supervisado: aprende a partir de datos que ya tienen respuestas correctas o etiquetas
Aprendizaje no supervisado: recibe datos sin respuestas previamente indicadas y busca patrones, semejanzas o grupos. 
Aprendizaje por refuerzo: aprende mediante la interacción con su entorno, recibiendo recompensas o penalizaciones según sus acciones

Osea Supervisado aprende con ejemplos con respuestas, No Supervisado descubriendo patrones por su cuenta y Por Refuerzo mediante las consecuencias de sus decisiones. 

**2. Sección “What is machine learning used for?”** Elige una aplicación (reconocimiento de imágenes, diagnóstico médico, conducción automática, texto y voz) y describe con las ideas de la clase de qué se trata: ¿cuál sería la tarea (T) y qué datos serían la experiencia (E)?

El Machine Learning puede analizar información medica para identificar patrones relacionados con enfermedades y ayudar a los médicos a detectar posibles problemas.

T: identificar si un paciente podría tener una enfermedad a partir de sus síntomas, laboratorios o estudios médico

E: conjunto de datos de pacientes anteriores, sus síntomas, resultados de análisis y diagnósticos confirmados 

**3. Sección “When to use machine learning?”** Según el artículo, ¿cuándo conviene usar ML en lugar de reglas tradicionales? Da un ejemplo de un problema donde NO convendría.
Cuando se tienen grandes cantidades de datos y es difícil encontrar patrones o hacer predicciones mediante reglas tradicionales

Cuando si conviene: detectar transacciones bancarias sospechosas porque los fraudes pueden presentar patrones diferentes y cambiar con el tiempo 

Cuando no conviene: calcular el total de una compra con precios fijos; es suficiente con multiplicar las cantidades por sus precios y sumar los resultados, no es necesario un modelo 

**4. Sección de aplicaciones, “Fraud detection” y “Anomaly detection”.** El artículo dice que en detección de anomalías los modelos no supervisados detectan irregularidades sin datos etiquetados como “normales”. ¿Por qué un enfoque no supervisado tiene sentido para detectar fraudes raros? ¿Qué problema tendría un modelo supervisado?

Tiene sentido porque pueden aparecer de formas nuevas que todavía no está registradas, el modelo puede aprender los patrones habituales de las transacciones y señalar las inusuales 

El modelo supervisado tendría el problema de depender de ejemplos previamente etiquetados como fraudulentos o legítimos, como los fraudes poco comunes, podría haber pocos ejemplos para entrenarlo y no aprendería a reconocerlos en modalidades que nunca ha visto

**5. Sección de aplicaciones, “Healthcare” o “Finance”.** Elige una. Escribe qué error de un modelo sería **peor**, el falso positivo o el falso negativo, y explica por qué.

En el ámbito de la salud, considero que el error más grave sería el falso negativo porque ocurre cuando el modelo indica que no hay una enfermedad cuando en realidad si la hay, esto podría retrasar el diagnóstico y el tratamiento necesario, poniendo en riesgo la salud del paciente.

También en el falso positivo, el modelo indica que se tiene una enfermedad cuando en realidad no es así, causando preocupación y pruebas medicas innecesarias pero aquí la gravedad dependería más de la enfermedad y sus circunstancias

**6. Sección “Machine learning examples by company”.** Elige un caso (Meta, Amazon). ¿Qué datos crees que usa el sistema? ¿Quién se beneficia y quién podría salir perjudicado (por ejemplo, por privacidad)?

Amazon: usa ML para recomendar productos segun intereses y compras de clientes

Podría utilizar: historial de compras, productos consultados, búsquedas de artículos agregados al carrito y compras de otros usuarios con intereses similares

Beneficia: a los clientes porque pueden encontrar productos de su interés fácilmente y a Amazon aumentando sus ventas 

Perjudica: a los usuarios cuya privacidad se vea afectada por la recopilación y análisis de sus datos de consumo, podrían recibir recomendaciones demasiado personalizadas o quedar expuestos a publicidad que influya sus decisiones 

**7. Lectura crítica.** Revisa el título y la sección de experiencia de la empresa. Escribe al menos dos cosas que te hagan dudar de la información y qué le pedirías al autor para confiar más. (Pista: ¿cuántos casos promete el título y cuántos hay? ¿qué cifras aparecen sin explicar cómo se midieron? ¿quién escribe el artículo y qué vende?)

El título promete 12 aplicaciones de Machine Learning pero algunas son muy parecidas entre ellas, le preguntaría al auto cómo las clasificó. 

Menciona cifras como que la precisión de los pronósticos llega al 80% y que se puede aumentar la retención de usuarios más del 30% pero no explica cómo obtuvo esos datos ni que datos fueron utilizados para medirlo, preguntaría por las fuentes que "respaldan" estas cifras

Como es de una empresa que ofrece servicios de tecnología, me hace pensar que podría estar destacando más las ventajas del Machine Learning que sus desventajas; buscaría fuentes independientes que confirmen lo que dice.



ACT3.4
**Qué relación las GPUS con las redes neuronales y las neuronas? como se beneficiaron una de otra?** 
Las GPU ayudan a las redes neuronales porque hacen muchos cálculos al mismo tiempo.  
Las redes neuronales están inspiradas en las neuronas del cerebro y necesitan muchos cálculos.  
Por eso, las GPU permitieron entrenarlas más rápido y las redes neuronales impulsaron GPU más potentes.

ACT 3.5
![[Pasted image 20261021162700.png]]