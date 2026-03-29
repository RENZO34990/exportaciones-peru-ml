# exportaciones-peru-ml
Modelo predictivo de oportunidades de exportación para PYMEs peruanas usando Random Forest y datos abiertos

# Detector de oportunidades de exportación — Perú

[![Python](https://img.shields.io/badge/Python-3.10-blue)]()
[![sklearn](https://img.shields.io/badge/scikit--learn-RandomForest-orange)]()
[![Plotly](https://img.shields.io/badge/Plotly-Dashboard-green)]()
[![License](https://img.shields.io/badge/License-MIT-lightgrey)]()

## Descripción
Modelo predictivo que identifica las mejores oportunidades de exportación
para PYMEs peruanas usando Random Forest y datos abiertos de comercio
internacional (Trade Map, BCRP, World Bank).

## Demo interactiva
**[Ver dashboard en GitHub Pages →](https://github.com/RENZO34990/exportaciones-peru-ml))**

## Resultados principales
- Modelo Random Forest con R² = 0.XX sobre datos de test
- Top oportunidad identificada: **Palta → Corea del Sur** (score: 84.2)
- Variable más importante: crecimiento de demanda del país destino (35%)
- 10 productos × 8 mercados × 5 años analizados

## Metodología
```
Datos abiertos → Limpieza → Feature Engineering → RCA (Balassa 1965)
       → Score ponderado → Random Forest → Ranking + Dashboard
```

## Fuentes de datos
| Fuente | Variable | Acceso |
|--------|----------|--------|
| Trade Map / ITC | Exportaciones Perú por HS Code | Gratuito |
| BCRP | Tipo de cambio, inflación | Gratuito |
| World Bank | PBI per cápita países | Gratuito |

## Estructura del proyecto
```
├── dataset_exportaciones_limpio.csv
├── Predicción_mercados.ipynb
├── ranking_oportunidades.csv
└── dashboard_exportaciones.html
```

## Tecnologías
Python · pandas · scikit-learn · Plotly · Google Colab

## Autor
**Renzo Rojas** — Economía Internacional, [Universidad Nacional Mayor de San Marcos] · Lima, Perú
[LinkedIn](www.linkedin.com/in/renzo-rojas-salazar-50841b286)
