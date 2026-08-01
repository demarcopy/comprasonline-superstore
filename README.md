# comprasonline-superstore

Proyecto del obligatorio de **Taller de Visualización de Datos** basado en el dataset Superstore.

El objetivo es analizar las ventas de la empresa ficticia **ComprasOnline.com** y construir visualizaciones que comuniquen hallazgos de negocio de forma clara.

## Contenido

- `consigna.md`: consigna original del desafío.
- `data/raw/`: dataset original en Excel.
- `notebooks/`: cuadernos Jupyter con el análisis exploratorio.
- `docs/`: documentación del dataset, exploración y decisiones visuales.
- `outputs/charts/`: gráficos exportados.
- `outputs/report/`: propuesta y materiales para el informe final.
- `outputs/presentation/`: propuesta y materiales para la presentación.

## Análisis iniciado

### Pregunta 2 - Venta por Estado

Se analizó la venta por estado, su evolución anual y el comportamiento del último año disponible, 2017.

Hallazgo inicial: algunos estados con ventas altas en 2017 tuvieron rentabilidad negativa. Por eso, el análisis no debería mirar solo `Sales`, sino también `Profit`.

Gráficos generados:

- `outputs/charts/estado_ventas_evolucion_top12.png`
- `outputs/charts/estado_ventas_2017_rentabilidad.png`

## Entregables en construcción

- Informe: `outputs/report/propuesta_informe.md`
- Presentación: `outputs/presentation/propuesta_presentacion.md`

Ambos archivos incluyen criterios de inclusión y la propuesta actual desarrollada hasta ahora.

## Cómo continuar

Abrir el notebook:

```bash
jupyter notebook notebooks/eda_superstore.ipynb
```

O desde VS Code/JupyterLab abrir directamente:

`notebooks/eda_superstore.ipynb`

## Dataset

El archivo original se mantiene sin modificar en:

`data/raw/Sample - Superstore v1.0.xlsx`
