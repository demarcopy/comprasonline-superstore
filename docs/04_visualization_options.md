# Alternativas de visualización

## Pregunta 2: venta por Estado, evolución y último año

### Opción A: barras agrupadas por año para top 12 estados

- Archivo prototipo: `outputs/charts/estado_ventas_evolucion_top12.png`
- Claridad: media-alta
- Comparación: buena para ver evolución anual dentro de cada estado.
- Ventaja: responde directamente la parte de evolución.
- Desventaja: con muchos estados puede volverse denso.
- Uso recomendado: informe, donde hay más tiempo para leer.

### Opción B: ranking 2017 por ventas con color según ganancia o pérdida

- Archivo prototipo: `outputs/charts/estado_ventas_2017_rentabilidad.png`
- Claridad: alta
- Comparación: muy buena para observar el último año.
- Ventaja: revela rápido que algunos estados venden mucho pero pierden dinero.
- Desventaja: no muestra toda la evolución histórica.
- Uso recomendado: presentación, porque comunica un hallazgo claro en pocos segundos.

### Opción C: mapa por estado con intensidad de ventas y borde/color de rentabilidad

- Claridad: media
- Comparación: limitada, porque comparar áreas geográficas no siempre es preciso.
- Ventaja: aprovecha la dimensión geográfica y puede ser atractivo visualmente.
- Desventaja: requiere más diseño para no convertirse en decoración.
- Uso recomendado: solo si se quiere enfatizar dispersión geográfica.

### Opción D: scatter plot ventas vs ganancia por estado

- Claridad: alta para detectar riesgos y oportunidades.
- Comparación: buena para separar estados de alto volumen rentables y no rentables.
- Ventaja: muestra en una sola vista ventas y rentabilidad.
- Desventaja: responde menos directamente la evolución temporal.
- Uso recomendado: análisis o como visual complementaria si el relato se centra en rentabilidad.

## Recomendación

Usar dos visualizaciones coordinadas:

- Para evolución: barras agrupadas del top 12 de estados.
- Para hallazgo principal del último año: ranking 2017 coloreado por rentabilidad.

La segunda visualización tiene mayor fuerza narrativa porque transforma la pregunta de “dónde vendemos más” en “dónde vender más no necesariamente genera valor”.
