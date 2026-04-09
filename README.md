# exportaciones-peru-ml
Sistema predictivo de oportunidades de exportación para PYMEs peruanas

# Detector de oportunidades de exportación — Perú

[![Python](https://img.shields.io/badge/Python-3.10-blue)]()
[![sklearn](https://img.shields.io/badge/scikit--learn-RandomForest-orange)]()
[![Plotly](https://img.shields.io/badge/Plotly-Dashboard-green)]()
[![License](https://img.shields.io/badge/License-MIT-lightgrey)]()

## Descripción
Este proyecto busca responder una pregunta clave para la internacionalización de las PYMEs peruanas:

¿En qué mercados y productos existen mayores probabilidades de éxito para exportar?

En un entorno global cada vez más dinámico —afectado por cambios en la demanda internacional, precios de commodities y condiciones macroeconómicas— tomar decisiones de exportación basadas únicamente en intuición implica un alto nivel de incertidumbre.

Para abordar este problema, se desarrolló un modelo de machine learning que permite identificar patrones en datos históricos de comercio internacional y detectar oportunidades potenciales de exportación.

## Demo interactiva
**[Ver dashboard en GitHub Pages →](https://renzo34990.github.io/exportaciones-peru-ml/)**

## Resultados principales
- Modelo Random Forest con R² = 0.637 sobre datos de test
- Top oportunidad identificada: **Arandanos → Estados Unidos** (score: 53.4)
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
