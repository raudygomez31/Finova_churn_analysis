# 🏦 Caso de Estudio: Predicción y Análisis de Churn en FinovaPay

## 1. Introducción y Preguntas de Negocio
> **Contexto:** En el sector de las plataformas de pago y fintech (FinovaPay), la retención de usuarios es un factor crítico para la sostenibilidad del modelo de negocio. Este proyecto analiza el comportamiento de los clientes para identificar patrones de abandono (Churn), evaluar la salud financiera de las cuentas y proponer estrategias basadas en datos para mitigar la fuga de usuarios.

Para guiar esta investigación financiera, nos planteamos resolver las siguientes **Preguntas Clave de Negocio**:
1. **¿Quiénes se están yendo?** ¿Cuáles son las características demográficas, comportamiento transaccional o antiguedad común entre los clientes que deciden abandonar FinovaPay?
2. **¿Existe un detonante financiero?** ¿El saldo en cuenta, el uso de productos financieros (tarjetas, créditos) o el volumen de transacciones mensuales influyen directamente en la tasa de Churn?
3. **¿Cómo segmentar el riesgo?** ¿Cómo podemos clasificar a los usuarios para que el equipo de Customer Success aplique campañas de retención antes de que abandonen la plataforma?

---

## 2. Metodología de Resolución: ¿Cómo Procedimos? (Paso a Paso)

Para resolver este desafío de extremo a extremo, estructuramos un pipeline de datos combinando tres herramientas esenciales:

### 📑 Paso 1: Auditoría e Ingesta de Datos con Excel
* **El Enfoque:** Utilizamos hojas de cálculo para realizar una primera inspección del dataset original de FinovaPay. Evaluamos la estructura de las filas, identificamos la presencia de valores nulos o registros duplicados y aseguramos que los formatos de las variables clave (IDs de cliente, saldos y banderas de Churn) estuvieran listos para su procesamiento técnico.

### 🐍 Paso 2: Análisis Exploratorio y Feature Engineering con Python
Llevamos el dataset limpio a Python para profundizar en el comportamiento de los datos mediante código:
* **Análisis Exploratorio (EDA):** Utilizamos librerías para calcular las correlaciones entre las variables financieras y la variable objetivo (`Churn`).
* **Ingeniería de Características:** Agrupamos y transformamos métricas transaccionales para aislar el comportamiento de los usuarios activos frente a los inactivos, preparando los datos para responder a las necesidades del negocio.

### 🛢️ Paso 3: Consultas Avanzadas y Segmentación con SQL
Migramos el set de datos transformado a un entorno de base de datos relacional para realizar la explotación de datos mediante queries estructuradas:
* **Explotación de Datos:** Diseñamos consultas optimizadas (`SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`) para segmentar a los usuarios por niveles de riesgo, calcular tasas de abandono agregadas por tipo de cuenta y extraer listas específicas de clientes con alta probabilidad de fuga.

---

## 3. Conclusiones y Plan de Acción Directiva

1. **Estrategia Preventiva Activa:** Implementar alertas automatizadas basadas en los patrones transaccionales identificados en Python y SQL para detectar usuarios que disminuyen drásticamente su actividad antes de que ocurra el Churn definitivo.
2. **Fidelización Basada en Segmentos:** Diseñar campañas de marketing dirigidas y beneficios exclusivos para los segmentos de usuarios más vulnerables y de mayor valor financiero detectados durante el análisis.

---

## 🔗 Enlaces y Recursos del Proyecto

### 📂 Repositorio de Código y Datos de FinovaPay
* [Ver Archivo de Datos en Excel](./Proyecto_churn_Finovapay.xlsx) 
* [Ver Script de Consultas SQL FinovaPay](./consultas_clientes.sql) 
* [Ver Notebook de Análisis en Python](./Untitled2.ipynb)
