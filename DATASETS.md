# Datasets - Guía de Descarga

Este proyecto utiliza **3 datasets públicos de Kaggle**. Seguí estas instrucciones para descargarlos.

---

## Requisitos Previos

### Opción 1: Descarga Manual (Recomendado para principiantes)
1. Creá una cuenta en [Kaggle](https://www.kaggle.com/)
2. Descargá cada dataset haciendo clic en "Download" en las páginas de abajo
3. Descomprimí los archivos `.zip` en la carpeta `data/raw/`

### Opción 2: Descarga con Kaggle API
```bash
pip install kaggle

# Configurá tu API key (descargar desde https://www.kaggle.com/settings)
mkdir ~/.kaggle
mv kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
```

---

## Dataset 01: Netflix Movies & TV Shows

**URL**: https://www.kaggle.com/datasets/shivamb/netflix-shows

**Archivo**: `netflix_titles.csv`

**Descripción**: Catálogo completo de Netflix con +8000 títulos, incluyendo:
- Tipo (Movie/TV Show)
- Géneros
- País de producción
- Año de lanzamiento
- Fecha de agregado a Netflix

**Descarga manual**: Click en "Download" en la URL

**Descarga con API**:
```bash
kaggle datasets download -d shivamb/netflix-shows
unzip netflix-shows.zip -d data/raw/
```

---

## Dataset 02: Spotify Top Songs 2023

**URL**: https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023

**Archivo**: `spotify-2023.csv`

**Descripción**: Top tracks de Spotify 2023 con features de audio:
- Streams totales
- Artistas
- Features de audio (danceability, energy, valence, etc.)
- Fechas de lanzamiento
- Presencia en playlists

**Descarga manual**: Click en "Download" en la URL

**Descarga con API**:
```bash
kaggle datasets download -d nelgiriyewithana/top-spotify-songs-2023
unzip top-spotify-songs-2023.zip -d data/raw/
```

---

## Dataset 03: Twitch Top Streamers

**URL**: https://www.kaggle.com/datasets/aayushmishra1512/twitchdata

**Archivo**: `twitchdata-update.csv`

**Descripción**: Estadísticas de los top streamers de Twitch:
- Followers
- Average viewers
- Peak viewers
- Watch time (minutos)
- Stream time (minutos)
- Lenguaje

**Descarga manual**: Click en "Download" en la URL

**Descarga con API**:
```bash
kaggle datasets download -d aayushmishra1512/twitchdata
unzip twitchdata.zip -d data/raw/
```

---

## Estructura de Archivos Final

Después de descargar todo, tu carpeta `data/raw/` debería verse así:

```
data/
└── raw/
    ├── netflix_titles.csv
    ├── spotify-2023.csv
    └── twitchdata-update.csv
```

---

## Verificación

Podés verificar que los datasets se descargaron correctamente ejecutando:

```python
import pandas as pd

# Verificar Netflix
netflix = pd.read_csv('data/raw/netflix_titles.csv')
print(f'✅ Netflix: {netflix.shape[0]} registros')

# Verificar Spotify
spotify = pd.read_csv('data/raw/spotify-2023.csv', encoding='latin-1')
print(f'✅ Spotify: {spotify.shape[0]} registros')

# Verificar Twitch
twitch = pd.read_csv('data/raw/twitchdata-update.csv')
print(f'✅ Twitch: {twitch.shape[0]} registros')
```

---

## Licencias

Todos los datasets están disponibles en Kaggle bajo licencias de uso público para fines educativos y de portafolio. Verificá las licencias específicas en cada página de Kaggle.

---

**¿Problemas con la descarga?** Abrí un issue en este repo.
