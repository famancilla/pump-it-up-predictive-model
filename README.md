# pump-it-up-predictive-model
💧 Pump It Up: Predicción de Estado de Bombas de Agua en Tanzania
Este proyecto se centra en la predicción del estado funcional de bombas de agua en Tanzania, utilizando técnicas de Machine Learning sobre datos abiertos provistos por DrivenData. Este trabajo fue realizado como parte de mi proceso de aprendizaje personal, fuera del contexto de mis estudios de máster, con el objetivo de afianzar conocimientos en ciencia de datos aplicada a problemas sociales reales.

📌 Contexto
En muchas regiones rurales de Tanzania, la disponibilidad de agua potable depende del correcto funcionamiento de bombas manuales. Identificar aquellas que requieren mantenimiento o están fuera de servicio permite enfocar recursos y mejorar el acceso al agua. Este proyecto replica un problema real de clasificación multinomial: predecir si una bomba de agua está:

Funcional (functional)

Funcional pero requiere reparación (functional needs repair)

No funcional (non functional)

🎯 Objetivo
Desarrollar un modelo de clasificación supervisada que permita predecir el estado de una bomba de agua en base a características geográficas, técnicas y operativas, buscando aportar en la priorización de mantenimiento y reparación en zonas críticas.

🧠 Metodología
El proyecto fue desarrollado íntegramente en Jupyter Notebook y sigue un pipeline clásico de machine learning:

Carga y exploración de datos

Limpieza y transformación de variables categóricas y numéricas

Imputación de datos faltantes

Feature Engineering

Selección de variables

Entrenamiento de modelos:

Random Forest

Gradient Boosting (XGBoost)

Evaluación con métricas como F1-score, matriz de confusión y validación cruzada

Generación de predicciones para el dataset de test (submission format)

🧾 Datos
Fuente del dataset: DrivenData - Pump it Up Challenge

Tamaño del conjunto de entrenamiento: 59.400 filas

Número total de columnas: 40 características (features)

Incluye datos sobre ubicación, tipo de extracción, método de tratamiento, antigüedad, tipo de instalador, tipo de bomba, etc.

Variables categóricas, numéricas, booleanas y de texto.

📊 Resultados
Se logró construir un modelo robusto de clasificación multicategoría. El modelo final optimizado con GridSearch (Random Forest) obtuvo:

F1 macro promedio en validación cruzada: ~0.80

Importancia de variables clave: antigüedad (construction_year), tipo de bomba (pump_type), fuente de agua (source), entre otras.


🧾 Observaciones
Este proyecto fue desarrollado de manera independiente como parte de mi interés por aplicar machine learning a problemas reales con impacto social. No forma parte de ningún curso formal ni evaluación académica.
