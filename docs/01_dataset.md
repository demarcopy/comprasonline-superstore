# Dataset Superstore

## Fuente inspeccionada

- Archivo: `data/raw/Sample - Superstore v1.0.xlsx`
- Hoja de datos utilizada: `Sample - Superstore`
- Hoja adicional: `intro`

## Estructura

- Registros: 9.994 filas
- Columnas: 22
- Cada fila representa una línea de pedido/transacción de venta.
- Período cubierto: 2014-01-03 a 2017-12-30
- Estados: 49
- País: United States

## Campos principales

- Fechas: `Order Date`, `Ship Date`
- Cliente: `Customer ID`, `Customer Name`, `Segment`
- Geografía: `Country`, `City`, `State`, `Postal Code`, `Region`
- Producto: `Product ID`, `Category`, `Sub-Category`, `Product Name`
- Métricas: `Sales`, `Quantity`, `Discount`, `Profit`
- Envío: `Ship Mode`
- Campo adicional: `Class`

## Calidad de datos observada

- No se detectaron valores nulos en la hoja de datos.
- Las fechas están en formato datetime.
- `Sales`, `Discount` y `Profit` son numéricos.
- `Quantity` es entero.
