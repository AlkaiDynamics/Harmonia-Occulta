# Harmonia Occulta: A Computational Study of Robert Fludd's Monochordum Mundi

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1234567.svg)](https://doi.org/10.5281/zenodo.1234567)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## Overview

This repository contains the code and data for the paper "The Completed Harmony: A Computational Pilot Study of Musical Encodings in Robert Fludd's Monochordum Mundi." The study applies computational methods to analyze the harmonic structure of Robert Fludd's 17th-century cosmological diagrams, with a focus on the Monochordum Mundi.

## Key Findings

- **Musical Encoding**: Identification of a statistically significant (p < 0.001) 16:15 interval at the Earth node in Fludd's diagram
- **Kepler Connection**: The measured interval matches the 16:15 ratio Kepler assigned to Earth's orbital eccentricity
- **Textual Analysis**: Detection of a statistically significant over-representation of musical characters in related Rosicrucian texts

## Repository Structure

```
harmonia-occulta/
├── data/                   # Raw and processed data
│   ├── images/            # Source images of Fludd's works
│   ├── measurements/      # Extracted measurements and coordinates
│   └── text/              # Source texts and character frequency data
├── notebooks/             # Jupyter notebooks for analysis
│   ├── omr_pipeline.ipynb # Optical Music Recognition pipeline
│   └── text_analysis.ipynb # Statistical text analysis
├── src/                   # Source code
│   ├── omr/               # Optical Music Recognition tools
│   └── analysis/          # Statistical analysis tools
├── outputs/               # Generated outputs and visualizations
├── docs/                  # Documentation and supplementary materials
└── environment.yml        # Conda environment specification
```

## Getting Started

### Prerequisites

- Python 3.8+
- Conda (recommended) or pip

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AlkaiDynamics/Harmonia-Occulta.git
   cd Harmonia-Occulta
   ```

2. Create and activate the conda environment:
   ```bash
   conda env create -f environment.yml
   conda activate harmonia-occulta
   ```

3. Install the package in development mode:
   ```bash
   pip install -e .
   ```

## Usage

### Running the OMR Pipeline

```bash
python -m src.omr.pipeline --input data/images/monochordum_mundi.tif --output outputs/measurements/
```

### Reproducing the Analysis

1. Launch Jupyter Lab:
   ```bash
   jupyter lab
   ```

2. Open and run the notebooks in the `notebooks/` directory

## Data

Source images are derived from the Wellcome Collection's digital archive of Robert Fludd's works. Processed data and measurements are included in the `data/` directory.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Citation

If you use this work in your research, please cite:

```bibtex
@article{sherer2025completed,
  title={The Completed Harmony: A Computational Pilot Study of Musical Encodings in Robert Fludd's Monochordum Mundi},
  author={Sherer, Morgan H.},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={2025}
}
```

## Acknowledgements

- The Wellcome Collection for providing digital access to Fludd's works
- The broader digital humanities and computational musicology communities for their tools and methodologies
