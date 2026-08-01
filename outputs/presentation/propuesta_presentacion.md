# Propuesta de presentación

## Objetivo de la presentación

Construir una presentación breve y narrativa para comunicar los principales hallazgos a ComprasOnline.com.

La presentación no debe repetir todo el informe. Debe funcionar como una historia oral con pocas ideas fuertes, una visualización principal por slide y texto mínimo.

## Criterios para incluir slides

Una slide se incluye si cumple estos criterios:

- Comunica una sola idea principal.
- Tiene un título que expresa una conclusión, no un tema genérico.
- Usa una visualización clara y legible.
- Evita tablas grandes o texto excesivo.
- Aporta a la historia general del negocio.
- Permite explicar el hallazgo oralmente en menos de 2 minutos.

## Estructura propuesta de slides

### Slide 1 - Portada

**Título sugerido:** Análisis de ventas y oportunidades para ComprasOnline.com

Contenido:

- Materia.
- Integrantes.
- Fecha.
- Dataset Superstore.

### Slide 2 - El desafío

**Título sugerido:** ComprasOnline.com quiere saber dónde puede crecer mejor

Contenido:

- La empresa tiene 4 años de datos de ventas.
- El objetivo es identificar características relevantes de las transacciones.
- El foco es detectar oportunidades y problemas de negocio.

### Slide 3 - Dataset analizado

**Título sugerido:** Analizamos 9.994 transacciones entre 2014 y 2017

Contenido:

- Período: 2014-2017.
- Métricas: ventas, cantidad, descuentos y ganancias.
- Dimensiones: clientes, estados, segmentos, categorías, productos y modos de envío.

### Slide 4 - Preguntas guía

**Título sugerido:** Las preguntas conectan ventas, rentabilidad y comportamiento del cliente

Contenido:

- Ventas por segmento.
- Ventas por estado.
- Categorías de producto.
- Productos con mayor ganancia y pérdida.
- Ship Mode para top clientes.
- Evolución reciente.

## Propuesta actual so far

### Slide 5 - Hallazgo por Estado

**Título sugerido:** En 2017, algunos estados vendieron mucho pero generaron pérdidas

Visual principal:

- `outputs/charts/estado_ventas_2017_rentabilidad.png`

Mensaje oral:

El ranking de ventas por estado muestra que California, New York y Washington fueron mercados fuertes y rentables en 2017. Pero Texas, Pennsylvania, Illinois, North Carolina y Ohio también aparecen entre los estados con más ventas y aun así tuvieron pérdidas.

Datos de apoyo:

- Texas: USD 43.421,76 en ventas y USD -8.838,50 de ganancia.
- Pennsylvania: USD 42.688,31 en ventas y USD -5.112,80 de ganancia.
- Los cinco estados con pérdida dentro del top 12 destruyeron USD 27.521,93 de ganancia.

Diseño sugerido:

- Usar barras horizontales.
- Mantener el eje X como ventas 2017.
- Usar verde para ganancia positiva y rojo para pérdida.
- Evitar saturar con demasiadas etiquetas.
- Incluir una nota breve: "Color según ganancia 2017".

### Slide 6 - Evolución por Estado

**Título sugerido:** Washington acelera en 2017, mientras California mantiene el liderazgo

Visual de apoyo:

- `outputs/charts/estado_ventas_evolucion_top12.png`

Mensaje oral:

La evolución anual permite ver que California se mantiene como el estado con mayor volumen. Washington destaca por un salto fuerte en 2017, lo que lo convierte en un mercado interesante para mirar con más detalle.

Uso recomendado:

- Esta slide puede ser opcional.
- Si la presentación queda larga, conviene mantenerla como apoyo para preguntas o anexos.

### Slide 7 - Interpretación de negocio

**Título sugerido:** No todos los mercados grandes son oportunidades claras de inversión

Contenido:

- Estados grandes y rentables: California, New York, Washington.
- Estados grandes con alerta: Texas, Pennsylvania, Illinois, North Carolina, Ohio.
- Próximo paso: analizar descuentos, categorías y productos en estados con pérdidas.

### Slide 8 - Cierre provisional

**Título sugerido:** La oportunidad está en crecer sin perder rentabilidad

Contenido:

- Priorizar mercados con ventas altas y ganancias positivas.
- Investigar estados con pérdidas antes de invertir más.
- Completar el análisis con segmento, categoría, productos y clientes.

## Próximas slides a desarrollar

- Ventas por segmento.
- Ventas por categoría de producto.
- Productos más rentables.
- Productos con mayores pérdidas.
- Ship Mode para principales clientes.
- Recomendaciones finales.
