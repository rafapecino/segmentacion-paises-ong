# 🌍 Clustering de Países para Ayuda Humanitaria (ONG)

![Estado del Proyecto](https://img.shields.io/badge/Estado-Completado-green)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Librerías](https://img.shields.io/badge/Librerías-Scikit--Learn%20%7C%20Pandas%20%7C%20Plotly-yellow)

## 📋 Descripción del Proyecto

Este proyecto colabora con la ONG internacional **"Ayuda Internacional"** para optimizar la distribución estratégica de un fondo de **10 millones de dólares**.

El objetivo es utilizar técnicas de **Machine Learning no supervisado (Clustering)** para categorizar 167 países basándonos en factores socioeconómicos y de salud. Esto permite identificar de manera objetiva y basada en datos qué naciones se encuentran en una situación más crítica y requieren ayuda prioritaria.

## 🎯 Objetivos

*   **Segmentar países** utilizando indicadores macroeconómicos y de salud (mortalidad infantil, PIB, esperanza de vida, etc.).
*   **Identificar grupos prioritarios** que necesiten asistencia urgente.
*   **Optimizar la asignación de recursos** del fondo humanitario de la ONG.

## 🗂️ Estructura del Dataset

El análisis se basa en un dataset con **167 registros** y **10 variables** clave:

| Variable | Descripción |
| :--- | :--- |
| `country` | Nombre del país. |
| `child_mort` | Muertes de niños menores de 5 años por cada 1000 nacidos. |
| `exports` | Exportaciones per cápita (% del PIB). |
| `health` | Gasto total en salud per cápita (% del PIB). |
| `imports` | Importaciones per cápita (% del PIB). |
| `income` | Ingreso neto por persona. |
| `inflation` | Tasa de crecimiento anual del PIB total. |
| `life_expec` | Esperanza de vida promedio al nacer. |
| `total_fer` | Tasa de fertilidad (hijos por mujer). |
| `gdpp` | PIB per cápita. |

## 🛠️ Metodología

1.  **Análisis Exploratorio de Datos (EDA):**
    *   Análisis de distribuciones y detección de outliers.
    *   Matriz de correlación para entender relaciones entre variables (ej. alta correlación entre `income` y `gdpp`).
2.  **Preprocesamiento:**
    *   Escalado de datos (StandardScaler) para normalizar rangos de variables dispares.
3.  **Modelado (K-Means Clustering):**
    *   Uso del **Método del Codo (Elbow Method)** y **Puntuación de Silueta** para determinar el número óptimo de clusters.
    *   Segmentación final en **3 grupos principales**.
4.  **Interpretación y Perfilado:**
    *   Análisis de las características promedio de cada cluster para asignar etiquetas ("Desarrollados", "En desarrollo", "Subdesarrollados/Prioritarios").

## 📊 Resultados Clave

Se han identificado tres perfiles claros de países:

*   🔴 **Cluster 0 (Prioridad Alta):** Países con alta mortalidad infantil, bajo PIB y baja esperanza de vida. Requieren la mayor parte de la ayuda.
*   🟡 **Cluster 1 (En Transición):** Países con indicadores medios.
*   🟢 **Cluster 2 (Desarrollados):** Países con altos ingresos y buenos indicadores de salud. No requieren ayuda urgente.

## 🚀 Cómo ejecutar el proyecto

1.  Clona el repositorio:
    ```bash
    git clone https://github.com/rafapcino/segmentacion-paises-ong.git
    ```
2.  Instala las dependencias necesarias:
    ```bash
    pip install pandas numpy matplotlib seaborn plotly scikit-learn
    ```
3.  Ejecuta el notebook en Jupyter o VS Code:
    ```bash
    jupyter notebook Feedback_Clustering_Rafael_Pecino.ipynb
    ```

## 👤 Autor

**Rafael Pecino**
*   Análisis de Datos y Machine Learning
