# Prueba Técnica - Tuya

Este repositorio contiene la solución al primer punto de la prueba técnica de Tuya, donde se procesan archivos HTML para reemplazar imágenes por versiones embebidas en formato base64.

## Objetivo

Automatizar el procesamiento de archivos HTML para:

- Buscar imágenes dentro del código HTML.
- Convertirlas a base64.
- Reemplazarlas directamente en el HTML.
- Guardar el HTML modificado y un resumen en formato JSON con las imágenes procesadas correctamente o con error.

## Tecnologías usadas

- Python 3
- Librerías estándar: `os`, `base64`, `json`, `pathlib`, `html.parser`

## Estructura del proyecto

- `htmls_prueba/`: Carpeta de entrada con los archivos HTML originales.
- `html_modificados/`: Carpeta de salida con los archivos HTML modificados.
- `resumen_resultado.json`: Archivo con el resumen del procesamiento.

## Cómo ejecutar

1. Asegúrate de tener tus archivos HTML en la ruta especificada.
2. Ejecuta el script en Google Colab o un entorno local de Python.
3. Verifica el contenido de la carpeta de salida y el archivo `resumen_resultado.json`.

