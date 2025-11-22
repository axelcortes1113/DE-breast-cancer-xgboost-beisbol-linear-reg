# 🧠 Modelos de Machine Learning – Clasificación y Regresión

Este repositorio contiene dos proyectos de aprendizaje automático, uno enfocado en **salud (detección de cáncer de mama)** y otro en **deportes (predicción de carreras en béisbol)**.  
Cada modelo fue entrenado, evaluado y optimizado para obtener los mejores resultados posibles en su respectivo dataset.

---

# 1️⃣ Clasificación de Cáncer de Mama – XGBoost Classifier  
**Objetivo:** Detectar tumores **Malignos (M)** o **Benignos (B)** usando el dataset *breast_cancer.csv*.

- **Dataset:** 569 pacientes, 30 características.  
- **Modelo final:** `XGBoostClassifier` optimizado.

## 📊 Resultados
- **Accuracy:** 97.4%  
- **Precision:** 98.1%  
- **Recall:** 95.3%  
- **F1-Score:** 96.7%  
- **ROC-AUC:** 99.8%  

➡️ *Detecta más del 95% de los casos malignos con muy pocos falsos positivos.*

## 📁 Archivos
- `breast_cancer.csv` → dataset original  
- `breast_cancer_xgboostDE.ipynb` → notebook con análisis, EDA y optimización  
- `best_xgb_classifier.pklDE` → modelo entrenado  

# 2️⃣ Predicción de Carreras en Béisbol – Regresión Lineal + Ridge
**Objetivo:** Predecir el número de carreras (runs) que anota un equipo MLB usando únicamente su número de bateos.

- **Dataset:** 30 equipos MLB (temporada 2008)
- **Modelo final:** Ridge Regression (alpha = 10)
- **Algoritmo alternativo**: Antes se usó Random Forest → ahora una regresión lineal regularizada para evitar overfitting

## 📊 Resultados
- **R²:** 0.372
- **RMSE:** 83.45
- **MAE:** 70.12
- **Correlación bateos–runs:** 0.611

➡️ *Modelo simple, interpretable y sin overfitting. Ideal para datasets pequeños (30 observaciones).*

## 📁 Archivos

- `beisbol.csv` → dataset original

- `beisbol_linear_regressionDE.ipynb` → análisis completo + gráficas

- `best_lr_model.pklDE` → modelo Ridge entrenado




