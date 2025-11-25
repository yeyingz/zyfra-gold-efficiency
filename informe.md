# Informe Técnico: Predicción de Recuperación de Oro

## 1. Análisis Exploratorio
Se analizó cómo cambia la concentración de metales (Au, Ag, Pb) a través de las etapas de purificación.
* **Oro (Au):** La concentración aumenta progresivamente desde la mezcla inicial hasta el concentrado final, validando la eficiencia del proceso físico-químico actual.
* **Plata (Ag):** La concentración disminuye en las etapas finales, lo cual es esperado ya que se busca purificar el oro.

## 2. Modelado y Evaluación
El desafío principal fue minimizar el sMAPE (Error Porcentual Absoluto Medio Simétrico). 
Se utilizó validación cruzada para ajustar los hiperparámetros.

| Modelo | sMAPE Validación | Observaciones |
| :--- | :--- | :--- |
| Regresión Lineal | Alto (Bajo rendimiento) | No capturó la no-linealidad del proceso químico. |
| **Random Forest** | **Bajo (Optimo)** | Mejor generalización y manejo de ruido en los sensores. |

## 3. Conclusión
El modelo de Random Forest es capaz de predecir la recuperación con un error cercano al 10%, lo cual es aceptable para la toma de decisiones operativas en planta. Esto permitirá a Zyfra optimizar sus procesos y reducir costos operativos significativamente.