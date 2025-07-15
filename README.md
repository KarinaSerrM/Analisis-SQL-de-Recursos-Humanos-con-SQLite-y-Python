# Análisis SQL de Recursos Humanos con SQLite y Python

Este repositorio documenta un proyecto de análisis de datos laborales a partir de un archivo CSV integrado en SQLite. Mediante consultas SQL, se exploran métricas clave como satisfacción, salario, horas trabajadas y accidentes laborales, utilizando Python para importar y visualizar datos.

## Objetivo

Desarrollar consultas SQL eficientes que permitan ordenar, agrupar y calcular métricas relevantes sobre los empleados, utilizando un entorno ligero con SQLite y pandas.

## Flujo de trabajo

### 1. Preparación de datos
- Creación del archivo `RH.db` como base de datos local
- Definición de la tabla `Detalle` con columnas completas
- Importación de datos desde `detalle.csv` con `pandas` y `sqlite3`

### 2. Consultas clave

- Cálculo del promedio de `satisfaction_level` general
- Agrupamiento por variable `left` (salida del empleado) con promedios asociados
- Promedio de `average_monthly_hours` para salarios “low” y “medium”
- Filtrado de empleados con `promotion_last_5years = 1 AND left = 1`
- Ordenamiento por `department` y salario con títulos añadidos para visualización
- Ejemplo teórico con uso de `HAVING` para detectar departamentos con más de 200 accidentes

### 3. Organización visual
- Inclusión de títulos en las visualizaciones
- Orden estructurado de salidas y agrupaciones
- Explicación clara del uso de `HAVING` para filtros condicionales

## Herramientas utilizadas

- Python 3.x  
- pandas  
- sqlite3  
- Jupyter Notebook  
- SQLiteStudio (opcional para inspección gráfica)

## Conclusiones

- La integración entre Python y SQLite permite estructurar bases de datos desde archivos CSV de forma rápida.
- Las cláusulas `GROUP BY` y `HAVING` enriquecen el análisis segmentado.
- El manejo visual mediante títulos y ordenamiento mejora la claridad de resultados.
- Este proyecto es ideal para entornos donde se requiere análisis ligero sin bases de datos externas.
