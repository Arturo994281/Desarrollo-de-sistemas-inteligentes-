
Subir dos ejemplos extra de aplicaciones donde se muestre T,E,P (Tarea, experiencia y medicion)

**ACT 2.1**

**Netflix**

**Tarea:** Recomendar películas y series que probablemente le gusten al usuario.

**Experiencia:** El usuario recibe recomendaciones personalizadas según lo que ha visto, buscado o calificado.

**Medición:** Se puede medir cuántas recomendaciones son seleccionadas, cuánto tiempo permanece viendo el contenido y la precisión de las recomendaciones.

 **Gmail**

**Tarea:** Detectar automáticamente correos que probablemente sean spam.

**Experiencia:** El usuario recibe los correos normales en su bandeja de entrada y los mensajes sospechosos son enviados automáticamente a la carpeta de spam.

**Medición:** Se mide qué tan correctamente identifica los correos spam, considerando falsos positivos y falsos negativos.

Planteamiento y solucion de problemas con machine learning

Machine learning: 
La capacidad de una computadora de aprender sin haber sigo programada explicitamente para la tarea que termina resolviendo 
Un programa aprende de una experiencia E, respecto a una tarea T y una medida de desempeño P, si su desempeño en T, medido por P,  mejoran con la experiencia. Mitchell obliga a definire 3 cosas antes de programar: tarea, experiencia y medición de acierto. 

Flujo de trabajo
Definir la tarea (T): qué se quiere predecir o decidir
Reunir la experiencia (E): los datos de lso que el sistema va a aprender
Elegir cómo medir el desempeño (P): la métrica que dirá si el modelo sirve
Entrenar: el algoritmo ajusta sus parámetros internos para minimizar el error sobre los datos de entrenamiento
Evaluar: se mide P sobre datos que el modelo nunca vio durante el entrenamiento
Usar o ajustar: si P es suficiente, se despliega; si no, se repite el ciclo con más datos o un modelo distinto

Clasificación de Machine Learning
Supervisado: el agente observa algunos apres de ejemplo entrada-salida y aprende una función que va de la entrada a la salida
No supervisado: el agente aprende patrones en la entrada aunque no se le proporcione retroalimentación explícita
Por refuerzo: es aprender qué hacer, como asociar situaciones con acciones, de manera que se maximice una señal numérica de recompensa

**ACT 2.2**

Estudiar los 3 artefactos y escribir con sus propias palabras en que consisten cada una de las 3 clasificaciones.

Supervisado: explica haciendo evaluaciones como si se estuviera entrenando
Sin supervisar: explica las cosas recibiendo información y probando que le va bien y que le va mal
Por refuerzo: busca por prueba y error

**ACT 2.3**

**Glosario (Todo con base en machine learning)

**-Pandas:** Es una biblioteca de Python utilizada para la manipulación, limpieza, organización y análisis de datos. Trabaja principalmente con estructuras llamadas Series y DataFrame. Puede manejar datos tabulares, datos numéricos y de texto, datos de fechas y horas, datos estadísticos y datos provenientes de archivos como CSV, Excel y bases de datos. 

**-Matplotlib:** Es una biblioteca de Python utilizada para crear gráficos y visualizar datos. Permite representar datos numéricos mediante diferentes tipos de gráficos, como gráficos de líneas, barras, dispersión, histogramas y gráficos tridimensionales. También cuenta con datos de prueba para algunas de sus funciones, como conjuntos de datos utilizados para realizar representaciones en 3D.

**-Scikit-learn:** es una biblioteca de Python especializada en Machine Learning. Contiene herramientas para clasificación, regresión, agrupamiento, reducción de dimensionalidad, selección de modelos y evaluación de modelos.
Entre sus conjuntos pequeños o de prueba se encuentran:

**Iris:** conjunto de datos para clasificación de especies de flores.

**Diabetes:** conjunto de datos utilizado para problemas de regresión.

**Digits:** conjunto de datos de imágenes de números escritos a mano para clasificación.

**Linnerud:** conjunto de datos relacionado con ejercicio físico.

**Wine:** conjunto de datos para clasificación de diferentes tipos de vino.

**Breast Cancer Wisconsin:** conjunto de datos para clasificación relacionada con cáncer de mama.


**-Google colab:** es un servicio de Google que permite escribir y ejecutar código Python desde un navegador. Es utilizado en Machine Learning para trabajar con bibliotecas, conjuntos de datos, modelos y notebooks sin tener que instalar todo el entorno de programación localmente.

**-Árbol de decisión:** es un algoritmo de Machine Learning supervisado que utiliza una estructura formada por nodos y ramas para tomar decisiones a partir de las características de los datos. Puede utilizarse principalmente para problemas de clasificación y regresión.

**-Matriz de confusión:** es una herramienta utilizada para evaluar modelos de clasificación. Compara las clases reales de los datos con las clases predichas por el modelo y permite identificar los aciertos y errores de clasificación.

**-Sobreajuste:** también conocido como overfitting, ocurre cuando un modelo de Machine Learning aprende demasiado los datos utilizados durante el entrenamiento, incluyendo características específicas o ruido, provocando que tenga un buen rendimiento con los datos de entrenamiento pero un rendimiento menor con datos nuevos.

**-Falso positivo:** ocurre cuando una prueba o situación indica que algo está presente o sucede, pero en realidad no está presente o no sucede.

**-Falso negativo:** ocurre cuando una prueba o situación indica que algo no está presente o no sucede, pero en realidad sí está presente o sí sucede.












