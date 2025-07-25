## 🏭 Modelo de predicción para recuperación de oro

### 📌 Introducción

Este proyecto desarrolla un modelo de machine learning para predecir la eficiencia del proceso de recuperación de oro en una planta de procesamiento mineral. El objetivo principal es **predecir las tasas de recuperación en dos etapas clave del proceso**: **Rougher** (primaria) y **Final** (secundaria), basándose en variables del proceso como la concentración de metales, tamaño de partículas y flujo de entrada/salida.

Este análisis es crucial para optimizar los procesos industriales, reducir costos operativos y maximizar la recuperación de recursos valiosos.

---

### 🎯 Objetivos

- Comprender el flujo de datos de entrada y salida de las distintas etapas del procesamiento de oro.
- Explorar y preparar los datos para entrenamiento.
- Entrenar modelos de regresión para predecir la eficiencia de recuperación.
- Evaluar el desempeño con métricas específicas del dominio (sMAPE).
- Aplicar los modelos al conjunto de prueba y comparar con valores reales.

---

### 🧠 Habilidades técnicas demostradas

Este proyecto aplica técnicas avanzadas de ciencia de datos en un contexto industrial, demostrando las siguientes habilidades:

- **Análisis exploratorio de datos (EDA)**: evaluación de concentración de metales, distribución de partículas, y comportamiento en distintas etapas del proceso.
- **Tratamiento de valores nulos**: limpieza de columnas específicas clave para el proceso.
- **Ingeniería de características**: selección y transformación de variables relevantes según su etapa (Rougher o Final).
- **Escalado de datos**: normalización para mejorar el desempeño del modelo.
- **Modelado predictivo**:
  - Entrenamiento de modelos separados para cada etapa (`Rougher`, `Cleaner`)
  - Comparación de modelos con validación cruzada.
- **Evaluación con métricas específicas**: uso del `sMAPE` (Symmetric Mean Absolute Percentage Error) ajustado como KPI al contexto industrial.
- **Visualización**: análisis gráfico de concentraciones y comportamiento del proceso.

---

### 🛠️ Tecnologías y herramientas utilizadas

- **Python**
- **pandas**: manejo y limpieza de datos.
- **NumPy**: operaciones numéricas.
- **scikit-learn**: modelado de regresión, escalado, validación cruzada.
- **matplotlib / seaborn**: visualización de resultados y relaciones.
- **Funciones clave**: `StandardScaler`, `cross_val_score`, `mean_absolute_error`, `RandomForestRegressor`

---

### ✅ Resultados y conclusiones

- Se entrenaron dos modelos de regresión para predecir la recuperación de oro en las etapas Rougher y Final.
- Se seleccionaron las columnas más relevantes para cada etapa, mejorando la precisión.
- El modelo alcanzó un sMAPE aceptable, cumpliendo con los criterios del problema.
- Se identificaron inconsistencias en la toma de datos de recuperación final, recomendando realizar una exploración de las razones de este evento.

---

### 📄 Notebook

El cuaderno interactivo contiene todo el flujo de trabajo del proyecto:
- Carga y preprocesamiento de datos industriales.
- Análisis exploratorio (EDA) con visualizaciones.
- Construcción de modelos de regresión para dos etapas del proceso (Rougher y Final).
- Evaluación con métricas ajustadas al contexto industrial (sMAPE).
- Discusión de resultados y recomendaciones.  

🔗 Ver notebook completo en GitHub → [mining-kpi-predictive-model](https://github.com/AndresCalvete-DataScientist/mining-kpi-predictive-model/blob/main/mining-kpi-predictive-model.ipynb)

---

### 📈 Posibles mejoras futuras

- Implementar modelos no lineales más complejos como Gradient Boosting o XGBoost.
- Incluir variables económicas (costos por tonelada procesada, precio del oro) para análisis de rentabilidad.
- Aplicar reducción de dimensionalidad (PCA).

---

### 👨‍💻 Autor

**Andrés Calvete**  
Científico de Datos Junior  
[LinkedIn](https://www.linkedin.com/in/andrescalvete/)  
ascalvete@hotmail.com
