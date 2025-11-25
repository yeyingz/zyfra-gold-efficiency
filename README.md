# Zyfra: Optimización de Recuperación de Oro con Machine Learning 🏭⚗️

![Status](https://img.shields.io/badge/Status-Completed-success)
![Python](https://img.shields.io/badge/Python-3.9-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)

## 💼 Resumen Ejecutivo
En la industria minera, la eficiencia lo es todo. Este proyecto fue desarrollado para **Zyfra** con el objetivo de desarrollar un prototipo de modelo de Machine Learning que prediga la cantidad de oro recuperado del mineral. 

**¿El valor de negocio?** El modelo permite optimizar la producción detectando parámetros no rentables antes de procesar el material, ahorrando costes operativos y maximizando el rendimiento del oro puro.

---

## 🛠️ Tecnologías Utilizadas
* **Python**: Pandas, NumPy.
* **Machine Learning**: Scikit-learn (RandomForestRegressor, LinearRegression).
* **Métrica de Negocio**: sMAPE (Symmetric Mean Absolute Percentage Error).
* **Visualización**: Matplotlib, Seaborn.

## 📊 Metodología (Pipeline)

1.  **Preprocesamiento Industrial**: Manejo de datos de concentraciones de metales (Au, Ag, Pb) en diferentes etapas de purificación (Flotación -> Primaria -> Final).
2.  **Análisis de Anomalías**: Detección de outliers en la alimentación de materia prima que podrían sesgar el modelo.
3.  **Métrica Personalizada (sMAPE)**: Implementación de una función de error porcentual simétrico para evaluar la precisión tanto en la etapa de 'rougher' como en la 'final'.
4.  **Selección de Modelo**: Comparación entre Regresión Lineal y Bosques Aleatorios.
    * *Ganador:* **Random Forest Regressor**.

## 📈 Resultados Clave
El modelo final alcanzó un **sMAPE ponderado del 10.79%** en el conjunto de prueba. Esto indica una alta fiabilidad para predecir la recuperación de oro en condiciones reales, permitiendo a la planta ajustar los parámetros de flotación y purificación con antelación.

## 🚀 Cómo ejecutar este proyecto

1.  Clonar el repositorio:
    ```bash
    git clone [https://github.com/yeyingz/zyfra-gold-efficiency.git](https://github.com/yeyingz/zyfra-gold-efficiency.git)
    ```
2.  Instalar dependencias:
    ```bash
    pip install -r requirements.txt
    ```
3.  Explorar el notebook.

---
*Desarrollado por [Aurelio González](https://www.linkedin.com/in/aureliogonzalez-datascientist)*