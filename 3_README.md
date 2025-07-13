# Boston_Housing_Regression  
#PREDICCIÓN DEL PRECIO DE VIVIENDAS EN BOSTON CON MODELOS DE REGRESIÓN

Este repositorio contiene un análisis completo sobre el conjunto de datos de viviendas en Boston, enfocado en la predicción del precio medio por vivienda. Se han aplicado diferentes modelos de regresión (simple, múltiple y árboles de regresión) para evaluar su capacidad predictiva y compararlos en cuanto a precisión y comportamiento.

## 📊 Tecnologías utilizadas

- Python 3  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Seaborn  

## 📁 Estructura

- `regresion_boston.ipynb`: Notebook principal con todo el flujo de trabajo de análisis y modelado.
- `Memoria_Tecnica.pdf`: Informe en PDF con el desarrollo completo, explicaciones, gráficas y conclusiones.

## 📌 Objetivo

Predecir el precio medio de una vivienda (`MEDV`) a partir de variables estructurales, geográficas y socioeconómicas del entorno, tales como el número medio de habitaciones (`RM`), la proporción de población de bajos ingresos (`LSTAT`), el índice de accesibilidad a carreteras (`RAD`), entre otras.

## 🧠 Modelos aplicados

- **Regresión lineal simple**: utilizando únicamente la variable `RM`.  
- **Regresión lineal múltiple**: incorporando todas las variables explicativas.  
- **Árbol de regresión**: modelo no lineal capaz de capturar patrones complejos.  
- Se incluye además un árbol limitado en profundidad para evitar sobreajuste.

## 📈 Resultados clave

- La regresión lineal simple muestra una tendencia positiva clara pero con baja capacidad explicativa (R² ≈ 0.37).
- La regresión múltiple mejora significativamente la precisión (R² ≈ 0.67).
- El árbol de regresión obtiene el mejor rendimiento (R² ≈ 0.86) y menor error cuadrático medio.
- Se analiza el riesgo de sobreajuste y se propone limitar la profundidad del árbol como medida de regularización.

## 📊 Visualizaciones

El proyecto incluye gráficos como:
- Diagramas de dispersión entre variables clave y precio (`RM` vs `MEDV`, `LSTAT` vs `MEDV`)
- Mapas de calor con correlaciones entre variables
- Gráficos de regresión ajustada
- Visualización del árbol de decisión

## 🧑‍💻 Autor

Carlos Gálvez

> Proyecto realizado con fines de práctica y desarrollo profesional en técnicas de análisis predictivo.

## 📂 Sobre el dataset

El conjunto de datos original proviene de la base de datos clásica "Boston Housing", incluida en versiones anteriores de Scikit-learn.  
Actualmente no se encuentra disponible directamente desde `load_boston()` por cuestiones éticas, pero puede descargarse desde repositorios de datasets públicos para replicar el análisis.

📝 Fuente sugerida para el dataset: [Boston Housing en Kaggle](https://www.kaggle.com/datasets/altavish/boston-housing-dataset)

## 📄 Memoria Técnica

Puedes consultar el informe completo del análisis aquí:

📥 [act3_Carlos_Galvez_Reguera.pdf](./3_Carlos_Galvez_Reguera_act3.pdf)
📥 [codigo python ](./3_regresion_boston.ipynb)
