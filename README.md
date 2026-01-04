# DS-009-model-tf-idf-logreg-Comparison-ConfusionMatrix

## 📊 Comparación de Matrices de Confusión según el Tamaño del Dataset
### 📌 Descripción

Este repositorio contiene el notebook `confusion_matrix_analisis.ipynb`, cuyo objetivo es comparar el desempeño de un mismo modelo de clasificación de sentimientos entrenado con datasets de distintos tamaños, utilizando matrices de confusión como principal herramienta de análisis.

El enfoque permite observar cómo el volumen de datos afecta la capacidad del modelo para clasificar correctamente los sentimientos negativo, neutro y positivo.

### 📂 Archivo principal

- `confusion_matrix_analisis.ipynb`
Notebook que incluye:
  - Carga de matrices de confusión generadas con diferentes tamaños de dataset
  - Visualización individual y comparativa de las matrices
  - Análisis del comportamiento del modelo según la cantidad de datos de entrenamiento

### 🎯 Objetivo del análisis
  - Evaluar la estabilidad y consistencia del modelo frente a distintos volúmenes de datos.
  - Identificar mejoras o degradaciones en la clasificación de cada clase.
  - Analizar errores comunes y patrones de confusión entre sentimientos.
  - Justificar la elección de un tamaño de dataset adecuado desde una perspectiva técnica.

### 📐 Metodología
1. Entrenamiento del modelo
    - El mismo modelo de clasificación se entrena utilizando datasets de diferentes tamaños (por ejemplo: 1 000 registros, 5 000 registros y dataset completo).
3. Obtención de matrices de confusión
    - Para cada entrenamiento se genera una matriz de confusión que refleja:
      - Predicciones correctas (diagonal principal)
      - Errores de clasificación entre clases
4. Comparación visual y numérica
    - Las matrices se presentan de forma independiente y comparativa para facilitar la interpretación del impacto del tamaño del dataset.

### 📊 Interpretación de resultados

El análisis de las matrices de confusión permite observar que:
- Con datasets pequeños, el modelo presenta mayor confusión entre clases, especialmente entre sentimientos neutros y positivos o negativos.
- A medida que aumenta el tamaño del dataset, se incrementa la cantidad de aciertos y se reduce la confusión entre clases.
- Los valores altos en la diagonal indican una mejor capacidad de generalización del modelo.
- Los valores fuera de la diagonal revelan debilidades específicas en la clasificación.

### 🧠 Importancia del análisis

Este enfoque es clave porque:
- Las métricas globales pueden ocultar errores por clase.
- La matriz de confusión ofrece una visión detallada del comportamiento real del modelo.
- Permite tomar decisiones fundamentadas sobre la cantidad de datos necesaria para entrenar modelos confiables.

### 🛠️ Tecnologías utilizadas

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook / Google Colab

🚀 Ejecución

1. Abrir el archivo confusion_matrix_analisis.ipynb.
2. Ejecutar las celdas en orden para visualizar y comparar las matrices de confusión.
3. Analizar los resultados según el tamaño del dataset utilizado.
