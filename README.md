# Predicción de Abandono Estudiantil

Proyecto del **Tema 2 — Fundamentos de IA y Machine Learning** del Máster en Data Science de IEBS Business School.

## Descripción

Desarrollo de un modelo de **regresión lineal** para predecir el **riesgo de abandono** de estudiantes (`dropout_risk_score`, escala 0–100) a partir de variables académicas y de comportamiento. El proyecto sigue la metodología **CRISP-DM** e incluye análisis exploratorio (EDA), modelado, evaluación de supuestos y una demostración de inferencia.

## Dataset

`student_dropout_risk_dataset_gaussiannoise.csv` — 733 observaciones y 9 variables (8 explicativas + la variable objetivo).

| Variable | Descripción |
|---|---|
| `age` | Edad del estudiante |
| `GPA` | Nota media (0–10) |
| `attendance` | % de asistencia (0–100) |
| `study_hours` | Horas de estudio semanales |
| `assignment_delay` | Nº de entregas fuera de plazo |
| `platform_usage` | Nivel de uso de la plataforma (0–100) |
| `working_student` | Trabaja mientras estudia (0/1) |
| `scholarship` | Dispone de beca (0/1) |
| `dropout_risk_score` | **Variable objetivo**: riesgo de abandono (0–100) |

## Metodología (CRISP-DM)

1. Comprensión del negocio
2. Comprensión de los datos (EDA)
3. Preparación de los datos
4. Modelado (regresión lineal)
5. Evaluación
6. Despliegue (conceptual, desarrollado en el documento)

## Resultados

- Modelo final: **regresión lineal con 5 variables** (modelo reducido, seleccionado por el **principio de parsimonia**).
- **R² ≈ 0.84** en test, sin sobreajuste (train ≈ test).
- Ausencia de multicolinealidad (VIF ≈ 1).
- Supuestos de **homocedasticidad** y **normalidad de residuos** verificados.

## Ejecución

Abrir el notebook directamente en Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mariosolervidal/Proyecto_Tema2/blob/main/Proyecto2_Fase1.ipynb)

## Tecnologías

Python · pandas · scikit-learn · statsmodels · seaborn · matplotlib · scipy

## Autor

**Mario Soler Vidal** — Máster en Data Science, IEBS Business School.
