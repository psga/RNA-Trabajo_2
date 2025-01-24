## Modelo de Probabilidad de Incumplimiento

### Introducción
Este repositorio contiene los archivos y scripts necesarios para entrenar, evaluar y utilizar el modelo de probabilidad de incumplimiento basado en redes neuronales artificiales. El modelo ha sido diseñado para predecir la probabilidad de que un individuo incumpla con el pago de un crédito. Además, el modelo se puede representar mediante una scorecard, lo que facilita su interpretación y uso en entornos empresariales.

### Estructura del Repositorio
* **Datos_Usados:** Contiene los conjuntos de datos utilizados para entrenar y evaluar el modelo.
    * `dataset_with_scorecard.csv`: Conjunto de datos con la puntuación de riesgo calculada por el modelo.
    * `loan.csv`: Conjunto de datos original de los préstamos.
    * `LCDataDictionary.xlsx`: Diccionario de datos que describe las variables del conjunto de datos.
* **Limpieza de datos:** Scripts utilizados para limpiar y preprocesar los datos.
    * `cleaned_dataset.csv`: Conjunto de datos limpio y preprocesado.
    * `Normalizacion_de_las_columnas_numericas.ipynb`: Notebook para la normalización de las variables numéricas.
    * `preprocesamiento_de_datos.ipynb`: Notebook para el preprocesamiento general de los datos.
* **Modelos:** Scripts y modelos entrenados.
    * `calculo_de_scorecard.ipynb`: Notebook para el cálculo de la scorecard.
    * `entrenamiento_evaluacion_del_modelo.ipynb`: Notebook para el entrenamiento y evaluación del modelo.
    * `serializado.ipynb`: Notebook para serializar el modelo para su uso en producción.
    * **'modelos para uso'**: Carpeta que contiene los modelos entrenados en diferentes formatos.
        * `modelo_clasificador_entrenado.keras`: Modelo clasificador entrenado en formato Keras.
        * `modelo_clasificador.pkl`: Modelo clasificador serializado en formato Pickle.
        * `modelo_probabilidad.keras`: Modelo de probabilidad entrenado en formato Keras.
        * `modelo_probabilidad.pkl`: Modelo de probabilidad serializado en formato Pickle.

### Uso del Modelo
1. **Preparación de los datos:** Asegurarse de que los datos de entrada tengan el mismo formato y las mismas variables que los datos utilizados para entrenar el modelo.
2. **Carga del modelo:** Cargar el modelo serializado en el formato deseado (Keras o Pickle).
3. **Predicción:** Utilizar el modelo cargado para realizar predicciones sobre nuevos datos. El modelo devolverá una probabilidad de incumplimiento para cada individuo.
4. **Interpretación:** Utilizar la scorecard para interpretar los resultados del modelo.

### Consideraciones
* **Escalabilidad:** El modelo puede ser escalado para manejar grandes volúmenes de datos utilizando técnicas de aprendizaje distribuido.
* **Interpretabilidad:** La scorecard facilita la interpretación de los resultados del modelo, lo que permite a los usuarios comprender los factores que influyen en la probabilidad de incumplimiento.
* **Actualización:** El modelo debe ser actualizado periódicamente para mantener su precisión.

### Próximos Pasos
* **Deployment:** Implementar el modelo en una aplicación web o API para facilitar su uso por parte de otros equipos.
* **Monitoreo:** Implementar un sistema de monitoreo para evaluar el desempeño del modelo en producción y detectar posibles problemas.

**Este README.md proporciona una descripción clara y concisa del repositorio, lo que facilitará a otros usuarios entender el proyecto y utilizarlo.**

**Consideraciones adicionales:**

* **Especificidad:** Si tienes más detalles sobre el proceso de entrenamiento, las métricas de evaluación o las características específicas del modelo, puedes incluirlos en el README.
* **Visualizaciones:** Si tienes visualizaciones que ayuden a entender el modelo o los datos, puedes incluir enlaces a ellas.
* **Licencia:** Indica la licencia bajo la cual se distribuye el código.
* **Contribuciones:** Si deseas que otros contribuyan al proyecto, puedes incluir una sección con instrucciones para hacerlo.

