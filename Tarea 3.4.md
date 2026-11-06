# Práctica: entrenar y probar un clasificador con Teachable Machine


**Herramienta:** https://teachablemachine.withgoogle.com
**Modalidad:** por equipos
**Entrega:** un solo archivo (PDF o Markdown en su repositorio) con las evidencias y respuestas que se piden abajo.

---

## 1. Objetivo

Entrenar un clasificador, medir qué tan bien funciona con pocos ejemplos, medir de nuevo con más ejemplos y, después, cambiar las opciones avanzadas para observar cómo se comporta el entrenamiento.

---

## 2. Antes de empezar: elijan el proyecto

Elijan **una** idea en la que la clase se vea en la imagen (no un estado interno como cansancio o miedo):

- Casco o chaleco puesto / no puesto
- Objeto bueno / objeto dañado
- Clasificar basura (papel, plástico, orgánico)
- Postura correcta / incorrecta (proyecto de **pose**)


Mínimo **2 clases**. Escriban en su entrega el proyecto elegido y las clases.

---

## 3. Instrucciones

### Fase A. Entrenamiento con 15 fotos por clase

1. Entren a Teachable Machine y elijan **Get Started**.
2. Creen un proyecto de **Imagen** (o **Pose**, si es el de postura) y elijan el modelo estándar.
3. Renombren las clases con lo que van a reconocer.
4. Capturen **15 imágenes por clase** (con la cámara o subiendo archivos). Varíen el ángulo, el fondo y la luz.
5. **Antes de entrenar**, separen **10 imágenes por clase para prueba**. Estas imágenes **no se suben a la plataforma ni se usan para entrenar**. Guárdenlas en una carpeta aparte.
6. Pulsen **Train Model** y esperen sin cerrar la pestaña. No cambien nada en **Advanced** en esta fase.
7. Midan la precisión:
   - Prueben el modelo con sus **imágenes de prueba** (las 10 por clase que no usaron) en la vista de **Preview**, una por una.
   - Anoten cuántas acertó.
   - Calculen el porcentaje: `aciertos / total de imágenes de prueba × 100`.
8. Tomen las capturas de pantalla que se piden en la sección 4 (Evidencia A).

### Fase B. Agregar 10 fotos más por clase

1. Agreguen **10 imágenes nuevas por clase** al entrenamiento (pasan a 25 por clase). Deben ser distintas de las 10 de prueba.
2. Vuelvan a entrenar con **los mismos ajustes** que en la fase A (sin tocar **Advanced**).
3. Prueben con **las mismas imágenes de prueba** de la fase A. Es importante que sean las mismas para poder comparar.
4. Calculen el nuevo porcentaje y tomen las capturas (Evidencia B).

### Fase C. Opciones avanzadas

1. Usen como base el modelo de la fase B (25 por clase).
2. Abran **Advanced**. Cambien **un solo ajuste a la vez** y vuelvan a entrenar.
3. Prueben con las mismas imágenes de prueba y registren los resultados en la tabla de la sección 5.
4. Después de cada experimento, regresen el ajuste a su valor original antes de cambiar el siguiente.

> Nota: si cambian dos ajustes al mismo tiempo no podrán saber cuál produjo el efecto.

---

## 4. Evidencias que deben entregar

### Evidencia A. Modelo con 15 fotos por clase

- [x] Captura de pantalla del proyecto con las clases y el número de imágenes de cada una (deben verse 15 por clase).
- [x] Captura de **Preview** probando con una imagen de prueba, donde se vea el porcentaje de confianza por clase.
- [x] Si la plataforma muestra métricas después de entrenar (por ejemplo, en el apartado **Under the hood**), captura de la **precisión por clase**.
- [x] Tabla de resultados de su prueba manual (formato de abajo).

### Evidencia B. Modelo con 25 fotos por clase

- [x] Captura del proyecto con las clases y el número de imágenes (deben verse 25 por clase).
- [x] Captura de **Preview** probando con una de las mismas imágenes de prueba.
- [x] Captura de la precisión por clase, si la plataforma la muestra.
- [x] Tabla de resultados de su prueba manual.

### Tabla de resultados (una por fase)

| Imagen de prueba | Clase real | Clase que predijo el modelo | Confianza (%) | ¿Acertó? |
| ---------------- | ---------- | --------------------------- | ------------- | -------- |
| 1                |            |                             |               |          |
| 2                |            |                             |               |          |
| ...              |            |                             |               |          |

**Precisión de la fase** = aciertos / total de imágenes de prueba × 100 = ______ %

### Comparación A contra B

| Fase | Fotos de entrenamiento por clase | Imágenes de prueba | Aciertos | Precisión (%) |
| ---- | -------------------------------- | ------------------ | -------- | ------------- |
| A    | 15                               |                    |          |               |
| B    | 25                               |                    |          |               |
|      |                                  |                    |          |               |

---

## 5. Experimentos con las opciones avanzadas

En **Advanced** encontrarán, según la versión de la página, ajustes como **Epochs**, **Batch Size** y **Learning Rate**. Usen los valores que ofrezca la lista; los de abajo son solo una guía de qué probar (un valor menor y uno mayor que el predeterminado).

| # | Ajuste | Qué probar | Qué observar |
|---|---|---|---|
| 1 | **Epochs** (cuántas veces recorre los ejemplos) | Un valor muy bajo (por ejemplo, 1 a 5), el predeterminado y uno más alto | ¿Con pocas épocas falla en todo? ¿Con muchas deja de mejorar o empieza a memorizar? |
| 2 | **Learning Rate** (qué tan grande es cada ajuste) | Un valor mucho menor y otro mucho mayor que el predeterminado | ¿Cuál se estabiliza? ¿Cuál se comporta de forma errática o no aprende? |
| 3 | **Batch Size** (cuántos ejemplos ve antes de ajustar) | Uno menor y uno mayor que el predeterminado | ¿Cambia la rapidez o la estabilidad del entrenamiento? ¿Cambia la precisión? |
| 4 | **Cantidad de datos** (no está en Advanced, pero conviene probarlo) | 5 imágenes por clase contra 25 por clase, con los demás ajustes iguales | ¿Qué cambia más: los ajustes avanzados o la cantidad de datos? |

### Tabla de registro (una fila por experimento)

| Experimento   | Ajuste cambiado   | Valor usado    | Aciertos en prueba | Precisión (%) | Observación |
| ------------- | ----------------- | -------------- | ------------------ | ------------- | ----------- |
| Base (fase B) | ninguno           | predeterminado |                    |               |             |
| 1a            | Epochs            |                |                    |               |             |
| 1b            | Epochs            |                |                    |               |             |
| 2a            | Learning Rate     |                |                    |               |             |
| 2b            | Learning Rate     |                |                    |               |             |
| 3a            | Batch Size        |                |                    |               |             |
| 3b            | Batch Size        |                |                    |               |             |
| 4             | Cantidad de datos | 5 por clase    |                    |               |             |

Si la plataforma muestra gráficas de exactitud o pérdida por época, tomen captura de la gráfica de al menos un experimento de Epochs y uno de Learning Rate.

---

## 6. Preguntas para responder en la entrega

1. ¿La precisión subió, bajó o se mantuvo al pasar de 15 a 25 fotos por clase? ¿A qué creen que se debe?
2. ¿Qué imágenes de prueba falló el modelo? ¿Qué tenían de distinto respecto a las de entrenamiento (fondo, luz, ángulo)?
3. ¿Qué ajuste avanzado tuvo más efecto en el resultado? ¿Y cuál casi no cambió nada?
4. ¿Su modelo mostró señales de sobreajuste (muy bueno con los ejemplos de entrenamiento, malo con los de prueba) o de subajuste (malo en ambos)? Expliquen con sus resultados.
5. En su proyecto, ¿qué error sería peor: un falso positivo o un falso negativo? Justifiquen.
6. ¿Confiarían en este modelo para usarlo en la vida real? ¿Qué le faltaría?

---


---

## 8. Recomendaciones

- Guarden el proyecto (en la plataforma o descargando el archivo del proyecto, si lo ofrece) antes de empezar los experimentos, para poder regresar al modelo base.
- No cierren la pestaña mientras entrena.
- Si usan imágenes de internet, revisen la licencia y no usen fotos de personas sin su permiso.

