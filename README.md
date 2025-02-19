# E-Commerce_Challenge

Este repositorio contiene un análisis completo de datos ficticios de un eCommerce correspondiente al año 2013. Se aborda el desafío técnico a través de un proceso de **limpieza**, **transformación**, **análisis de conversión**, **time lag entre compras** y **segmentación de clientes** utilizando la metodología **RFM** (Recency, Frequency, Monetary) combinada con técnicas de *clustering* (K-Means).

---

## Estructura del Repositorio

- **datasets/**  
  Carpeta que contiene los archivos CSV necesarios para el análisis:
  - `Hendylaset - ordenes.csv`
  - `Hendylaset - cart-items.csv`

- **E-commerce_Analysis.ipynb**  
  Notebook principal en el que se realiza todo el proceso:
  - Limpieza y transformación de datos (tipos, valores nulos, normalización).
  - Análisis de conversión y cálculo de métricas (incluyendo un análisis del funnel de conversión y cálculo del time lag entre compras).
  - Segmentación de clientes mediante la metodología RFM y aplicación de clustering (K-Means), con justificación basada en el Método del Codo y Silhouette Score.
  - Visualizaciones interactivas y estáticas utilizando Plotly, Seaborn y Matplotlib.

- **README.md**  
  Este documento, que describe el proyecto y su estructura.

---

## Descripción General del Proyecto

El proyecto se desarrolló para resolver un desafío técnico con los siguientes objetivos:

- **Limpieza y Transformación de Datos:**  
  Conversión de tipos de datos, imputación de valores nulos, normalización y validación de columnas.

- **Time Lag entre Compras:**  
  Cálculo de la diferencia en días entre órdenes consecutivas para cada usuario, permitiendo identificar comportamientos de recompra.

- **Conversión de Carritos:**  
  Cálculo y análisis de la tasa de conversión global en el proceso de compra, explorando cada etapa del funnel (desde la creación del carrito hasta la entrega).

- **Segmentación de Clientes:**  
  Aplicación de la metodología RFM para extraer métricas clave (recency, frequency, monetary) y, posteriormente, la aplicación de clustering con K-Means para identificar segmentos diferenciados de clientes. Se incluye la justificación de la elección del número de clusters mediante el Método del Codo y el Silhouette Score.

---

## Cómo Ejecutar el Proyecto

1. **Requisitos:**
   - Python 3.8+  
   - Librerías: pandas, numpy, matplotlib, seaborn, sqlite3, scikit-learn, plotly  
     

2. **Ejecución:**
   - Clona el repositorio.
   - Asegúrate de que los archivos CSV estén en la carpeta `datasets/`.
   - Abre el notebook `E-commerce_Analysis.ipynb` en Jupyter Notebook o JupyterLab.
   - Ejecuta todas las celdas para reproducir el análisis completo.

---

## Resultados e Insights

- **Análisis de Time Lag:**  
  Se ha calculado la diferencia de días entre compras consecutivas, permitiendo entender el comportamiento de recompra de los clientes.

- **Conversión de Carritos:**  
  Se analiza la tasa de conversión global y se identifican puntos de mejora en el proceso de compra.

- **Segmentación de Clientes:**  
  Se realiza una segmentación basada en las métricas RFM y se aplican 5 clusters, cuya elección se justifica con técnicas estadísticas (Elbow Method y Silhouette Score). Los segmentos se etiquetan de la siguiente manera (ordenados de mayor a menor composite_score):
  - **Mejores clientes**
  - **Cliente Leal**
  - **Cliente Prometedor**
  - **Clientes que Necesitan Atención**
  - **Cliente Perdido**

---

## Conclusiones y Próximos Pasos

El análisis permite:
- Identificar segmentos con oportunidades para estrategias de retención y fidelización.
- Detectar posibles cuellos de botella en el proceso de conversión de carritos.
- Proponer mejoras basadas en insights derivados de los datos.

**Futuros desarrollos:**
- Integración de más variables y fuentes de datos para enriquecer el análisis.
- Profundización en la comparación con benchmarks de la industria.
- Automatización de reportes e integración en dashboards interactivos.

---

