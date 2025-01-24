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

Para utilizar el modelo, es necesario cargar el modelo serializado y preparar los datos de entrada con el mismo formato que los datos de entrenamiento. El modelo generará una probabilidad de incumplimiento para cada nuevo individuo. La scorecard asociada al modelo permite interpretar estas probabilidades en términos de riesgo crediticio.
