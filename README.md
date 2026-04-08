# 📊 Retail Analytics Pipeline con Apache Spark

## 🚀 Descripción del proyecto

Este proyecto desarrolla un pipeline completo de análisis de datos para una empresa de e-commerce ficticia (**RetailMax**), utilizando tecnologías de Big Data como **Apache Spark**.

El objetivo es procesar grandes volúmenes de datos, generar métricas de negocio y aplicar modelos de Machine Learning escalables para obtener insights relevantes para el área de marketing.

---

## 🎯 Objetivo

Diseñar e implementar un pipeline de Big Data capaz de:

* Procesar datos estructurados y no estructurados
* Ejecutar transformaciones masivas
* Generar métricas de negocio
* Aplicar modelos de Machine Learning escalables con Spark MLlib

---

## 🧠 Tecnologías utilizadas

* Python
* Apache Spark (PySpark)
* Spark SQL
* Spark MLlib
* Pandas
* PyArrow
* Matplotlib (opcional)

---

## 🔄 Pipeline de datos

```text
[Fuentes de datos: Transacciones | Reseñas | Navegación]
        ↓
[Ingesta de datos]
        ↓
[Procesamiento distribuido (Spark)]
        ↓
[Análisis (Spark SQL)]
        ↓
[Machine Learning (MLlib)]
        ↓
[Exportación de datos (Parquet)]
```

---

## 📂 Estructura del proyecto

```text
retail-analytics-pipeline/
│
├── notebook.ipynb
├── data/
│   └── ventas.parquet
├── outputs/
│   └── resultados.csv
└── README.md
```

---

## 📊 Procesamiento de datos

* Creación y manipulación de RDDs
* Transformaciones (map, filter, flatMap, distinct, sortBy)
* Acciones (count, collect, mean, stdev)
* Conversión a DataFrames
* Consultas con Spark SQL

---

## 🤖 Machine Learning

Se implementaron modelos utilizando Spark MLlib:

* Regresión Logística (supervisado)
* K-Means (no supervisado)

Estos modelos permiten clasificar usuarios y segmentar comportamientos para apoyar decisiones de marketing.

---

## 💾 Exportación de datos

Los resultados se almacenan en formato **Parquet**, optimizado para entornos Big Data.

Debido a limitaciones del entorno local en Windows, la exportación se realizó utilizando Pandas:

```python
df.toPandas().to_parquet("ventas.parquet")
```

---

## ⚠️ Limitaciones

* Ejecución en entorno local (no distribuido real)
* Problemas de compatibilidad de Spark con Windows para escritura en Parquet
* Uso de Pandas como alternativa para exportación

---

## 🔮 Mejoras futuras

* Implementación en entorno distribuido (cluster o nube)
* Uso de almacenamiento en Data Lake (S3, Azure, GCP)
* Optimización con particionado y caching
* Visualización avanzada de datos
* Automatización del pipeline

---

## 💼 Aplicación profesional

Este proyecto demuestra habilidades en:

* Procesamiento de datos a gran escala
* Uso de Apache Spark
* Desarrollo de pipelines de datos
* Aplicación de Machine Learning en Big Data

---

## 👤 Autor

Manuel Quintana


---

## 📌 Nota

Este proyecto fue desarrollado como parte del programa de formación en Ciencia de Datos de Talento Digital (SENCE).
