# Simulación de Intercambio de Riqueza: Modelo Base vs. Corregido

Este proyecto implementa un modelo probabilístico de transferencia de riqueza para analizar la evolución de la desigualdad en una sociedad artificial. Se incluye la medición del índice de Gini y una propuesta de corrección mediante impuestos, ahorros y redistribución.

## Contenido del Repositorio
- `MM_Tarea1.ipynb`: Notebook con el código fuente, simulaciones y gráficas.
- `datos_finales.csv`: (O el nombre de tu archivo) Resultados de la riqueza final de los agentes.
- `README.md`: Instrucciones y descripción del proyecto.

## Requisitos
Para ejecutar el código es necesario contar con Python 3 y las siguientes librerías:
- `numpy`
- `matplotlib`
- `pandas`
- `scipy`

## Instrucciones de Ejecución
1. Abrir el archivo `MM_Tarea1.ipynb` en Jupyter Notebook o Google Colab.
2. Ejecutar las celdas iniciales para cargar las funciones de simulación y el cálculo del coeficiente de Gini.
3. En la sección "Simulador usuario", ingresar los valores de $N$ (agentes) e $Y$ (interacciones) cuando el programa lo solicite.
4. Las gráficas de Ranking, CCDF y la evolución de Gini se generarán automáticamente al final de cada simulación.

## Descripción del Modelo
- **Modelo Base:** Intercambio aleatorio simple donde la riqueza total se conserva pero tiende a concentrarse en pocos agentes (distribución tipo Gibbs/Exponencial).
- **Modelo Corregido:** Implementa un sistema de impuestos del 20% al top 10% de la población y una redistribución uniforme hacia el 10% más pobre, con el fin de evitar que la riqueza caiga a cero.

## Estadísticas Reportadas
El código calcula automáticamente:
- Media y desviación estándar.
- Porcentaje de agentes en pobreza relativa (riqueza < media/2).
- Participación del top 10% en la riqueza total.
- Evolución temporal del Índice de Gini para comparar la estabilidad de ambos modelos.

## Autores
Sebastián Rodríguez Labastida
