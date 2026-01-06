# 🌍 Clustering de Países para Ayuda Humanitaria (ONG)

![Status](https://img.shields.io/badge/Status-Completado-success)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Visualization](https://img.shields.io/badge/Visualization-Plotly-purple)

## 📋 Descripción del Proyecto
Este proyecto utiliza técnicas de **Machine Learning no supervisado (Clustering)** para categorizar países según factores socioeconómicos y de salud. El objetivo es ayudar a la ONG internacional **"Ayuda Internacional"** a distribuir un fondo de **10 millones de dólares** de manera estratégica y basada en datos.

A través del algoritmo **K-Means**, hemos segmentado 167 países en grupos de prioridad para optimizar la asignación de recursos humanitarios.

## 🎯 Objetivos
*   **Analizar** un dataset global con indicadores económicos (PIB, inflación, ingresos) y de salud (mortalidad infantil, esperanza de vida).
*   **Identificar** patrones ocultos mediante técnicas de agrupación.
*   **Recomendar** una estrategia de inversión priorizando a los países con necesidades más urgentes.

## 🛠️ Tecnologías y Herramientas
*   **Python**: Lenguaje principal.
*   **Pandas & NumPy**: Manipulación y limpieza de datos.
*   **Scikit-learn**: Implementación del algoritmo K-Means, estandarización (StandardScaler) y métricas de evaluación (Silhouette, Davies-Bouldin).
*   **Plotly & Seaborn**: Visualización avanzada interactiva (mapas coropléticos y gráficos 3D).

## 📊 Metodología
1.  **EDA (Análisis Exploratorio):** Detección de outliers y análisis de correlaciones.
2.  **Feature Engineering:** Creación de indicadores sintéticos (*Semántica de Negocio*) para Salud, Comercio y Finanzas.
3.  **Preprocesamiento:** Estandarización de datos con `StandardScaler`.
4.  **Modelado:** Selección del número óptimo de clusters (K=3) basándonos en el *Método del Codo* y criterios de negocio.
5.  **Resultados:** Definición de 3 perfiles de países:
    *   🔴 **Ayuda Urgente:** Alta mortalidad, bajos ingresos.
    *   🟠 **En Desarrollo:** Mortalidad moderada, economía en transición.
    *   🟢 **Autosuficiente:** Altos ingresos, buena salud.

## 📈 Resultados Clave
El modelo recomienda destinar el **70% del presupuesto** a un grupo crítico de países, identificando como máxima prioridad a:
1.  Haití
2.  Sierra Leona
3.  Chad
4.  República Centroafricana
5.  Burkina Faso

### Visualización del Modelo
*(Aquí puedes subir una captura de pantalla de tu mapa interactivo o boxplot y pegarla)*
`![Mapa de Clusters](ruta_de_tu_imagen.png)`

## 📂 Estructura del Repositorio
*   `Feedback_Clustering_Final.ipynb`: Notebook principal con todo el código y análisis.
*   `Country-data.csv`: Dataset original.
*   `mapa_prioridad_ong_interactivo.html`: Mapa mundial interactivo con los resultados.
*   `README.md`: Documentación del proyecto.

## 🚀 Cómo ejecutarlo
1.  Clona el repositorio:
    ```bash
    git clone https://github.com/tu-usuario/clustering-paises-ong.git
    ```
2.  Instala las dependencias:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn plotly
    ```
3.  Ejecuta el notebook en Jupyter o VS Code.

---
*Proyecto realizado como parte del módulo de Técnicas de IA: Clasificaciones y Agrupaciones.*
