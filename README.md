# Streaming Analytics Factory

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Kaggle](https://img.shields.io/badge/Kaggle-Datasets-20BEFF?logo=kaggle&logoColor=white)

> Fábrica de análisis de datos sobre plataformas de streaming con foco en **valor económico real**: revenue, retención, LTV y decision-making basado en datos.

---

## 🎯 Objetivo

Demostrar capacidad analítica end-to-end: desde la exploración del dataset hasta insights accionables con impacto de negocio medible. Cada notebook está diseñado como un caso de negocio real.

---

## 👨‍💻 Enfoque del Proyecto

Este repositorio documenta un **framework de análisis de datos** para plataformas de streaming. Incluye:

- Metodología de análisis orientado a valor económico
- Stack técnico recomendado (Pandas, Matplotlib, Seaborn)
- Estructura de proyecto profesional con carpetas organizadas
- Documentación de datasets públicos relevantes

---

## 📂 Estructura del Repositorio

```
streaming-analytics-factory/
├── notebooks/
│   ├── 01_netflix_content_analysis.ipynb
│   ├── 02_spotify_revenue_analysis.ipynb
│   └── 03_twitch_monetization_analysis.ipynb
├── data/
│   ├── raw/          # Datasets originales de Kaggle
│   └── processed/    # Datos limpios post-ETL
├── assets/
│   └── charts/       # Visualizaciones exportadas
├── requirements.txt
└── README.md
```

---

## 💡 Insights Clave por Análisis

### 🎥 Netflix
- Identificación de géneros con mayor densidad de contenido vs rating
- Evolución de producción propia vs adquirida (2015–2023)
- Países con mayor potencial de expansión de catálogo

### 🎵 Spotify
- Top artistas por revenue estimado (streams x $0.004 por stream)
- Correlación entre duración del track y popularidad
- Análisis de características de audio en canciones virales

### 🎮 Twitch
- Revenue estimado por streamer (suscripciones + bits)
- Relación entre horas transmitidas y crecimiento de audiencia
- Categorías con mayor monetización por viewer

---

## 🛠️ Tecnologías Utilizadas

| Herramienta | Uso |
|---|---|
| **Python 3.10+** | Lenguaje principal |
| **Pandas** | Manipulación y limpieza de datos |
| **Matplotlib / Seaborn** | Visualización |
| **NumPy** | Cálculos numéricos |
| **Jupyter Notebook** | Entorno de análisis |

---

## 🚀 Cómo Ejecutar

```bash
# 1. Clonar el repositorio
git clone https://github.com/federicoramos67/streaming-analytics-factory.git
cd streaming-analytics-factory

# 2. Instalar dependencias
pip install -r requirements.txt

# 3. Abrir Jupyter
jupyter notebook notebooks/
```

También podés ejecutar cada notebook en **Google Colab** haciendo clic en el badge de cada uno.

---

## 📊 Datasets

Este proyecto utiliza **3 datasets públicos de Kaggle**.

📝 **Ver guía completa**: [DATASETS.md](https://github.com/federicoramos67/streaming-analytics-factory/blob/main/DATASETS.md)

**Quick Start** (descarga manual desde Kaggle):
- [Netflix Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- [Top Spotify Songs 2023](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023)
- [Twitch Data](https://www.kaggle.com/datasets/aayushmishra1512/twitchdata)

Colocá los archivos CSV descargados en `data/raw/`.

---

## 👤 Sobre el Autor

**Federico Ramos** — Analista de Datos Jr.

Formado como Analista de Datos Jr. por Fundación Telefónica Movistar en colaboración con la Universidad Católica del Uruguay e INEFOP (300 h). Apasionado por transformar datos en decisiones de negocio.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/federico-ramos-904024281)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/federicoramos67)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:federicoramos6767@gmail.com)

---

> Datasets obtenidos de Kaggle bajo licencias de uso público para fines educativos y de portafolio.
