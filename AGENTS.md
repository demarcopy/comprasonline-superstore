# AGENTS.md — Obligatorio Taller de Visualización de Datos

## Contexto del proyecto

Este proyecto corresponde a un **obligatorio universitario de la materia Taller de Visualización de Datos**.

El trabajo utiliza el dataset **Superstore**, con información de compras/ventas de los últimos 4 años de la empresa ficticia **ComprasOnline.com**.

La entrega final debe incluir:

1. **Un documento/informe**
2. **Una presentación**
3. **Visualizaciones elaboradas y justificadas**

El foco principal no es solamente analizar datos, sino **comunicar hallazgos de negocio mediante visualizaciones claras, bien pensadas y visualmente trabajadas**.

---

## Consigna del cliente

La empresa ComprasOnline.com dispone de información de compras de los últimos 4 años y contrató una consultoría para identificar las características más relevantes de las transacciones y detectar oportunidades de crecimiento.

Se quiere analizar, entre otros aspectos:

- ventas por Segmento;
- ventas por Estado;
- evolución por año;
- ventas por Categoría de Producto;
- día de la semana con mayor cantidad de compras;
- top 10 de productos comprados;
- evolución de esos productos durante los 4 años;
- top 10 de productos más comprados en los últimos 6 meses;
- evolución reciente de esos productos.

Preguntas guía de la consigna:

- ¿Cómo ha sido la venta por Segmento?
- ¿Cómo ha sido la venta por Estado? Analizar evolución y observar especialmente el último año.
- ¿Cuál ha sido la venta por categoría de producto?
- Identificar las ventas de productos con mayores ganancias.
- Identificar las ventas de productos con mayores pérdidas.
- Identificar el ShipMode para el top 10 de clientes.

Estas preguntas son orientativas. Se pueden proponer otras si resultan relevantes y están respaldadas por el dataset.

---

# Rol de los agentes

Actuar como apoyo en:

- análisis exploratorio de datos;
- visualización de datos;
- storytelling;
- diseño de información;
- análisis de negocio;
- redacción del informe;
- preparación de la presentación.

No actuar únicamente como programador.

La prioridad es producir **pocas visualizaciones buenas** antes que muchos gráficos superficiales.

---

# Principio fundamental

Cada visualización debe responder una pregunta concreta.

Antes de crear un gráfico, siempre poder completar:

> “Quiero mostrar que…”

Diferenciar siempre entre:

1. **Exploración:** gráficos para entender los datos.
2. **Hallazgo:** patrón relevante detectado.
3. **Visualización final:** gráfico diseñado específicamente para comunicar ese hallazgo.

Los gráficos exploratorios no tienen que formar parte de la entrega final.

---

# Forma de trabajo

Trabajar por etapas:

**dataset → exploración → preguntas → hallazgos → alternativas visuales → prototipos → refinamiento → narrativa → documento → presentación**

No completar todas las etapas automáticamente.

Cuando sea necesaria una decisión del usuario:

1. presentar alternativas;
2. explicar ventajas y desventajas;
3. recomendar una o dos;
4. detenerse;
5. esperar la decisión del usuario.

---

# ETAPA 0 — Entender el dataset

Inspeccionar primero el Excel real del proyecto.

Identificar:

- hojas;
- columnas;
- cantidad de registros;
- qué representa cada fila;
- tipos de datos;
- fechas y rango temporal;
- clientes;
- productos;
- categorías;
- subcategorías;
- segmentos;
- estados y regiones;
- ventas;
- cantidades;
- descuentos;
- ganancias/pérdidas;
- ShipMode;
- cualquier otra dimensión o métrica disponible.

Revisar:

- valores nulos;
- duplicados;
- inconsistencias;
- formatos de fecha;
- valores extremos;
- problemas de calidad.

No modificar el archivo original.

Documentar en:

`docs/01_dataset.md`

---

# ETAPA 1 — Análisis exploratorio

Analizar como mínimo:

- ventas por segmento;
- ventas por estado;
- evolución temporal;
- ventas por categoría y subcategoría;
- productos más vendidos;
- productos con mayor ganancia;
- productos con mayor pérdida;
- comportamiento de clientes;
- ShipMode;
- últimos 6 meses;
- día de la semana;
- descuentos y rentabilidad.

Buscar también patrones más interesantes que los pedidos explícitamente.

Ejemplos:

- estados con muchas ventas pero poca rentabilidad;
- descuentos altos asociados a operaciones poco rentables;
- categorías que crecen o caen;
- productos que concentran pérdidas;
- clientes que concentran una parte importante de las ventas;
- diferencias entre segmentos;
- cambios recientes;
- estacionalidad.

Documentar hallazgos potenciales en:

`docs/02_exploration.md`

---

# ETAPA 2 — Selección de preguntas

Proponer entre **6 y 10 preguntas de negocio** con potencial visual.

Para cada una indicar:

### Pregunta
Qué queremos comprender.

### Métricas
Qué valores se necesitan.

### Dimensiones
Cómo se segmentará la información.

### Hallazgo potencial
Qué podría volver interesante esa pregunta.

### Utilidad de negocio
Por qué le importaría al cliente.

### Potencial visual
Bajo / Medio / Alto.

Priorizar preguntas que permitan contar una historia.

Es mejor:

> ¿Qué estados generan muchas ventas pero destruyen rentabilidad?

que:

> ¿Cuánto vende cada estado?

Al finalizar:

- recomendar las preguntas con mayor potencial;
- esperar aprobación del usuario.

Guardar en:

`docs/03_questions.md`

---

# ETAPA 3 — Alternativas de visualización

Para cada hallazgo seleccionado, proponer varias formas de visualizarlo antes de implementar.

Considerar:

- barras;
- barras divergentes;
- líneas;
- áreas;
- slope charts;
- dumbbell charts;
- scatter plots;
- heatmaps;
- treemaps;
- small multiples;
- mapas;
- rankings;
- highlight tables;
- gráficos combinados.

Para cada alternativa evaluar:

- claridad;
- facilidad de comparación;
- jerarquía visual;
- complejidad;
- capacidad para destacar el hallazgo;
- adecuación al documento;
- adecuación a la presentación.

Guardar en:

`docs/04_visualization_options.md`

No implementar automáticamente todas las opciones.

---

# Principios de diseño visual

## Color

El color debe tener significado.

Usarlo para:

- representar una dimensión;
- mantener categorías consistentes;
- diferenciar ganancia y pérdida;
- destacar una categoría frente a un contexto neutro;
- representar intensidad.

No usar colores decorativos sin función.

Mantener el mismo significado cromático entre gráficos cuando sea posible.

Evitar demasiados colores simultáneos y priorizar contraste y accesibilidad.

---

## Labels

Usar etiquetas directas cuando mejoren la lectura.

Priorizar:

- valores importantes;
- máximos y mínimos;
- cambios relevantes;
- etiquetas directas sobre líneas o categorías.

Evitar saturar el gráfico.

---

## Iconos

Los iconos pueden utilizarse cuando tengan significado semántico.

Ejemplos:

- camión para ShipMode;
- caja/producto;
- cliente;
- flechas de tendencia;
- símbolos de ganancia/pérdida.

No utilizarlos solo como decoración.

Nunca deben reemplazar información cuantitativa precisa.

---

## Jerarquía visual

Debe ser evidente:

1. qué mirar primero;
2. qué información es secundaria;
3. qué funciona como contexto.

Usar posición, tamaño, contraste y color con intención.

---

## Ejes

Revisar:

- escala;
- unidades;
- orden;
- formato numérico;
- etiquetas;
- intervalos.

No manipular escalas para exagerar diferencias.

---

## Títulos

Evitar títulos genéricos.

Evitar:

> Ventas por Estado

Preferir títulos que comuniquen una conclusión:

> California lidera las ventas, pero otros estados muestran una rentabilidad muy inferior

solo si los datos lo respaldan.

---

## Anotaciones

Usar cuando aporten:

- líneas de referencia;
- promedios;
- highlights;
- flechas;
- texto breve;
- máximos;
- mínimos;
- eventos o cambios relevantes.

No agregar anotaciones como decoración.

---

# ETAPA 4 — Prototipos

Una vez elegida una visualización, crear un primer prototipo.

Herramientas posibles:

- Excel;
- Python;
- Pandas;
- Jupyter Notebook;
- Matplotlib;
- Plotly;
- otra herramienta apropiada.

Elegir la tecnología en función de la visualización.

No usar Python solamente por parecer más avanzado.

Si Excel resuelve mejor una visualización, usar Excel.

Guardar gráficos en:

`outputs/charts/`

---

# ETAPA 5 — Revisión crítica

Antes de considerar un gráfico final, evaluar:

### Mensaje
- ¿Qué quiero mostrar?
- ¿Se entiende rápidamente?

### Tipo de gráfico
- ¿Es la mejor representación?

### Jerarquía
- ¿Se sabe dónde mirar primero?

### Color
- ¿Tiene significado?
- ¿Es consistente?

### Labels
- ¿Ayudan?
- ¿Hay demasiados?

### Ejes
- ¿Son claros y honestos?

### Carga cognitiva
- ¿Hay ruido?
- ¿Se puede eliminar la leyenda?
- ¿Hay demasiadas categorías?

### Narrativa
- ¿Aporta al relato general?

Guardar en:

`docs/05_visual_review.md`

---

# ETAPA 6 — Iteración

No considerar el primer gráfico como final.

Registrar para cada iteración:

- problema detectado;
- cambio realizado;
- motivo;
- resultado esperado.

Guardar en:

`docs/06_iterations.md`

---

# ETAPA 7 — Storytelling

Las visualizaciones finales deben formar una historia coherente.

Evitar una colección de gráficos independientes.

Estructura narrativa sugerida:

1. situación general;
2. qué está ocurriendo;
3. dónde aparece el problema u oportunidad;
4. qué variables ayudan a explicarlo;
5. qué debería considerar la empresa.

Para cada visualización documentar:

- pregunta;
- hallazgo;
- evidencia;
- interpretación;
- relevancia para el cliente;
- relación con el siguiente gráfico.

Guardar en:

`docs/07_storytelling.md`

---

# Recomendaciones de negocio

Separar siempre:

### Dato
Lo que muestra el dataset.

### Interpretación
Lo que razonablemente puede inferirse.

### Recomendación
Acción que el cliente podría evaluar.

No afirmar causalidad sin evidencia.

---

# Documento final

El informe debe ser visual y utilizar los gráficos como parte central de la comunicación.

Estructura sugerida:

## Portada
- trabajo;
- materia;
- integrantes;
- fecha.

## 1. Contexto
Problema del cliente.

## 2. Dataset
Período, dimensiones, métricas y limitaciones.

## 3. Objetivos
Preguntas seleccionadas.

## 4. Hallazgos
Organizar por hallazgo, no por columnas.

Cada sección debería contener:

- pregunta;
- visualización;
- lectura;
- conclusión.

## 5. Oportunidades y problemas

## 6. Conclusiones y recomendaciones

## 7. Metodología / notas
Solo cuando aporten valor.

Evitar bloques de texto excesivamente largos.

---

# Presentación final

La presentación NO debe ser el informe dividido en slides.

Debe funcionar como una narración oral.

Estructura sugerida:

### Slide 1 — Portada

### Slide 2 — El desafío
Contexto del cliente.

### Slide 3 — Panorama general
Uno o dos datos que den contexto.

### Slides centrales — Hallazgos
Una idea principal por slide.

Cada slide debería tener:

- título que comunique una conclusión;
- visualización principal;
- poco texto;
- uno o dos elementos de apoyo.

### Penúltima slide — Qué aprendimos

### Última slide — Recomendaciones / cierre

Evitar slides saturadas.

---

# Coherencia visual

Documento y presentación deben compartir:

- narrativa;
- paleta;
- categorías;
- definiciones;
- métricas;
- conclusiones.

Mantener colores consistentes para las mismas dimensiones.

El informe puede tener más detalle.

La presentación debe ser más sintética.

---

# Estructura recomendada del proyecto

```text
project/
│
├── AGENTS.md
├── README.md
│
├── data/
│   ├── raw/
│   │   └── superstore.xlsx
│   └── processed/
│
├── notebooks/
├── src/
│
├── outputs/
│   ├── charts/
│   ├── report/
│   └── presentation/
│
└── docs/
    ├── 01_dataset.md
    ├── 02_exploration.md
    ├── 03_questions.md
    ├── 04_visualization_options.md
    ├── 05_visual_review.md
    ├── 06_iterations.md
    └── 07_storytelling.md
```

No crear archivos vacíos innecesariamente.

---

# Reglas para los agentes

## Hacer

- inspeccionar siempre los datos reales;
- cuestionar si un gráfico es la mejor opción;
- proponer alternativas;
- justificar decisiones visuales;
- buscar historias;
- trabajar iterativamente;
- mantener consistencia visual;
- usar color con significado;
- cuidar labels;
- usar anotaciones e iconos cuando aporten;
- pensar en la audiencia;
- documentar decisiones relevantes.

## No hacer

- inventar datos;
- inventar conclusiones;
- generar automáticamente todo el obligatorio;
- crear muchos gráficos superficiales;
- usar gráficos 3D;
- usar pie charts sin justificación clara;
- usar colores arbitrarios;
- saturar con labels;
- usar iconos decorativos sin función;
- confundir análisis exploratorio con visualización final;
- afirmar causalidad sin evidencia;
- escribir el informe final antes de definir los hallazgos;
- diseñar la presentación antes de definir la narrativa.

---

# Checklist de calidad visual

Antes de considerar final una visualización:

- [ ] Responde una pregunta clara.
- [ ] Tiene un hallazgo.
- [ ] Se entiende rápidamente.
- [ ] El tipo de gráfico es apropiado.
- [ ] El color tiene significado.
- [ ] Existe jerarquía visual.
- [ ] Los labels son útiles.
- [ ] Los ejes son claros.
- [ ] No hay decoración innecesaria.
- [ ] El título comunica información.
- [ ] Las categorías son consistentes con otros gráficos.
- [ ] Las anotaciones aportan.
- [ ] La visualización es honesta.
- [ ] Aporta algo a la narrativa general.

---

# Criterio de éxito

El obligatorio debe permitir que el cliente comprenda:

1. qué está ocurriendo en el negocio;
2. dónde existen oportunidades;
3. dónde existen problemas;
4. qué patrones son importantes;
5. qué evidencia respalda las conclusiones.

La prioridad es:

**claridad + análisis + intención visual + elaboración + storytelling**

por encima de:

**cantidad de gráficos + complejidad técnica + decoración**.
