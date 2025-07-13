# Data_Engineer_Clasificacion_NO2  
#CLASIFICACIÓN DE NIVELES DE NO₂ MEDIANTE ÁRBOLES DE DECISIÓN

Este repositorio contiene un proyecto de análisis de datos aplicado a la predicción del nivel de dióxido de nitrógeno (NO₂) en Madrid a partir de datos de contaminación atmosférica. El trabajo incluye limpieza, discretización, análisis de correlación y entrenamiento de modelos de clasificación basados en árboles de decisión y Random Forest.

## 📊 Tecnologías utilizadas

- Python 3  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Seaborn  

## 📁 Estructura

- `2_Min_act_2.ipynb`: Notebook principal con la implementación completa del análisis y entrenamiento de modelos.
- `2_Memoria_Tecnica_carlos_galvez_act2.pdf`: Informe detallado del análisis y resultados.
- `data.csv`: datos necesarios para reproducir el entorno(NO SE INCLUYE EN GITHUB).

## 📌 Objetivo

Predecir el nivel de NO₂ (bajo, medio o alto) en la ciudad de Madrid a partir de otras variables contaminantes como NO, NOx, PM10 o CO. Para ello se discretiza la variable `no2`, se seleccionan atributos predictivos relevantes y se entrenan modelos interpretables.

## 🧠 Metodología

- **Limpieza de datos**: selección de estaciones con más registros válidos, tratamiento de nulos e imputación por media.  
- **Discretización**: uso de `KBinsDiscretizer` con estrategia de cuantiles para clasificar `no2` en tres niveles.  
- **Análisis de correlación**: evaluación de multicolinealidad para seleccionar atributos relevantes y eliminar redundancias.  
- **Clasificación**: entrenamiento y evaluación de:
  - Árbol de decisión (DecisionTreeClassifier)
  - Random Forest con ajuste de hiperparámetros (GridSearchCV)
- **Evaluación**: matriz de confusión, precisión, recall y F1-score por clase.

## 📄 Resultados

- Se alcanzó una **exactitud global del 76 %** con el árbol de decisión simple.  
- El modelo Random Forest optimizado mejoró la clasificación especialmente en la clase intermedia (`medio`).  
- Se demostró que eliminar variables altamente correlacionadas (como `nox`) no degrada gravemente el rendimiento, simplificando el modelo.

## 📄 Propuesta de aplicación real

Random Forest es una técnica ampliamente utilizada en entornos reales:
- Detección de fraude financiero
- Evaluación de riesgos crediticios
- Predicción médica y genómica
- Motores de recomendación

## 🧑‍💻 Autor  
Carlos Gálvez Reguera

> Este proyecto se desarrolló como parte de una actividad académica de la asignatura *Minería de Datos* del Grado en Ingeniería Informática.

## 📂 Sobre el dataset

El conjunto de datos original proviene del portal de calidad del aire del Ayuntamiento de Madrid.  
No se incluye el archivo `.csv` por cuestiones de distribución.

📥 Para reproducir el análisis, ubique el archivo de datos original en el mismo directorio que el notebook principal.  
📊 Fuente de datos: [Datos Madrid – Calidad del Aire](https://datos.madrid.es/)

## 📄 Memoria Técnica

Puedes consultar el informe completo del análisis en el siguiente documento:

📥 [Memoria_Tecnica.pdf](./2_Memoria_Tecnica_carlos_galvez_act2.pdf)
