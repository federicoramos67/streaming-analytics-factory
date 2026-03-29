# Streaming Analytics Factory

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Kaggle](https://img.shields.io/badge/Kaggle-Datasets-20BEFF?logo=kaggle&logoColor=white)

> Fabrica de analisis de datos sobre plataformas de streaming con foco en **valor economico real**: revenue, retencion, LTV y decision-making basado en datos.

---

## Objetivo

Demostrar capacidad analitica end-to-end: desde la exploracion del dataset hasta insights accionables con impacto de negocio medible. Cada notebook esta disenado como un caso de negocio real.

---

## Analisis Incluidos

| # | Plataforma | Dataset | Foco de Negocio | Notebook |
|---|-----------|---------|-----------------|----------|
| 01 | Netflix | Netflix Movies & TV Shows (Kaggle) | Estrategia de contenido y ROI por genero | [En desarrollo](notebooks/01_netflix_content_analysis.ipynb) |
| 02 | Spotify | Spotify Top Tracks 2023 (Kaggle) | Revenue estimado por streams y artistas | [En desarrollo](notebooks/02_spotify_revenue_analysis.ipynb) |
| 03 | Twitch | Twitch Top Streamers (Kaggle) | Monetizacion y valor por viewership | [En desarrollo](notebooks/03_twitch_monetization_analysis.ipynb) |

---

## Estructura del Repositorio

```
streaming-analytics-factory/
|-- notebooks/
|   |-- 01_netflix_content_analysis.ipynb
|   |-- 02_spotify_revenue_analysis.ipynb
|   |-- 03_twitch_monetization_analysis.ipynb
|-- data/
|   |-- raw/          # Datasets originales de Kaggle
|   |-- processed/    # Datos limpios post-ETL
|-- assets/
|   |-- charts/       # Visualizaciones exportadas
|-- requirements.txt
|-- README.md
```

---

## Insights Clave por Analisis

### Netflix
- Identificacion de generos con mayor densidad de contenido vs rating
- Evolucion de produccion propia vs adquirida (2015-2023)
- Paises con mayor potencial de expansion de catalogo

### Spotify
- Top artistas por revenue estimado (streams x $0.004 por stream)
- Correlacion entre duracion del track y popularidad
- Analisis de caracteristicas de audio en canciones virales

### Twitch
- Revenue estimado por streamer (suscripciones + bits)
- Relacion entre horas transmitidas y crecimiento de audiencia
- Categorias con mayor monetizacion por viewer

---

## Tecnologias Utilizadas

- **Python 3.10+** - Lenguaje principal
- **Pandas** - Manipulacion y limpieza de datos
- **Matplotlib / Seaborn** - Visualizacion
- **NumPy** - Calculos numericos
- **Jupyter Notebook** - Entorno de analisis

---

## Como Ejecutar

```bash
# 1. Clonar el repositorio
git clone https://github.com/federicoramos67/streaming-analytics-factory.git
cd streaming-analytics-factory

# 2. Instalar dependencias
pip install -r requirements.txt

# 3. Abrir Jupyter
jupyter notebook notebooks/
```

Tambien podes ejecutar cada notebook en **Google Colab** haciendo clic en el badge de cada uno.

---

## 📊 Datasets

Este proyecto utiliza **3 datasets públicos de Kaggle**. 

📝 **Ver guía completa**: [DATASETS.md](DATASETS.md)

**Quick Start**:
```bash
# Opción 1: Descarga manual desde Kaggle (recomendado)
# - Netflix: https://www.kaggle.com/datasets/shivamb/netflix-shows
# - Spotify: https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023
# - Twitch: https://www.kaggle.com/datasets/aayushmishra1512/twitchdata

# Opción 2: Con Kaggle API
pip install kaggle
kaggle datasets download -d shivamb/netflix-shows
kaggle datasets download -d nelgiriyewithana/top-spotify-songs-2023
kaggle datasets download -d aayushmishra1512/twitchdata
```

Colocá los archivos CSV descargados en `data/raw/`.

## Sobre el Autor

**Federico Ramos** - Analista de Datos Jr.

Formado como Analista de Datos Jr. por Fundacion Telefonica Movistar en colaboracion con la Universidad Catolica del Uruguay e INEFOP (300 h). Apasionado por transformar datos en decisiones de negocio.

[![GitHub](https://img.shields.io/badge/GitHub-federicoramos67-181717?logo=github)](https://github.com/federicoramos67)
[![Email](https://img.shields.io/badge/Email-federicoramos6767@gmail.com-red?logo=gmail)](mailto:federicoramos6767@gmail.com)

---

*Datasets obtenidos de Kaggle bajo licencias de uso publico para fines educativos y de portafolio.*
