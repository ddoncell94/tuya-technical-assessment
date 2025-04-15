# Prueba Técnica - Tuya

## Punto 3: Rachas de Niveles de Deuda

Este módulo analiza la historia de saldos mensuales de clientes y detecta rachas consecutivas donde los clientes se mantienen en el mismo nivel de deuda.

### 📌 Objetivo

- Clasificar los saldos en niveles de deuda.
- Identificar secuencias consecutivas (rachas) de un mismo nivel.
- Seleccionar la racha más larga (o más reciente en caso de empate) por cliente.

### 📂 Archivos de entrada

- `rachas.xlsx` con dos hojas:
  - `historia`: contiene identificación, corte_mes y saldo.
  - `retiros`: contiene la fecha de retiro del cliente.

### 🛠️ Herramientas utilizadas

- Python 3
- pandas
- sqlite3
- SQL (para lógica de procesamiento de rachas)

### 🧮 Niveles de saldo

- `N0`: saldo entre 0 y <300,000
- `N1`: 300,000 <= saldo < 1,000,000
- `N2`: 1,000,000 <= saldo < 3,000,000
- `N3`: 3,000,000 <= saldo < 5,000,000
- `N4`: saldo >= 5,000,000

### 📋 Instrucciones

1. Asegúrate de tener el archivo `rachas.xlsx` en la ruta correspondiente.
2. Ejecuta el script en Google Colab o entorno local.
3. Se generará una base de datos SQLite (`rachas.db`) y múltiples vistas auxiliares para facilitar el análisis.
4. El resultado final será una tabla con la racha más larga por cliente.

### Archivos generados

- `rachas.db`: base de datos SQLite con todas las tablas y vistas necesarias.
- DataFrame con el resultado final del análisis (puede exportarse a CSV si se desea).

