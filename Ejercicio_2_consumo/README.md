# Prueba Técnica - Tuya

## Ejercicio 2: Preferencias de Consumo

Este repositorio contiene la solución al segundo ejercicio de la prueba técnica de Tuya. El objetivo principal es identificar las categorías de consumo preferidas por los clientes con base en sus transacciones aprobadas dentro de un rango de fechas configurable.

---

## Objetivo

- Cargar y estructurar información proveniente de un archivo Excel.
- Crear y poblar una base de datos SQLite con los datos.
- Ejecutar una consulta SQL que:
  - Filtre las transacciones aprobadas dentro de un rango de fechas.
  - Cuente las transacciones por categoría y cliente.
  - Identifique las categorías más relevantes para cada cliente usando funciones de ventana.
  - Devuelva las categorías más preferidas por cliente según el número de transacciones y la fecha más reciente.

---

## Tecnologías utilizadas

- **Python 3**
- **SQLite**
- **Pandas**
- **Google Colab** (entorno de ejecución)
- **psycopg2** (instalado por compatibilidad, pero no se usa en SQLite)

---

## Estructura del Proyecto

- `bd.xlsx`: Archivo de entrada con las hojas CLIENTES, TRANSACCIONES y CATEGORIAS_CONSUMO.
- `base_de_datos.db`: Base de datos generada a partir de los datos del Excel.
- `script_sqlite_consumo.py`: Script principal con todo el proceso ETL y la consulta SQL.
- `resultado_consumo.csv`: Resultado final de la consulta exportado como archivo CSV.
- `README.md`: Este documento.
- `.gitignore`: Archivos que se excluyen del control de versiones.

---

## Instrucciones de uso

1. Coloca el archivo `bd.xlsx` en la carpeta del proyecto.
2. Abre y ejecuta el archivo `script_sqlite_consumo.py` (puedes usar Google Colab o cualquier entorno con Python).
3. El script cargará los datos, los procesará, ejecutará la consulta y mostrará el resultado.
4. Se generará el archivo `resultado_consumo.csv` con las preferencias por cliente.

---

## Notas adicionales

- Se implementó limpieza básica de datos, especialmente en las fechas.
- Se puede modificar fácilmente el rango de fechas (`fecha_inicio` y `fecha_fin`) y el número de preferencias (`top_n`).
- Se respetan buenas prácticas de escritura SQL como uso de CTEs y funciones de ventana.

