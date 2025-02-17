# E-Commerce_Challenge

Este repositorio contiene un análisis de datos ficticios de un eCommerce para el año 2013, enfocado en **limpieza**, **transformación**, **análisis de conversión**, **time lag** entre compras y **segmentación de clientes** con la metodología **RFM** (Recency, Frequency, Monetary).

## Estructura del Repositorio


### 1. `datasets/`
Contiene los archivos CSV necesarios para el análisis:

- **Hendylaset - ordenes.csv**
- **Hendylaset - cart-items.csv**

### 2. `E-commerce_Analysis.ipynb`
Notebook principal donde se lleva a cabo el **proceso de limpieza**, **transformación** y **análisis** de los datos.  
Incluye **visualizaciones** con librerías como Plotly y Seaborn, y **ejecución de consultas SQL** en memoria (SQLite).

### 3. `README.md`
Este documento con una descripción general del proyecto.

---

## Descripción General

En este proyecto se aborda un desafío con los siguientes objetivos:

- **Limpieza y Transformación de Datos**  
  Conversión de tipos, manejo de valores nulos, normalización y validación de columnas.

- **Time Lag entre Compras**  
  Cálculo de la diferencia en días entre órdenes consecutivas de cada usuario.

- **Conversión de Carritos**  
  Cálculo de la tasa de conversión global y análisis de cada etapa del funnel (mail, warehouse, etc.).

- **Segmentación de Clientes**  
  Aplicación de la metodología RFM y *clustering* K-Means para identificar grupos de clientes con comportamientos de compra similares.
