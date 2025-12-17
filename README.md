# Análisis de eficiencia operativa y satisfacción en retail con NLP

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-150458)
![Status](https://img.shields.io/badge/Status-Completed-success)

## Descripción del Proyecto

Este proyecto aplica técnicas de **Ciencia de Datos y Procesamiento de Lenguaje Natural (NLP)** para analizar encuestas operativas de líderes de zona en el sector Retail. El objetivo principal fue transformar **28 preguntas abiertas (datos no estructurados)** en **indicadores cuantitativos (KPIs)** para medir la fricción operativa, identificar cuellos de botella y proyectar el impacto financiero de la ineficiencia administrativa.

El análisis permite pasar de opiniones subjetivas ("siento que pierdo tiempo") a datos accionables ("el 28% de las horas hombre se pierden en procesos manuales de nómina").

## Objetivos del Análisis

1.  **Cuantificar el "Esfuerzo sin Valor":** Identificar qué tareas consumen más tiempo del líder sin aportar al negocio.
2.  **Mapeo de Prioridades:** Entender la brecha entre lo que la empresa pide (Estrategia) y lo que el líder ejecuta (Realidad).
3.  **Detección de Automatización:** Encontrar candidatos perfectos para RPA (Automatización Robótica de Procesos).
4.  **Span of Control:** Determinar la carga óptima de tiendas por líder basada en la voz del experto.

##  Metodología y Stack Tecnológico

El proyecto fue desarrollado en **Python** utilizando Google Colab.

* **Librerías:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `re` (Expresiones Regulares), `unicodedata`.
* **Técnicas de NLP aplicadas:**
    * **Data Wrangling:** Limpieza de ruido, normalización de texto y eliminación de stopwords.
    * **Pattern Matching (Regex):** Segmentación semántica de respuestas complejas (ej. separar "Lo urgente" de "Lo que se aplaza").
    * **Categorización basada en Reglas:** Algoritmos de clasificación por palabras clave contextuales para agrupar dolores operativos (TimeSoft, COA, Burocracia).
    * **Análisis de Frecuencia:** Identificación de tendencias mediante N-gramas.

##  Principales Insights (Resultados)

Tras procesar la data, se generaron las siguientes categorías de análisis:

### 1. Fricción Operativa (Pain Points)
Se detectó que las tareas de **Gestión de Nómina (TimeSoft)** y **Auditorías (COA)** son las mayores generadoras de esfuerzo sin valor percibido.
* *Acción sugerida:* Revisión de UX de la herramienta de nómina y automatización de reportes de auditoría.

### 2. Matriz de Priorización
Mediante la segmentación de texto, se identificó que las tareas **Administrativas y de Correo** son las primeras en ser sacrificadas/aplazadas cuando la operación se complica, lo que genera un riesgo de cumplimiento normativo.

### 3. Oportunidades de Automatización
El análisis reveló que el **30%+ de las solicitudes de automatización** se concentran en reportes manuales y consolidación de Excel, lo que justifica la inversión en dashboards de BI centralizados.

### 4. Span of Control (Carga Laboral)
El análisis numérico extraído del texto sugiere que el número de tiendas por líder para mantener la calidad operativa es **7-8 tiendas**. Superar este número diluye la supervisión efectiva en la cargo de jefe de zona.

##  Impacto Financiero (Modelo de ROI)

Este análisis sirve como base para calcular el costo de la ineficiencia:

$$\text{Costo Anual Ineficiencia} = (\text{Horas/Semana en Tareas "Sin Valor"}) \times (\text{Costo Hora Líder}) \times (\text{Nº Líderes}) \times 52$$

*Este modelo permite justificar inversiones en tecnología comparando el costo del desarrollo vs. el ahorro en horas-hombre recuperadas para la venta.*

##  Estructura del Repositorio

* `/notebooks`: Scripts de Python con el paso a paso del procesamiento (ETL y NLP).
* `/data`: (Anonimizado) Muestra de la estructura de datos utilizada.
* `/results`: Gráficos generados en Power BI y archivo Excel categorizados y anonimizado.

##  Contacto

Si te interesa saber más sobre cómo aplicar NLP para optimizar operaciones masivas, contáctame en www.linkedin.com/in/jorge-restrepo-alvarez-analisis-datos

---
