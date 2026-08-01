# Exploración

## Pregunta 2: ¿Cómo ha sido la venta por Estado?

Quiero mostrar que las ventas están muy concentradas en pocos estados y que, al observar el último año, algunos estados con ventas relevantes no generan rentabilidad positiva.

### Métricas y dimensiones usadas

- Métrica principal: `Sales`
- Métrica complementaria: `Profit`
- Dimensión principal: `State`
- Dimensión temporal: año de `Order Date`
- Foco temporal: último año disponible, 2017

### Lectura general 2014-2017

- Ventas totales del período: USD 2.297.200,86
- Los 5 estados con mayores ventas concentran aproximadamente 52,0% de las ventas totales.
- Top 5 por ventas acumuladas:
- California: USD 457.687,63
- New York: USD 310.876,27
- Texas: USD 170.188,05
- Washington: USD 138.641,27
- Pennsylvania: USD 116.511,91

### Evolución anual

- California se mantiene como el estado dominante durante el período.
- New York sostiene el segundo lugar y crece con fuerza en 2017 frente a 2016.
- Washington tiene un salto muy marcado en 2017: pasa de USD 19.814,28 en 2016 a USD 65.539,90 en 2017.
- Pennsylvania también aumenta en 2017, pero con rentabilidad negativa.
- Virginia cae fuertemente en 2017 frente a 2016, por lo que conviene no tratarla solo como un estado históricamente relevante.

### Foco en 2017

Top 12 estados por ventas en 2017:

| Estado | Ventas 2017 | Ganancia 2017 |
|---|---:|---:|
| California | USD 146.388,34 | USD 29.366,46 |
| New York | USD 93.923,00 | USD 24.357,07 |
| Washington | USD 65.539,90 | USD 17.256,78 |
| Texas | USD 43.421,76 | USD -8.838,50 |
| Pennsylvania | USD 42.688,31 | USD -5.112,80 |
| Florida | USD 26.444,72 | USD 244,13 |
| Michigan | USD 25.833,65 | USD 8.487,76 |
| Illinois | USD 24.351,61 | USD -6.745,56 |
| North Carolina | USD 23.456,83 | USD -5.088,53 |
| Ohio | USD 23.264,85 | USD -1.736,53 |
| Georgia | USD 19.160,02 | USD 6.447,98 |
| Indiana | USD 18.516,45 | USD 5.139,53 |

### Hallazgo potencial

El análisis por estado no debería comunicarse solo como ranking de ventas. En 2017, Texas, Pennsylvania, Illinois, North Carolina y Ohio aparecen entre los 12 estados con más ventas, pero cierran el año con pérdidas. En conjunto, esos cinco estados aportan USD 157.183,36 en ventas 2017, pero destruyen USD 27.521,93 de ganancia.

### Interpretación de negocio

California, New York y Washington parecen ser mercados fuertes y rentables en el último año. En cambio, Texas y Pennsylvania son estados comercialmente importantes, pero requieren revisar descuentos, mix de productos, costos de envío o segmentos de clientes, porque vender más allí no está implicando ganar más.

### Recomendación preliminar

Para responder la pregunta del cliente, conviene reformularla ligeramente:

> ¿Qué estados explican las ventas y cuáles representan una oportunidad o riesgo al mirar la rentabilidad del último año?

Esta formulación permite pasar de una descripción básica a una historia de negocio más útil.
