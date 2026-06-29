# ⚽ International Football Analytics

Análisis exploratorio y modelo predictivo sobre 150 años de fútbol internacional (1872–2025), usando el dataset de [martj42](https://www.kaggle.com/datasets/martj42/international-football-results-from-1872-to-2017) con más de 49.000 partidos.

## Estructura del proyecto

```
football-analytics/
├── data/
│   ├── raw/          # Datos originales descargados (no versionados en Git)
│   └── processed/    # Datos limpios generados por este proyecto
├── notebooks/        # Análisis exploratorio y modelado
├── src/              # Módulos Python reutilizables
├── reports/
│   └── figures/      # Visualizaciones exportadas
└── requirements.txt
```

## Cómo reproducir

```bash
# 1. Clonar el repositorio
git clone https://github.com/AngelASAP107/football-analytics.git
cd football-analytics

# 2. Crear entorno virtual e instalar dependencias
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

# 3. Descargar los datos (requiere cuenta en Kaggle y API key configurada)
kaggle datasets download martj42/international-football-results-from-1872-to-2017 \
  --unzip -p data/raw/
```

## Dataset

| Archivo | Descripción |
|---|---|
| `results.csv` | 49.000+ partidos internacionales (1872–2025) |
| `goalscorers.csv` | Goleadores por partido |
| `shootouts.csv` | Resultados de definiciones por penales |
| `former_names.csv` | Mapeo de nombres históricos de selecciones |

> Los datos **no están versionados en Git**. Descárgalos siguiendo las instrucciones de arriba.

## Estado del proyecto

- [x] Etapa 1 — Setup de entorno, estructura y descarga de datos
- [ ] Etapa 2 — Limpieza y unificación de datos
- [ ] Etapa 3 — Análisis exploratorio (Capa A)
- [ ] Etapa 4 — Feature engineering
- [ ] Etapa 5 — Modelo predictivo (Capa B)
- [ ] Etapa 6 — README final con hallazgos y visualizaciones

## Tecnologías

![Python](https://img.shields.io/badge/Python-3.9-blue)
![pandas](https://img.shields.io/badge/pandas-2.x-lightgrey)
![scikit--learn](https://img.shields.io/badge/scikit--learn-1.x-orange)
![Jupyter](https://img.shields.io/badge/Jupyter-notebook-orange)
