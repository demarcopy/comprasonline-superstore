# Propuesta de informe

## Objetivo del documento

Construir un informe visual y analítico para ComprasOnline.com a partir del dataset Superstore. El informe debe comunicar hallazgos de negocio respaldados por datos y visualizaciones claras.

No debe ser una colección de gráficos. Cada sección debe responder una pregunta concreta y aportar a una narrativa general sobre ventas, rentabilidad y oportunidades de crecimiento.

## Criterios para incluir contenido

Una visualización o hallazgo se incluye en el informe si cumple estos criterios:

- Responde una pregunta de negocio clara.
- Está respaldado por campos reales del dataset.
- Aporta una lectura útil para el cliente.
- Tiene una visualización comprensible sin demasiada explicación.
- Usa color con significado, no decorativo.
- Distingue entre dato, interpretación y recomendación.
- Evita afirmar causalidad si el dataset solo permite observar asociación.

## Estructura propuesta

### 1. Portada

- Nombre del trabajo.
- Materia.
- Integrantes.
- Fecha.
- Cliente: ComprasOnline.com.

### 2. Contexto del cliente

ComprasOnline.com cuenta con información de compras y ventas de los últimos 4 años. El objetivo del análisis es identificar características relevantes de las transacciones y detectar oportunidades de crecimiento.

### 3. Dataset utilizado

- Dataset: Superstore.
- Archivo: `data/raw/Sample - Superstore v1.0.xlsx`.
- Período: 2014-01-03 a 2017-12-30.
- Registros: 9.994 filas.
- Cada fila representa una línea de pedido/transacción.
- Métricas principales: `Sales`, `Quantity`, `Discount`, `Profit`.
- Dimensiones principales: `Segment`, `State`, `Region`, `Category`, `Sub-Category`, `Product Name`, `Customer Name`, `Ship Mode`.

### 4. Objetivos del análisis

Responder preguntas sobre:

- Ventas por segmento.
- Ventas por estado y evolución anual.
- Ventas por categoría de producto.
- Productos con mayores ganancias.
- Productos con mayores pérdidas.
- Ship Mode para los principales clientes.
- Patrones adicionales relevantes para oportunidades de crecimiento.

### 5. Hallazgos

Cada hallazgo debería tener esta estructura:

- Pregunta.
- Visualización.
- Lectura del gráfico.
- Evidencia numérica.
- Interpretación de negocio.
- Recomendación o próximo análisis.

## Propuesta actual so far

### Hallazgo 1 - Ventas por Estado

**Pregunta:** ¿Cómo ha sido la venta por Estado? Ver evolución y observar especialmente el último año.

**Mensaje principal:** en 2017, algunos estados vendieron mucho pero generaron pérdidas.

**Campos utilizados:**

- `State`: estado.
- `Order Date`: fecha de la orden, usada para extraer el año.
- `Sales`: ventas.
- `Profit`: ganancia o pérdida.

**Evidencia:**

En 2017, dentro del top 12 de estados por ventas, hubo cinco estados con ganancia negativa:

| Estado | Ventas 2017 | Ganancia 2017 |
|---|---:|---:|
| Texas | USD 43.421,76 | USD -8.838,50 |
| Pennsylvania | USD 42.688,31 | USD -5.112,80 |
| Illinois | USD 24.351,61 | USD -6.745,56 |
| North Carolina | USD 23.456,83 | USD -5.088,53 |
| Ohio | USD 23.264,85 | USD -1.736,53 |

En conjunto, estos estados aportaron USD 157.183,36 en ventas 2017, pero destruyeron USD 27.521,93 de ganancia.

**Visualización principal propuesta:**

- Archivo: `outputs/charts/estado_ventas_2017_rentabilidad.png`.
- Tipo: barras horizontales por estado.
- Eje X: suma de `Sales` en 2017.
- Eje Y: `State`.
- Color: verde si `Profit` es positivo, rojo si `Profit` es negativo.
- Motivo: permite ver rápidamente que vender más no siempre implica ganar más.

**Visualización de apoyo:**

- Archivo: `outputs/charts/estado_ventas_evolucion_top12.png`.
- Tipo: barras horizontales agrupadas por año.
- Eje X: suma de `Sales`.
- Eje Y: `State`.
- Series: año de `Order Date`.
- Motivo: muestra la evolución anual y destaca el crecimiento de Washington en 2017.

**Lectura para el informe:**

California y New York son los estados con mayor volumen de ventas y mantienen ganancias positivas en 2017. Washington también muestra un crecimiento fuerte y rentable en el último año. Sin embargo, Texas, Pennsylvania, Illinois, North Carolina y Ohio combinan ventas relevantes con pérdidas, por lo que representan mercados que requieren análisis adicional antes de considerarlos oportunidades de inversión.

**Interpretación:**

El volumen de ventas por estado no alcanza para definir dónde invertir. ComprasOnline.com debería distinguir entre estados grandes y rentables, y estados grandes pero problemáticos.

**Recomendación preliminar:**

Profundizar en los estados con pérdidas revisando descuentos, categorías, subcategorías, productos y Ship Mode. El objetivo sería detectar si la pérdida está asociada a descuentos altos, mix de productos poco rentable o costos de envío.

## Próximos hallazgos a desarrollar

- Ventas por segmento.
- Ventas por categoría y subcategoría.
- Productos con mayores ganancias.
- Productos con mayores pérdidas.
- Ship Mode para top clientes.
- Últimos 6 meses y evolución reciente de productos principales.
