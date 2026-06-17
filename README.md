# 📊 Análisis de Inversión Inmobiliaria - Airbnb Buenos Aires

Este proyecto contiene el pipeline de análisis de datos desarrollado para evaluar el mercado de alquileres temporales de Airbnb en la Ciudad Autónoma de Buenos Aires (CABA). El objetivo es procesar métricas clave de oferta, ocupación y rendimiento financiero para identificar oportunidades de inversión estratégicas según diferentes perfiles de riesgo.

---

## 📁 1. Estructura del Proyecto

El repositorio está organizado de manera modular para garantizar la reproducibilidad del análisis desde cero:

* **01_Data_Raw/**: Datasets crudos de origen sin modificar (listings.csv, calendar.csv, reviews.csv).
* **02_Notebooks/**: Scripts ejecutables de Jupyter (01_Data_Cleaning.ipynb).
* **03_Data_Processed/**: Archivos limpios generados por el código (listings_cleaned.csv, calendar_cleaned.csv, reviews_cleaned.csv).
* **04_Dashboards/**: Capa de visualización de negocio (Archivo original de Power BI / Link a Reporte).

---

## ⚙️ 2. Ejecución del Notebooks

Para replicar el análisis completo, los archivos de la carpeta `02_Notebooks/` deben ejecutarse en el siguiente orden secuencial:

### `01_Data_Cleaning.ipynb`
* **Función:** Este script toma los datos crudos y realiza el proceso de extracción y transformación (ETL).
* **Procesos clave:** Normaliza tipos de datos en variables críticas (habitaciones, baños, precios), maneja nulos y utiliza bucles (loops) para filtrar e identificar outliers (valores atípicos).
* **Resultado:** Genera el archivo optimizado `listings_cleaned.csv`, `calendar_cleaned.csv`, `reviews_cleaned.csv`.

---

## 🚀 3. Guía de Reproducción (Paso a Paso)

1. Descargue o clone este repositorio en su máquina local.
2. Asegúrese de tener instalado Python y las librerías: `pandas`, `numpy` y `jupyter`.
3. Ejecute por completo el archivo `01_Data_Cleaning.ipynb` para procesar los datos crudos.
4. Abra el archivo del Dashboard en Power BI y haga clic en **"Actualizar"** para refrescar automáticamente todos los gráficos interactivos.
