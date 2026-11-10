<div align="center">

# 🚛 Mantenimiento Predictivo de Flota Pesada

### Proyecto Final de Data Science

**Análisis de datos reales de operación y mantenimiento de camiones mediante Machine Learning**

<br>

![Python](https://img.shields.io/badge/Python-Data%20Science-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Análisis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

</div>

---

## 📌 Descripción

Este proyecto aborda un **caso real de mantenimiento de flota pesada**, utilizando información histórica de operación y mantenimiento de camiones.

A diferencia de trabajar con un dataset académico preparado previamente, los datos utilizados en este proyecto fueron obtenidos a partir de información operativa real y requirieron un proceso previo de análisis, limpieza, transformación y construcción de variables antes de poder ser utilizados para Machine Learning.

El trabajo recorre distintas etapas de un proyecto de Data Science: desde el entendimiento y preparación de los datos hasta la construcción, evaluación e interpretación de modelos de aprendizaje supervisado y no supervisado.

---

## 🎯 Objetivo

El objetivo general del proyecto es analizar el comportamiento histórico de los equipos de la flota y estudiar hasta qué punto sus características de utilización, antigüedad, consumo e historial de mantenimiento permiten:

- identificar patrones asociados a eventos de mantenimiento;
- construir modelos capaces de estimar la necesidad de mantenimiento;
- descubrir perfiles operativos dentro de la flota;
- obtener información útil para comprender mejor el comportamiento de los equipos.

El proyecto no busca reemplazar el criterio de mantenimiento, sino evaluar cómo las técnicas de **Data Science y Machine Learning** pueden complementar el análisis de información operacional real.

---

## 📊 Dataset

El dataset se construyó a partir de registros históricos de la operación de **camiones de una flota real**.

Cada observación representa el comportamiento de un equipo durante un determinado período e incluye información relacionada con:

- horas de utilización;
- kilómetros recorridos;
- tiempo de operación;
- antigüedad;
- capacidad del equipo;
- consumo;
- historial desde el último evento;
- sistemas asociados a fallas;
- ocurrencia de mantenimiento.

El dataset procesado utilizado para los modelos contiene:

> **7.874 observaciones**

El proceso de construcción del dataset fue una parte fundamental del proyecto, debido a que la información original no estaba diseñada específicamente para entrenar modelos de Machine Learning.

---

## 🔎 1. Análisis Exploratorio de Datos

El primer notebook realiza el **Análisis Exploratorio de Datos (AED)**.

📓 `01_AED_mantenimiento_predictivo_CAMIONES.ipynb`

Durante esta etapa se trabajó sobre:

- estructura general del dataset;
- tipos de variables;
- valores faltantes;
- distribuciones;
- comportamiento de las variables operativas;
- mantenimiento y fallas;
- relaciones entre características;
- preparación y transformación de los datos.

Esta etapa permitió comprender la información disponible y construir un dataset procesado destinado posteriormente al entrenamiento de los modelos.

---

## 🤖 2. Aprendizaje Supervisado

📓 `02_Modelo_Supervisado_CAMIONES.ipynb`

La siguiente etapa estudia el problema como una tarea de **clasificación binaria**.

La variable objetivo indica si una observación requirió o no mantenimiento:

```text
REQUIRIO_MANT

SI → ocurrió un evento de mantenimiento
NO → no ocurrió un evento de mantenimiento