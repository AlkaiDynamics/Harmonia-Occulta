

# Harmonia Occulta: Un Estudio Computacional del Monochordum Mundi de Robert Fludd

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1234567.svg)](https://doi.org/10.5281/zenodo.1234567)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## Descripción General

Este repositorio contiene el código y los datos para el artículo "The Completed Harmony: A Computational Pilot Study of Musical Encodings in Robert Fludd's Monochordum Mundi". El estudio aplica métodos computacionales para analizar la estructura armónica de los diagramas cosmológicos del siglo XVII de Robert Fludd, con un enfoque específico en el Monochordum Mundi.

## Hallazgos Principales

- **Codificación Musical**: Identificación de un intervalo 16:15 estadísticamente significativo (p < 0.001) en el nodo de la Tierra en el diagrama de Fludd
- **Conexión con Kepler**: El intervalo medido coincide con la relación 16:15 que Kepler asignó a la excentricidad orbital de la Tierra
- **Análisis Textual**: Detección de una sobrerepresentación estadísticamente significativa de caracteres musicales en textos rosacrucianos relacionados

## Estructura del Repositorio

```
harmonia-occulta/
├── data/                   # Datos crudos y procesados
│   ├── images/            # Imágenes fuente de las obras de Fludd
│   ├── measurements/      # Mediciones y coordenadas extraídas
│   └── text/              # Textos fuente y datos de frecuencia de caracteres
├── notebooks/             # Cuadernos Jupyter para el análisis
│   ├── omr_pipeline.ipynb # Pipeline de Reconocimiento Óptico de Música
│   └── text_analysis.ipynb # Análisis estadístico de textos
├── src/                   # Código fuente
│   ├── omr/               # Herramientas de Reconocimiento Óptico de Música
│   └── analysis/          # Herramientas de análisis estadístico
├── outputs/               # Salidas y visualizaciones generadas
├── docs/                  # Documentación y materiales complementarios
└── environment.yml        # Especificación del entorno Conda
```

## Primeros Pasos

### Requisitos Previos

- Python 3.8+
- Conda (recomendado) o pip

### Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/AlkaiDynamics/Harmonia-Occulta.git
   cd Harmonia-Occulta
   ```

2. Crea y activa el entorno conda:
   ```bash
   conda env create -f environment.yml
   conda activate harmonia-occulta
   ```

3. Instala el paquete en modo de desarrollo:
   ```bash
   pip install -e .
   ```

## Uso

### Ejecución del Pipeline de OMR

```bash
python -m src.omr.pipeline --input data/images/monochordum_mundi.tif --output outputs/measurements/
```

### Reproducción del Análisis

1. Inicia Jupyter Lab:
   ```bash
   jupyter lab
   ```

2. Abre y ejecuta los cuadernos en el directorio `notebooks/`

## Datos

Las imágenes fuente se obtienen del archivo digital de la Colección Wellcome sobre las obras de Robert Fludd. Los datos procesados y las mediciones se incluyen en el directorio `data/`.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT - consulta el archivo [LICENSE](LICENSE) para obtener más detalles.

## Citación

Si utilizas este trabajo en tu investigación, por favor cítalo:

```bibtex
@article{sherer2025completed,
  title={The Completed Harmony: A Computational Pilot Study of Musical Encodings in Robert Fludd's Monochordum Mundi},
  author={Sherer, Morgan H.},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={2025}
}
```

## Agradecimientos

- A la Colección Wellcome por proporcionar acceso digital a las obras de Fludd
- A las comunidades más amplias de humanidades digitales y musicología computacional por sus herramientas y metodologías
