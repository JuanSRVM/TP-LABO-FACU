# TP-LABO-FACU

# Estimación del costo de equipar un gimnasio mediante análisis de datos de comercio electrónico (2024–2025)

## Trabajo Práctico Grupal

**Laboratorio de Métodos Cuantitativos Aplicados a la Gestión**
Tecnicatura Universitaria en Gestión y Análisis de Datos en Organizaciones
Facultad de Ciencias Económicas – Universidad de Buenos Aires
Primer Cuatrimestre 2026

### Integrantes

* Damián Ariel Larrosa
* Juan Sebastián Vallone
* Lautaro Caprile

---

## Resumen

El presente trabajo tiene como objetivo aplicar técnicas de exploración, transformación, análisis y visualización de datos sobre un conjunto masivo de transacciones de comercio electrónico. A partir de un dataset con aproximadamente un millón de registros correspondientes al período 2024–2026, se desarrolla un análisis orientado a estimar el costo de equipar un gimnasio utilizando productos comercializados dentro de las categorías Sports y Health.

Para ello se realizaron procesos de limpieza y filtrado de datos, análisis estadísticos descriptivos, agrupaciones mediante Pandas, visualizaciones desarrolladas con Matplotlib y Seaborn, y una aplicación de conceptos de costo, ingreso, beneficio y punto de equilibrio estudiados en la materia.

---

## Pregunta de investigación

**¿Cuál sería el costo estimado de equipar un gimnasio utilizando productos de las categorías Sports y Health comercializados durante los años 2024 y 2025?**

Esta pregunta permite aproximar una inversión inicial utilizando precios observados en transacciones reales de comercio electrónico, aportando una referencia basada en evidencia para la adquisición de equipamiento y accesorios relacionados con la actividad física.

---

## Dataset utilizado

**Global E-Commerce Dataset (2024–2026)**

Fuente:

https://www.kaggle.com/datasets/akrambelha/global-e-commerce-dataset-1m-records-20242026

El dataset contiene información sobre órdenes de compra, productos, categorías, precios, costos, ganancias, reseñas y otros indicadores vinculados a operaciones de comercio electrónico a nivel global.

---

## Metodología

El análisis se desarrolló en Python utilizando Google Colab y se estructuró en cinco etapas principales:

### 1. Exploración inicial

Se examinó la estructura general del dataset mediante:

* Dimensiones del conjunto de datos.
* Tipos de variables.
* Valores faltantes.
* Registros duplicados.
* Estadísticas descriptivas.

### 2. Transformación de datos

Se aplicaron filtros para conservar únicamente:

* Productos pertenecientes a las categorías **Sports** y **Health**.
* Órdenes con estado **Completed**.
* Transacciones correspondientes a los años **2024** y **2025**.

Posteriormente se seleccionaron productos considerados relevantes para el equipamiento y funcionamiento habitual de un gimnasio.

### 3. Análisis estadístico

Se calcularon indicadores agrupados por producto, subcategoría y período temporal, incluyendo:

Cantidad de ventas.
Precio promedio.
Ingresos totales.
Ganancia total.
Evolución anual de las ventas.

### 4. Visualización de datos

Se desarrollaron distintos gráficos para analizar:

 * Distribución de precios por subcategoría.
 * Comparación entre marcas y segmentos de mercado.
 * Evolución temporal de precios.
 * Relación entre variables relevantes para la toma de decisiones.

### 5. Aplicación de conceptos de la materia

Con el objetivo de complementar el análisis descriptivo y responder a la pregunta de investigación, se implementó una función en Python que calcula indicadores económicos y de rentabilidad para cada sub-categoría de productos.

La función agrupa la información por sub-categoría y calcula:

* **Cantidad total vendida (Q)**.
* **Ingreso Total (IT)**.
* **Costo Total (CT)**.
* **Beneficio**.
* **Margen de rentabilidad (%)**.
* **Precio promedio por unidad**.
* **Costo promedio por unidad**.
* **Costos fijos estimados (CF)**.
* **Punto de equilibrio en unidades (Q*)**.

A partir de estos indicadores se construyó una tabla resumen y una visualización comparando ingresos, costos y beneficios por sub-categoría.

### Supuesto para el punto de equilibrio

El dataset utilizado no diferencia explícitamente entre costos fijos y costos variables. Por este motivo, y únicamente con fines ilustrativos, se asumió que los costos fijos representan el 20% del costo total de cada sub-categoría.

Este supuesto permite estimar el punto de equilibrio mediante la fórmula:

**Q* = CF / (Precio Promedio − Costo Promedio)**

Los resultados obtenidos permiten identificar qué tipos de productos generan mayores beneficios y cuáles requieren menores volúmenes de venta para cubrir sus costos estimados.



---

## Herramientas utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* KaggleHub
* Google Colab
* GitHub

---

## Uso de Inteligencia Artificial



---

## Conclusiones

