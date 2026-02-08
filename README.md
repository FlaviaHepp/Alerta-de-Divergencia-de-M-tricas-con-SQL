# 🚨Alerta de Divergencia de Métricas con SQL

## 📌Descripción del proyecto

Este proyecto implementa una consulta SQL para la detección automática de divergencias entre métricas, con el objetivo de identificar inconsistencias, desvíos anómalos o posibles errores operativos en procesos de negocio.

La lógica permite generar alertas tempranas cuando una métrica se desvía significativamente respecto a su valor esperado, histórico o de referencia, facilitando tareas de monitoreo, auditoría y control de calidad de datos.

## 🎯Objetivos del proyecto

- Detectar divergencias relevantes entre métricas comparables.
- Automatizar el control de consistencia de datos.
- Reducir el tiempo de detección de errores operativos.
- Proveer una base SQL reutilizable para sistemas de alerta.
- Facilitar la toma de decisiones basada en datos confiables.

## 🏦Contexto de negocio

En entornos corporativos (banca, fintech, retail, operaciones):
- Las métricas deben ser consistentes entre sistemas.

Una divergencia puede indicar:
- Errores de carga (ETL)
- Problemas de integración
- Cambios no documentados en reglas de negocio
- Riesgos operativos o financieros

📌 Este tipo de alertas es clave en áreas de:
 - Riesgo
 - Finanzas
 - BI
 - Data Quality
 - Auditoría interna

## 🧠Lógica de la alerta

La consulta SQL:
- Calcula métricas agregadas relevantes.

Compara valores actuales contra:
- Valores históricos
- Umbrales definidos
- Métricas de referencia
- Calcula la diferencia absoluta y/o porcentual.
- Dispara una alerta cuando la divergencia supera un umbral predefinido.

📌 El enfoque es flexible y adaptable a distintos KPIs.

## 🧪Ejemplo de divergencia detectada

- Diferencia porcentual mayor al X% respecto al valor esperado.
- Incrementos o caídas abruptas en métricas críticas.
- Inconsistencias entre sistemas fuente y destino.

## 🛠️Tecnologías utilizadas

- SQL
- Compatible con:
- PostgreSQL
- MySQL
- SQL Server
- BigQuery (con mínimos ajustes)
- Oracle

## 📁Estructura del proyecto

├── Alerta_de_divergencia.sql
└── README.md

▶️ Cómo utilizar la consulta

Abrir el archivo Alerta_de_divergencia.sql.

Ajustar:
 - Tablas de origen
 - Métricas a comparar
 - Umbrales de divergencia
 - Ejecutar la query en el motor SQL correspondiente.
 - Integrar el resultado con:
 - Dashboards
 - Jobs automáticos
 - Sistemas de notificación (mail, Slack, etc.)

## 🚀Posibles extensiones

- Programar la query como job automático.
- Registrar alertas históricas en una tabla.
- Integrar con herramientas de monitoreo (Airflow, dbt).
- Agregar severidad por nivel de divergencia.
- Visualizar alertas en Power BI / Tableau.

## 👤Autora

Flavia Hepp
Proyecto de análisis y control de datos con SQL orientado a monitoreo y alertas operativas.
