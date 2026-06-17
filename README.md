# EcoModelo: Calibración de Sucesión Poblacional mediante Backtracking

Proyecto final para la asignatura de Introducción a las Ciencias de la Computación de la Universidad Nacional de Colombia, Sede Manizales.

## Contributors
* Juan Sebastian Yepez
* Juan Sebastian Pardo
* Simon Ospina Gomez

## Descripción del Proyecto
Este repositorio contiene la implementación en Python de un algoritmo de **backtracking con poda** diseñado para calibrar un modelo matemático de crecimiento poblacional logístico discreto. El objetivo es explorar combinaciones de parámetros (tasa de crecimiento `r` y capacidad de carga `K`) para encontrar la que mejor explique una serie de datos observados.

A diferencia de una búsqueda exhaustiva ciega, el algoritmo implementa técnicas de poda para optimizar el cómputo: 
- **Restricción Física:** Retrocede inmediatamente si la combinación produce valores biológicamente imposibles (población negativa).
- **Restricción de Eficiencia:** Corta la simulación si el error acumulado parcial ya supera al mejor error total conocido hasta el momento.

## Estructura del Repositorio
* `EcoModelo_Backtracking.ipynb`: Código fuente ejecutable con el algoritmo y visualización de resultados.
* `Informe_EcoModelo.pdf`: Explicación del modelamiento matemático y ejemplo de poda manual.
* `Presentacion_EcoModelo.pdf`: Diapositivas de soporte para la exposición oral.

## 🚀 Cómo ejecutar
1. Abrir el archivo `.ipynb` en Google Colab o Jupyter Notebook.
2. Ejecutar toda la celda
3. El output final mostrará los mejores parámetros calibrados, la comparativa de eficiencia vs fuerza bruta, y la gráfica de ajuste poblacional.
